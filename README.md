# paru-completion-hook

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
