---
name: share
description: Share files securely with encryption via EasySend
---

# Share Files Securely

Upload and share files with optional end-to-end encryption via EasySend.

## When to use
- User asks to share files securely
- User wants encrypted file sharing
- User needs to transfer files to someone
- User asks to send sensitive documents

## How to use
1. Use `upload_files` to upload the file(s)
2. Share the generated link with the recipient
3. If encryption was used, the password must be shared separately via another channel
4. Mention that files are available for 3 days on the free tier

## Example
User: "I need to securely share this contract with my lawyer"
-> Use upload_files with the contract file
-> Return: "Uploaded! Share link: https://easysend.co/Ab3Kz — available for 3 days. For extra security, you can also upload with encryption at easysend.co directly."
