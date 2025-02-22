---
# Basic Options
title: So your Ubuntu installation is off
date: 2025-02-21
categories: [Ubuntu, Tutorial]
tags: [Ubuntu, Tutorial, Installation]

# Additional Options
author: IronDingo
pin: true    # pins post to top
math: true   # enables math formatting
mermaid: true # enables mermaid diagrams
image:
  path: https://allpcworld.com/wp-content/uploads/2016/09/Ubuntu-latest-version-free-download.jpg
  alt: Ubuntu
---

# Fix fkn everything

If you can't upgrade, can't update and everything seems off. Run:

```bash
sudo do-release-upgrade
```

This will download for a while, you'll need a hot beverage and be ready to press "y" when prompted basically.


# Get Gnome
Gnome install command
```bash
sudo apt install ubuntu-gnome-desktop
```

Remove plasma because why not
```bash
sudo apt remove --purge plasma-desktop
```
```bash
sudo apt autoremove
```

# Your VM wont full-screen?
No worries, update your vmware tools
```bash
sudo apt install open-vm-tools
```

# Get the theme beautiful

```bash
sudo apt install gnome-tweaks
```

## Choose a Theme:
Adwaita (Default Enhanced): GNOME’s default, polished with variants like Adwaita-dark. Comes with GNOME.
Yaru: Ubuntu’s modern theme, sleek and intuitive. Install with sudo apt install yaru-theme-gnome-shell yaru-theme-gtk yaru-theme-icon (Yaru Theme on GitHub).
Pop!_OS Theme: Clean and flat, available via sudo apt install pop-theme if repositories are added (Pop!_OS Themes).

## Apply the Theme:
Open GNOME Tweaks ("Tweaks" in the app menu).
Go to "Appearance," select your theme (e.g., Yaru) for Shell, GTK, and Icons.
For icons, try "Yaru" or download "Papirus" with sudo apt install papirus-icon-theme for a lighter, plentiful look (Papirus Icon Theme).

## Resource Recommendation:
Visit Reddit for a vast collection of themes and icons. Download .tar.gz files, extract to ~/.themes or ~/.icons, and apply via Tweaks (Get a guide to GNOME Themes).
Example: Search for "Nordic" or "Arc" for smooth, modern options.

## pling.com

Go to pling.com and get a theme.



## VM not recognizing usb devices?

Fret not. Change the .vmx config file to

```md
usb.restrictions.defaultAllow = "TRUE"
```
