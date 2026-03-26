---
name: easysend
description: Upload and share files via EasySend
---

Upload files to EasySend for instant sharing. No signup or API key required.

## Usage
- `/easysend upload <file>` — Upload a file and get a share link
- `/easysend info <code>` — Get info about a bundle (files, sizes, expiry)
- `/easysend download <code>` — Download all files from a bundle
- `/easysend status <code>` — Quick status check (alive/expired)

## Examples
- `/easysend upload ./report.pdf` — Uploads and returns share link
- `/easysend info Ab3Kz` — Shows file list for bundle Ab3Kz
- `/easysend download Xk9Pq` — Downloads all files from bundle to current directory

## Notes
- Free tier: up to 1GB, available for 3 days
- No authentication required
- Any file type accepted
- Multiple files bundled under one link
