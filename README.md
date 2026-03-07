# ansible_pull_desktop

Desktop bootstrap repo for Debian/Ubuntu-based systems using `ansible-pull`.

## What it does

- installs base desktop packages
- optionally installs Google Chrome
- optionally installs Tailscale
- applies desktop settings
- manages local user configuration

## Bootstrap

```bash
sudo apt update
sudo apt install -y ansible git
ansible-pull -U https://github.com/brownkurts/ansible_pull_desktop.git