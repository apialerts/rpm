# API Alerts • rpm repository

This repository hosts the rpm package repository for the [API Alerts CLI](https://github.com/apialerts/apialerts-cli), served via GitHub Pages at [rpm.apialerts.com](https://rpm.apialerts.com).

- Website: [apialerts.com](https://apialerts.com)
- Docs: [apialerts.com/docs/tools/cli](https://apialerts.com/docs/tools/cli)

> Do not edit this repository manually. It is updated automatically on each CLI release.

## Installation

```bash
sudo rpm --import https://rpm.apialerts.com/key.gpg
sudo tee /etc/yum.repos.d/apialerts.repo <<EOF
[apialerts]
name=API Alerts
baseurl=https://rpm.apialerts.com
enabled=1
gpgcheck=1
gpgkey=https://rpm.apialerts.com/key.gpg
EOF
sudo dnf install apialerts
```

## Upgrading

```bash
sudo dnf upgrade apialerts
```

## Uninstalling

```bash
sudo dnf remove apialerts
```
