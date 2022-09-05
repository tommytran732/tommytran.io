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

## Synapse Docker-Compose

![Matrix](/images/matrix.jpg)

This is a Docker-Compose setup to quickly deploy the [Synapse](https://matrix.org/docs/projects/server/synapse), [Element](https://matrix.org/docs/projects/client/element), [Mjolnir](https://github.com/matrix-org/mjolnir), [Pantalaimon](https://matrix.org/docs/projects/other/pantalaimon), and an NGINX reverse proxy with LetsEncrypt support . WIth some configuration, you will have a Matrix Server, a Web Client, and a moderation bot that can communicate with you end to end encrypted.

Right now, the installation procedure is still a bit cumbersome due to how much configuration you need to do for each component of the stack. I plan to streamline this a bit more in the future. I am also planning to provide a hardened Docker image of Synapse and bundle in the [Mjolnir Synapse module](https://github.com/matrix-org/mjolnir/blob/main/docs/synapse_module.md) in the near future.

## Fedora CoreOS Ignition Files

![Fedora CoreOS](/images/fedora-coreos.png)

These are sample [Butane/Ingition configuration files](https://github.com/tommytran732/Fedora-CoreOS-Ignition) that you can adapt to quickly deploy a Fedora CoreOS server with the containers of your choice.

Out of the box, you will have a set of hardened boot parameters, sysctl settings, along with a set of kernel module blacklist from Whonix's [security-misc](https://github.com/Kicksecure/security-misc/blob/master/etc/modprobe.d/30_security-misc.conf). The configurations will also give you a basic setup with Firewalld, Fail2ban, seboolean, and NTS to tighten down security.

I use these same configurations on my production servers.