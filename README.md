<div align="center">

# VoidGram

**Your Instagram. Your desktop. Your rules.**

![Latest Release](https://img.shields.io/github/v/release/REMvisual/VoidGram-releases?label=latest&color=ffb800)
![Downloads](https://img.shields.io/github/downloads/REMvisual/VoidGram-releases/total?color=22c55e)
![Platform](https://img.shields.io/badge/platform-Windows-blue)
![License](https://img.shields.io/badge/license-Elastic%202.0-yellow)

Free desktop app for posting images, reels, stories, and carousels to Instagram.
Self-hosted. No subscriptions. Your data stays on your machine.

[**Download Latest Release**](https://github.com/REMvisual/VoidGram-releases/releases/latest)

</div>

---

## What is VoidGram?

VoidGram is a desktop application that lets you create, schedule, and publish Instagram content without opening a browser or scrolling your feed. Connect your Instagram Business or Creator account, drag in your media, write your caption, and post -- all from your desktop. No cloud accounts to sign up for, no monthly fees, and no one else touching your data.

## Key Features

- **Post anything** -- images, reels, stories, and multi-image carousels, all from one interface
- **Schedule posts** -- pick any date and time; posts publish automatically, even while you sleep
- **Auto story reposter** -- automatically repost feed posts to your story on a schedule
- **Collaborator tagging** -- invite collaborators directly from the post form
- **User tags and location tagging** -- tag people in photos and add locations to any post
- **Text overlays on stories** -- add styled text to story images without a separate editor
- **Local or cloud scheduling** -- schedule with the app running, or deploy a Cloudflare Worker for hands-off publishing when the app is closed
- **Built-in setup wizard** -- guided configuration from first launch to first post, no technical knowledge required
- **Auto-updates** -- the app checks for new versions and updates itself in the background
- **Source available** -- the full source code is available for inspection and self-hosting

## Download

| Asset | Link |
|-------|------|
| **Windows Installer** | [**Download latest .exe**](https://github.com/REMvisual/VoidGram-releases/releases/latest) |

**Already installed?** VoidGram checks for updates automatically. You will be prompted to install new versions when they are available.

### System Requirements

- Windows 10 or later (64-bit)
- An Instagram Business or Creator account connected to a Facebook Page
- A Meta Developer App (the setup wizard walks you through creating one)

## Quick Start

1. **Download** the latest installer from the [Releases page](https://github.com/REMvisual/VoidGram-releases/releases/latest).
2. **Install** by running the `.exe` -- no admin privileges required, installs to your user folder.
3. **Set up** using the built-in wizard. It guides you through connecting your Meta Developer App and Instagram account step by step.
4. **Post** -- drag in an image or video, write your caption, and hit publish.

## Screenshots

<!-- TODO: Add screenshots -->
<!-- Suggested: setup wizard, create post view, schedule view, post history -->

## How It Works

VoidGram connects to Instagram through the **official Instagram Graph API** -- the same API that professional social media tools use. Your content is uploaded through Meta's servers, exactly as if you posted from the Instagram app.

- **All data stored locally** -- your account tokens, post history, and media files live in a SQLite database on your machine. Nothing is sent to any third-party server.
- **Publishing while running** -- when the app is open, scheduled posts are processed by a local job queue. No external services required.
- **Cloud scheduling (optional)** -- for posts scheduled outside your working hours, you can deploy a lightweight Cloudflare Worker that publishes on your behalf. This is fully optional and configured through the app's settings.

## Security

- Access tokens are **encrypted at rest** using AES encryption before being stored in the local database.
- All communication with Instagram and Meta uses **HTTPS**.
- The full source code is **available for inspection** -- you can verify exactly what the app does with your credentials.
- VoidGram never transmits your data to any server other than Meta's official API endpoints (and optionally, your own Cloudflare Worker).

Found a security issue? Please report it responsibly by opening a private issue or contacting REMvisual directly on GitHub.

## Support the Project

VoidGram is free and always will be. If it saves you time or makes your workflow better, consider supporting continued development.

<!-- TODO: Add donation/sponsorship link -->

## License

VoidGram is released under the [**Elastic License 2.0 (ELv2)**](https://www.elastic.co/licensing/elastic-license).

In short:
- **Free to use** for any purpose, personal or commercial.
- **Free to modify** and run your own builds.
- **You may not** offer VoidGram as a managed or hosted service to third parties.
- **You may not** redistribute VoidGram or create derivative products for sale.

This license protects the project while keeping it free and open for individual users.

## Links

- [**Website**](https://voidgram.org)
- [**Release Notes**](https://github.com/REMvisual/VoidGram-releases/releases)
- [**Report an Issue**](https://github.com/REMvisual/VoidGram-releases/issues)
- [**Discussions**](https://github.com/REMvisual/VoidGram-releases/discussions)

---

<div align="center">

Built by [REMvisual](https://github.com/REMvisual)

</div>
