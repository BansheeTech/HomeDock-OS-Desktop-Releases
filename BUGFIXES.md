# Bugfixes

## How to Report Bugs

If you encounter a bug while using HomeDock OS Desktop, please report it through any of the following channels:

📧 Email – **support@homedock.cloud**

💬 **Discord** – open a ticket in `#support-ticket` at [discord.gg/Zj3JCYsRWw](https://discord.gg/Zj3JCYsRWw)

🐙 **GitHub** – open an issue at [github.com/BansheeTech/HomeDockOS/issues/new](https://github.com/BansheeTech/HomeDockOS/issues/new)

We greatly appreciate every report from our community. Each one helps us make HomeDock OS Desktop more stable, reliable, and enjoyable to use. Thank you for contributing!

---

## Bugfix History

- `✦ Ubuntu 22.04 Rootfs Download Fails with 0KB File (Windows)`

  - **Reported on Discord by Jatin** – Fixed
  - The Ubuntu 22.04 rootfs download from the Ubuntu CDN on Windows was not following HTTP redirects, resulting in an empty redirect response being written to disk instead of the actual ~500MB rootfs archive. Additionally, the existence check was performed against the VHDX WSL2 disk file rather than the `tar.gz` archive itself, so any manually placed rootfs file was overwritten on every launch. Now follows the same redirect-aware download path already used for the Docker Compose download and validates the archive presence before re-downloading.
