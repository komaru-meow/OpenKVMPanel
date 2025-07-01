<p align="center">
  <img src="https://github.com/kvm-i7/.github/blob/main/profile/logo.png?raw=true" alt="KVM-i7 Logo" width="150">
</p>

<h1 align="center">Official KVM-i7 Web Panel</h1>

<p align="center">
  <strong>A lightweight, client-side web interface for managing your KVM-i7 VPS.</strong>
</p>

<p align="center">
  <a href="https://discord.gg/t3vps"><img src="https://img.shields.io/badge/Join_Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white"></a>
  <a href="https://github.com/KVM-i7/OpenKVMPanel/issues"><img src="https://img.shields.io/badge/Report_an_Issue-orange?style=for-the-badge&logo=github"></a>
</p>

---

## What Is This?

This is the official, open-source web panel for managing your KVM-i7 lifetime VPS. It's a single, static HTML file that uses JavaScript to interact directly with the [KVM-i7 REST API](https://github.com/KVM-i7). It provides a simple graphical interface as an alternative to using Discord bot commands.

Below is a image of what the panel looks like.

![](https://github.com/user-attachments/assets/c060912d-1d92-40fb-9b42-f4c900923739)

### Features

*   **Server Control:** Start, Stop, and Reinstall your VPS.
*   **Live Status:** View the current status (running, stopped) of your server.
*   **Resource Monitoring:** See real-time CPU, RAM, and disk usage.
*   **Secure & Client-Side:** Your API token is **never** sent to our servers or stored anywhere. It is only kept in your browser's memory for the duration of your session and is sent directly to the API endpoint.

## How to Use

There are two ways to use the panel:

### 1. The Official Hosted Version (Recommended)

The easiest way is to use the official version hosted by us. No setup required.

**➡️ [https://panel.kvm-i7.host](https://panel.kvm-i7.host)**

### 2. Self-Hosting

Since this is just a single `index.html` file, you can easily host it yourself for maximum privacy and control.

1.  **Download:** Download the `index.html` file from this repository.
2.  **Run it:**
    *   Simply open the file in your local web browser.
    *   Or, upload it to any static hosting service (like Vercel, Netlify, GitHub Pages, or even your own KVM-i7 VPS!).

## How It Works (Security)

This panel is designed with security as a top priority.

*   It is a **fully client-side application**. This means all the logic runs in your web browser.
*   When you enter your API token, it is stored in a JavaScript variable within the page.
*   All API requests are made **directly from your browser to the KVM-i7 API** (`https://platform.kvm-i7.host`).
*   **Your token never get's sent to a database.** This is verifiable by inspecting the source code in this repository and monitoring your browser's network requests.

> **Warning:** Always be cautious about where you enter your API token. Only use the official panel or trusted community panels that are open-source and verifiable. Your API token provides full control over your VPS.

## Contributing

We welcome contributions from the community!

*   **Found a bug?** [Open an issue.](https://github.com/KVM-i7/OpenKVMPanel/issues)
*   **Have a feature request?** [Open an issue](https://github.com/KVM-i7/OpenKVMPanel/issues) and describe what you'd like to see.
*   **Want to submit a change?** Fork the repository and submit a pull request with your improvements.

This project is released under the MIT License.
