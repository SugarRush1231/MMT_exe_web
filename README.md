# Multi Media Toolkit Download Page

Simple static download page for Cloudflare Pages.

## Folder structure

```text
download-page/
  index.html
  versions.json
  versions.js
  files/
    MMT_Setup_v1.3.0.exe
    MMT_Setup_v1.2.2.exe
```

## How to add a version

1. Put the exe file in `files`.
2. Add or edit an item in `versions.js`.
3. If you also want a JSON copy for later API use, update `versions.json`.
4. Deploy the folder to Cloudflare Pages.

## Version item

```json
{
  "type": "latest",
  "version": "1.3.0",
  "note": "Current latest version.",
  "file": "files/MMT_Setup_v1.3.0.exe"
}
```

Use `latest`, `stable`, `backup`, or `test` for `type`.
