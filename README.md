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

`paru-completion-hook` is authored and maintained by **[Vikyek](https://github.com/Vikyek)** as an independent open-source project. Everything is 100% open-source, telemetry-free, and public.

<div align="center">


[![Sponsor Vikyek](https://img.shields.io/badge/Sponsor-%E2%9D%A4-ea4aaa?logo=github&style=for-the-badge)](https://github.com/sponsors/Vikyek)
[![Donate on Liberapay](https://img.shields.io/badge/Donate-Liberapay-f6c915?style=for-the-badge&logo=liberapay&logoColor=black)](https://liberapay.com/Vikyek)
[![Donate with Stripe](https://img.shields.io/badge/Donate-Stripe-635BFF?style=for-the-badge&logo=stripe&logoColor=white)](https://profile.stripe.com/@vikyek)

</div>

> ### 🎯 Active Sponsorship Goal: Monthly Living Essentials
> **Target:** **2,710 PLN / ~$680 USD per month** (`630 PLN / week`) — Rent & Essential Utilities  
> Covering basic living essentials directly unlocks dedicated, sustainable full-time independent open-source engineering across Arch Linux ecosystem tools free from corporate telemetry, ads, or paywalls.

If `paru-completion-hook` improves your Arch Linux shell workflow, consider supporting ongoing work:

- **GitHub Sponsors**: [github.com/sponsors/Vikyek](https://github.com/sponsors/Vikyek) *(Monthly tiers and one-time tips)*
- **Liberapay**: [liberapay.com/Vikyek](https://liberapay.com/Vikyek) *(0% platform fee recurrent patronage in EUR/USD/PLN)*
- **Direct Stripe Profile**: [profile.stripe.com/@vikyek](https://profile.stripe.com/@vikyek) *(Direct one-time tips & sponsorship)*

Every contribution—monthly or one-time—directly supports active maintenance, hardware testbeds, and new feature development!

---

## License

This project is licensed under the [MIT License](LICENSE).

