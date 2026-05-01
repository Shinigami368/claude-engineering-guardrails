# EKS Upgrade Runbook

This document describes the official procedure for upgrading Amazon EKS clusters.

The process ensures clusters remain secure, stable, and compatible with AWS services.

---

# PURPOSE

Regular EKS upgrades help:

- maintain security patches and bug fixes
- gain access to new Kubernetes features
- maintain compatibility with AWS services
- avoid extended support fees for outdated versions

---

# PREREQUISITES

This section helps engineers performing upgrades for the first time.

---

# TERMINOLOGY

StorageClass enables dynamic provisioning of volumes.

If no StorageClass is marked as default, PersistentVolumeClaims without a storageClassName will fail.

---

# READ DOCUMENTATION

Before upgrading always review addon compatibility documentation.

VPC CNI

https://docs.aws.amazon.com/eks/latest/userguide/managing-vpc-cni.html

CoreDNS

https://docs.aws.amazon.com/eks/latest/userguide/managing-coredns.html

Kube Proxy

https://docs.aws.amazon.com/eks/latest/userguide/managing-kube-proxy.html

---

# WARNING AREA

The environment uses a free Docker Hub account.

Docker Hub rate limits image pulls to 100 pulls per 6 hours per cluster.

Large clusters may hit this limit during upgrades.

If HTTP 429 errors occur or images fail to pull:

Use mirrored images from the operations repository:

https://github.com/Remangu/dockerhub-mirror

Alternative mirrors:

public.ecr.aws/docker/library/<image>

mirror.gcr.io/<image>

---

# CLI PREPARATION

Pull cluster contexts to your local machine.

Instructions:

https://github.com/Remangu/operations-internal

---

# REQUIRED TOOLS

silver-surfer

Tool used to detect Kubernetes API deprecations.

Installation:

go install github.com/devtron-labs/silver-surfer@latest

Ensure GOPATH is set correctly.

Verify installation:

silver-surfer --version

kubectx

Tool for switching between Kubernetes contexts.

https://github.com/ahmetb/kubectx

---

# UPGRADE PROCEDURE

1 Ensure correct Kubernetes context

Example:

kubectx

Switch to the cluster that will be upgraded.

---

2 Run silver-surfer

Check API compatibility with the target Kubernetes version.

Example:

silver-surfer --target-kubernetes-version 1.31

If output is empty no API migration is required.

---

3 Verify default storage class

Run:

kubectl get storageclass

Ensure one storage class is marked as default.

This is required for Kubernetes version 1.30+.

---

4 Determine compatible addon versions

Use AWS CLI:

export TARGET_VERSION="1.32"

for addon in vpc-cni coredns kube-proxy aws-ebs-csi-driver; do
aws eks describe-addon-versions \
--addon-name $addon \
--kubernetes-version "$TARGET_VERSION"
done

Record compatible versions.

---

5 Create upgrade branch

Branch naming convention:

feature/eks-upgrade-<version>-<environment>

Example:

feature/eks-upgrade-1.32-production

---

6 Update Terraform variables

Update terraform.tfvars values.

Example:

cluster_version    = "1.31"
vpc_cni_version    = "v1.19.6-eksbuild.1"
coredns_version    = "v1.11.4-eksbuild.14"
kube_proxy_version = "v1.31.9-eksbuild.2"
ebs_csi_version    = "v1.45.0-eksbuild.2"

Also update worker AMI filters if required.

---

7 Create Pull Request

Push the branch and open a PR.

Receive approval from team or customer if required.

---

8 Atlantis Terraform plan

Atlantis automatically runs terraform plan for each environment.

Review plan output carefully.

---

9 Apply environments

Run Atlantis apply per environment.

Example:

atlantis apply -d terraform/develop

Repeat for stage and production.

---

10 Merge PR

Once all environments are successfully upgraded merge the PR.

---

# POST UPGRADE VERIFICATION

Run cluster health checks.

Commands:

kubectl get nodes
kubectl get pods -A
kubectl get events -A

Confirm:

nodes upgraded
pods healthy
system components stable

Monitor cluster behaviour for at least 30 minutes.

---

# KNOWN ISSUES

VerticalFox cluster

Grafana pod may temporarily crashloop during upgrade.

It typically stabilizes automatically after approximately 2 hours.

---

# REFERENCES

Docker Hub rate limit troubleshooting

https://repost.aws/knowledge-center/ecs-pull-container-error-rate-limit