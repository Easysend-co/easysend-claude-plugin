# EasySend Plugin for Claude Code

Upload, download, and share files instantly from Claude Code. No signup, no API key, no configuration.

## Install

```
/install easysend
```

Or manually add to `~/.claude/settings.json`:
```json
{
    "mcpServers": {
        "easysend": {
            "command": "npx",
            "args": ["-y", "easysend-mcp"]
        }
    }
}
```

## What You Can Do

Just ask Claude naturally:

| You say | What happens |
|---------|-------------|
| "Upload this file to EasySend" | Uploads and returns a share link |
| "Share these logs with my teammate" | Bundles files under one link |
| "What's in easysend.co/Ab3Kz?" | Lists files with sizes |
| "Download the files from that bundle" | Saves all files locally |

## Tools

| Tool | Description |
|------|-------------|
| `upload_files` | Upload one or more files, get a share link |
| `get_bundle` | Get bundle info (files, sizes, expiry, downloads) |
| `download_file` | Download a single file by ID |
| `download_bundle` | Download all files in a bundle |
| `delete_file` | Delete a file (requires upload_token) |
| `bundle_status` | Quick alive/expired check |

## Slash Command

```
/easysend upload ./report.pdf
/easysend info Ab3Kz
/easysend download Xk9Pq
```

## No API Key Required

EasySend's API is free and public. The plugin works immediately with zero configuration.

## Features

- Any file type, up to 1GB free
- Files available for 3 days (upgradeable)
- Optional end-to-end encryption
- Multiple files bundled under one link
- QR code for each bundle
- Download notifications

## Links

- [EasySend](https://easysend.co) — Website
- [API Docs](https://easysend.co/api) — REST API
- [MCP Docs](https://easysend.co/mcp) — MCP integration details

## License

MIT
