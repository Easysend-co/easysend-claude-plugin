---
name: upload
description: Upload files to EasySend and get a shareable link
---

# Upload Files to EasySend

Use the easysend MCP tools to upload files and get a shareable link. No signup or API key required.

## When to use
- User asks to share a file or files
- User wants to upload a file to get a link
- User needs to send files to someone
- User asks about file sharing or file transfer
- User says "share this", "send this file", "upload this"

## How to use
1. Use the `upload_files` tool with the file path(s)
2. Optionally add a `description` for context
3. Return the share URL to the user
4. Mention the upload token if they may want to add/delete files later

## Example
User: "Share this log file with my team"
-> Use upload_files tool with the file path
-> Return: "Here's your share link: https://easysend.co/Ab3Kz — anyone with this link can download the file. Available for 3 days."

User: "Upload report.pdf and data.csv together"
-> Use upload_files with both paths
-> Return: "Both files uploaded to one bundle: https://easysend.co/Xk9Pq"
