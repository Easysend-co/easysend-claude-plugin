---
name: download
description: Download files from an EasySend bundle
---

# Download Files from EasySend

Use the easysend MCP tools to download files from a shared bundle.

## When to use
- User provides an easysend.co link
- User asks to download files from EasySend
- User asks "what files are in this bundle?"
- User pastes a short code like "Ab3Kz"

## How to use
1. Extract the short code from the URL (e.g., Ab3Kz from easysend.co/Ab3Kz)
2. Use `get_bundle` tool to see what files are available
3. Use `download_file` to save a specific file, or `download_bundle` to save all files
4. Report the saved file paths to the user

## Example
User: "Download the files from easysend.co/Ab3Kz"
-> Use get_bundle to list files
-> Use download_bundle to save all files
-> Return: "Downloaded 3 files to your current directory: report.pdf, photo.jpg, notes.txt"

User: "What's in this EasySend link: easysend.co/Mn4Rz?"
-> Use get_bundle to list files
-> Return file names, sizes, and download counts
