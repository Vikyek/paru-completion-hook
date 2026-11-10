# paru-completion-hook

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Sponsor Vikyek](https://img.shields.io/badge/Sponsor-GitHub-ea4aaa?logo=github-sponsors&logoColor=white)](https://github.com/sponsors/Vikyek)

Automated `libalpm` pacman hook and systemd path unit to dynamically regenerate and maintain the `paru` shell completion cache across Bash, Zsh, and Fish.

---

## Features
- **Automatic Triggers**: Executes automatically post-transaction upon package install, upgrade, or removal.
- **Systemd Path Monitoring**: Keeps cached completions synchronized in background environments without blocking package manager transactions.
- **Multi-Shell**: Refreshes completions for Bash, Zsh, and Fish.

---

## Installation

### Via AUR
```bash
paru -S paru-completion-hook
```

### Manual Installation
```bash
git clone https://github.com/Vikyek/paru-completion-hook.git
cd paru-completion-hook
makepkg -si
```

---

## Usage

The update runs automatically via pacman hooks. To trigger manual cache generation:

```bash
sudo paru-completion-update
```

See `man paru-completion-update` for manual pages.

---

## Support & Sponsorship

`paru-completion-hook` is authored and maintained by **[Vikyek](https://github.com/Vikyek)** as an independent open-source project.

> ### 🎯 Active Sponsorship Goal: Monthly Living Essentials
> **Target:** **2,710 PLN / ~$675 USD per month** (Rent & Utilities)  
> Covering basic living essentials directly unlocks dedicated, sustainable full-time independent open-source engineering across Arch Linux ecosystem tools.

If `paru-completion-hook` improves your Arch Linux shell workflow, consider supporting my work:

- **GitHub Sponsors**: [github.com/sponsors/Vikyek](https://github.com/sponsors/Vikyek)

---

## License

This project is licensed under the [MIT License](LICENSE).

