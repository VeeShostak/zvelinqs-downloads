# Zvelinqs downloads

Zvelinqs is a private workspace for mail and notes. It runs on your computer. There is no Zvelinqs account, no cloud, and no telemetry.

This repository holds the installers. The application source is private.

## Download the latest version

| Platform | Download |
| --- | --- |
| Mac, Apple silicon | [Zvelinqs-mac-arm64.dmg](https://github.com/VeeShostak/zvelinqs-downloads/releases/latest/download/Zvelinqs-mac-arm64.dmg) |
| Mac, Intel | [Zvelinqs-mac-x64.dmg](https://github.com/VeeShostak/zvelinqs-downloads/releases/latest/download/Zvelinqs-mac-x64.dmg) |
| Linux, x86_64 | [Zvelinqs-linux-x86_64.AppImage](https://github.com/VeeShostak/zvelinqs-downloads/releases/latest/download/Zvelinqs-linux-x86_64.AppImage) |
| Linux, x86_64 Debian package | [Zvelinqs-linux-amd64.deb](https://github.com/VeeShostak/zvelinqs-downloads/releases/latest/download/Zvelinqs-linux-amd64.deb) |
| Linux, arm64 | [Zvelinqs-linux-arm64.AppImage](https://github.com/VeeShostak/zvelinqs-downloads/releases/latest/download/Zvelinqs-linux-arm64.AppImage) |
| Windows, x64 | [Zvelinqs-win-x64.exe](https://github.com/VeeShostak/zvelinqs-downloads/releases/latest/download/Zvelinqs-win-x64.exe) |
| Windows, arm64 | [Zvelinqs-win-arm64.exe](https://github.com/VeeShostak/zvelinqs-downloads/releases/latest/download/Zvelinqs-win-arm64.exe) |

The [latest release](https://github.com/VeeShostak/zvelinqs-downloads/releases/latest) also includes the Mac zip files, the Linux arm64 Debian package, and `SHA256SUMS.txt`.

## macOS first open

Zvelinqs is not notarized by Apple yet. macOS may say it cannot verify the app.

1. Open the `.dmg` and drag Zvelinqs into Applications.
2. Open Zvelinqs from Applications.
3. If macOS blocks it, open System Settings, Privacy & Security, and choose **Open Anyway**.
4. If macOS says the app is damaged, open Terminal and run:

```bash
xattr -dr com.apple.quarantine /Applications/Zvelinqs.app
```

A signed and notarized build will remove this step.

## Linux

AppImage:

```bash
chmod +x Zvelinqs-linux-x86_64.AppImage
./Zvelinqs-linux-x86_64.AppImage
```

For Debian or Ubuntu, open the `.deb` with your software installer.

## Windows

Run the `.exe`. If SmartScreen appears, choose **More info**, then **Run anyway**.

## What it does

- Reads mail directly from your mail server with an app password.
- Keeps notes as plain Markdown files in a folder you own.
- Connects to a GitHub vault in one step. Sync starts off, so nothing is sent until you turn it on.
- Brings a local agent into the inbox for briefs, drafts, and answers with sources.
- Saves an email, a brief, or an answer to notes with one press.

## Privacy

Mail goes to your mail server. Prompts go to the model endpoint on this computer. Notes go to GitHub only after you connect a repository and turn on sync. Nothing is sent to Zvelinqs.

## Verify a download

Every release includes `SHA256SUMS.txt`.

```bash
shasum -a 256 Zvelinqs-mac-arm64.dmg
```

Compare the value with the file in the release.

## Links

- Website: https://zvelinqs.com
- Latest release: https://github.com/VeeShostak/zvelinqs-downloads/releases/latest
