# Hook Index

Hooks stay as platform-specific files. Copy only the hook pair or single file you intend to enable.

## Hook prerequisites

The Bash hook variants use `jq` to parse Claude hook payloads. Install `jq`
before enabling Bash hooks such as `pretooluse-guard.sh`,
`write-guard.sh`, or `read-injection-scanner.sh`.

The PowerShell hook variants do not use the same Bash `jq` dependency.

Hooks are optional. Enable them one at a time and verify the behavior before
using them globally.

| Hook | Purpose | Platform files | Path |
|---|---|---|---|
| `error-capture` | Capture failed Bash command output patterns after execution without echoing raw secrets. | [error-capture.sh](../.claude/hooks/error-capture.sh), [error-capture.ps1](../.claude/hooks/error-capture.ps1) | [.claude/hooks/](../.claude/hooks) |
| `notify-bell` | Ring the terminal bell when a task finishes or needs attention. | [notify-bell.sh](../.claude/hooks/notify-bell.sh), [notify-bell.ps1](../.claude/hooks/notify-bell.ps1) | [.claude/hooks/](../.claude/hooks) |
| `pretooluse-guard` | Block risky shell commands before Bash execution. | [pretooluse-guard.sh](../.claude/hooks/pretooluse-guard.sh), [pretooluse-guard.ps1](../.claude/hooks/pretooluse-guard.ps1) | [.claude/hooks/](../.claude/hooks) |
| `read-injection-scanner` | Scan read and fetch results for prompt-injection style content. | [read-injection-scanner.sh](../.claude/hooks/read-injection-scanner.sh), [read-injection-scanner.ps1](../.claude/hooks/read-injection-scanner.ps1) | [.claude/hooks/](../.claude/hooks) |
| `write-guard` | Block destructive or secret-handling patterns inside write and edit payloads. | [write-guard.sh](../.claude/hooks/write-guard.sh), [write-guard.ps1](../.claude/hooks/write-guard.ps1) | [.claude/hooks/](../.claude/hooks) |
