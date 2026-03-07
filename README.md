# ansible_pull_desktop

Desktop bootstrap repo for Debian/Ubuntu systems using `ansible-pull`.

## What it does

- ensures the local desktop user exists
- installs common desktop packages
- optionally installs Google Chrome
- optionally installs Tailscale
- optionally runs `ansible-pull` from cron as root

## First-time bootstrap

```bash
sudo apt update
sudo apt install -y ansible git dconf-cli
ansible-galaxy collection install community.general
sudo ansible-pull -o -U https://github.com/brownkurts/ansible_pull_desktop.git local.yml