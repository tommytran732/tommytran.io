---
title: "Projects"
date: 2022-09-02
---

## PrivSec.dev

![Privsec.dev](/images/privsec.png)

[PrivSec.dev](https://privsec.dev) is a website made by me and a couple of friends. The goal is to provide practical privacy and security advice for the end user. You can think of it as a shared blog focusing on this topic.

We focus on in-depth system configuration, security analysis, and software/hardware recommendations. Our site is based on technical merits, not ideologies and politics.

## Pterodactyl Script

![Pterodactyl](/images/pterodactyl.png)

The [Pterodactyl Script](https://github.com/tommytran732/Pterodactyl-Script) is a bash script I wrote to automate the fairly tedious installation process of the popuar Pterodactyl control panel. It comes with automatic SSL certificate generation using Certbot, MariaDB SSL, basic firewall configuration, Fail2ban, and optional phpMyAdmin support. With this script, a 30-40 minutes task for a seasoned system administrator could be completed in under 5 minutes. This is my most popular project to date, with over 150 stars on GitHub.

## Arch Install Script

![Arch Linux](/images/archlinux.jpg)

The Arch Setup Script is a script that I wrote to automate my Arch Linux installation which mimics openSUSE's setup with BTRFS and Snapper. At the time, there was no other installer that does this nicely because they all use the same flat layout as recommended in the Arch Wiki. The downside of using this layout is that snapper rollback does not work properly and the user has to get into the Arch ISO to manually rollback their system. This could be solved by using the openSUSE's layout for BTRFS, and I forked Easy Arch to do just that. 

Over time, I have been adding more security/privacy related settings by default (such as randomized MAC address, IPv6 Privacy, Apparmor, Kernel module blacklist, encrypted /boot). The project is still actively developed, and many of the changes I made are merged upstream as well.