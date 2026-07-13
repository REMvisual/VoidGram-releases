<div align="center">

![VoidGram](./assets/readme-banner.png)

![Latest Release](https://img.shields.io/github/v/release/REMvisual/VoidGram-releases?label=latest&color=ffb800)
![Downloads](https://img.shields.io/github/downloads/REMvisual/VoidGram-releases/total?color=22c55e)
![Platform](https://img.shields.io/badge/platform-Windows-blue)
![License](https://img.shields.io/badge/license-Elastic%202.0-yellow)

Free desktop app for posting images, reels, stories, and multi-image posts to Instagram.
Runs entirely on your machine. No subscriptions. Your data stays with you.

[**Download Latest Release**](https://github.com/REMvisual/VoidGram-releases/releases/latest)

</div>

---

## What is VoidGram?

VoidGram is a desktop application that lets you create, schedule, and publish Instagram content without opening a browser or scrolling your feed. Connect your Instagram Business or Creator account, drag in your media, write your caption, and post -- all from your desktop. No cloud accounts to sign up for, no monthly fees, and no one else touching your data.

## Key Features

- **Post anything** -- images, reels, stories, and multi-image posts, all from one interface
- **Schedule posts** -- pick any date and time; posts publish automatically, even while you sleep
- **Auto story reposter** -- when someone mentions you in their story, VoidGram can repost it to your own story automatically, within safety limits you control
- **Unified inbox & Inbound hub** -- read your Instagram DMs and see everything that comes in -- story mentions, automated reposts, and collaboration invites -- in one place, each with clear status on what fired and when
- **Collaboration invites** -- VoidGram detects when someone invites you to co-author a post and lets you accept it right from the Inbound hub
- **Collaborator tagging** -- invite collaborators directly from the post form
- **User tags and location tagging** -- tag people in photos and add locations to any post
- **Text overlays on stories** -- add styled text to story images without a separate editor
- **Local or cloud scheduling** -- schedule with the app running, or deploy a Cloudflare Worker for hands-off publishing when the app is closed
- **Built-in setup wizard** -- guided configuration from first launch to first post, no technical knowledge required
- **Auto-updates** -- the app checks for new versions and updates itself in the background
- **Private by design** -- your account tokens, post history, and media never leave your computer
- **Mobile companion (in development)** -- a native mobile app to drive your VoidGram from your phone is on the way

## Download

| Asset | Link |
|-------|------|
| **Windows Installer** | [**Download latest .exe**](https://github.com/REMvisual/VoidGram-releases/releases/latest) |

**Already installed?** VoidGram checks for updates automatically. You will be prompted to install new versions when they are available.

### System Requirements

- Windows 10 or later (64-bit)
- An Instagram Business or Creator account
- No Meta Developer App required for most users -- the built-in setup wizard connects through VoidGram's shared login. (Advanced users can supply their own Meta app in the wizard.)

## Quick Start

1. **Download** the latest installer from the [Releases page](https://github.com/REMvisual/VoidGram-releases/releases/latest).
2. **Install** by running the `.exe` -- no admin privileges required, installs to your user folder.
3. **Set up** using the built-in wizard. It guides you through connecting your Instagram account step by step.
4. **Post** -- drag in an image or video, write your caption, and hit publish.

## Screenshots

<!-- TODO: Add screenshots: setup wizard, create post view, schedule view, post history -->

## How It Works

VoidGram publishes through Instagram's **official Graph API** -- the same API professional social media tools use. Your content is uploaded through Meta's servers, exactly as if you posted from the Instagram app.

- **All data stored locally** -- your account tokens, post history, and media files live in a SQLite database on your machine.
- **Publishing while running** -- when the app is open, scheduled posts are processed by a local job queue. No external services required.
- **Cloud scheduling (optional)** -- for posts scheduled outside your working hours, you can deploy a lightweight Cloudflare Worker that publishes on your behalf. This is fully optional and configured through the app's settings.

## Security & Privacy

- Access tokens are **encrypted at rest** with AES-256-GCM before being stored in the local database.
- All communication with Instagram and Meta uses **HTTPS**.
- VoidGram never transmits your data to any server other than Meta's official API endpoints (and optionally, your own Cloudflare Worker).
- The shared login proxy performs a one-shot OAuth exchange and never persists your tokens.

Found a security issue? Please report it responsibly by [opening an issue](https://github.com/REMvisual/VoidGram-releases/issues) or contacting REMvisual on GitHub.

## Support the Project

VoidGram is free and always will be. If it saves you time, consider supporting continued development:

- [Patreon](https://patreon.com/remrepo)
- [Gumroad](https://remrepo.gumroad.com)

## License

VoidGram is released under the [**Elastic License 2.0 (ELv2)**](https://www.elastic.co/licensing/elastic-license).

In short:
- **Free to use** for any purpose, personal or commercial.
- **Free to run** your own copy.
- **You may not** offer VoidGram as a managed or hosted service to third parties.
- **You may not** redistribute VoidGram or create derivative products for sale.

This releases repo is the public home for VoidGram -- downloads, issues, and discussions.

## Links

- [**Website**](https://voidgram.org)
- [**Release Notes**](https://github.com/REMvisual/VoidGram-releases/releases)
- [**Report an Issue**](https://github.com/REMvisual/VoidGram-releases/issues)
- [**Discussions**](https://github.com/REMvisual/VoidGram-releases/discussions)

---

<div align="center">

Built by [REMvisual](https://github.com/REMvisual)

</div>
