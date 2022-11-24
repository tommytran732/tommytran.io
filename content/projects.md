---
title: "Projects"
date: 2022-09-02
---

## PrivSec.dev

![Privsec.dev](/images/privsec.png)

[PrivSec.dev](https://privsec.dev) is a website made by me and a couple of friends. The goal is to provide practical privacy and security advice for the end user. You can think of it as a shared blog focusing on this topic.

We focus on in-depth system configuration, security analysis, and software/hardware recommendations. Our site is based on technical merits, not ideologies and politics.

## ArcticFoxes.net

![ArcticFoxes.net](/images/arcticfoxes.png)

[ArcticFoxes.net](https://arcticfoxes.net) is a group of self hosted and federated services run by me. It consists of:

- [A Matrix server](https://matrix.arcticfoxes.net) using my [hardened docker image](https://github.com/tommytran732/Synapse-Docker). I also have a [web client](https://element.arcticfoxes.net) and TURN server as accessories for the Matrix server.
- [A OpenVPN to ONC converter](onc.arcticfoxes.net). This is a simpel fork of [thomkeh/ovpn2onc](https://github.com/thomkeh/ovpn2onc) with a dark theme.

Most of the configurations and deployment files are available on [GitHub](https://github.com/ArcticFoxes-net).

## Pterodactyl Script

![Pterodactyl](/images/pterodactyl.png)

The [Pterodactyl Script](https://github.com/tommytran732/Pterodactyl-Script) is a bash script I wrote to automate the fairly tedious installation process of the popuar Pterodactyl control panel. It comes with automatic SSL certificate generation using Certbot, MariaDB SSL, basic firewall configuration, Fail2ban, and optional phpMyAdmin support. With this script, a 30-40 minutes task for a seasoned system administrator could be completed in under 5 minutes. This is my most popular project to date, with over 150 stars on GitHub.

## Arch Install Script

![Arch Linux](/images/archlinux.jpg)

The Arch Setup Script is a script that I wrote to automate my Arch Linux installation which mimics openSUSE's setup with BTRFS and Snapper. At the time, there was no other installer that does this nicely because they all use the same flat layout as recommended in the Arch Wiki. The downside of using this layout is that snapper rollback does not work properly and the user has to get into the Arch ISO to manually rollback their system. This could be solved by using the openSUSE's layout for BTRFS, and I forked Easy Arch to do just that.

Over time, I have been adding more security/privacy related settings by default (such as randomized MAC address, IPv6 Privacy, Apparmor, Kernel module blacklist, encrypted /boot). The project is still actively developed, and many of the changes I made are merged upstream as well.

## Fedora CoreOS Ignition Files

![Fedora CoreOS](/images/fedora-coreos.png)

These are sample [Butane/Ingition configuration files](https://github.com/tommytran732/Fedora-CoreOS-Ignition) that you can adapt to quickly deploy a Fedora CoreOS server with the containers of your choice.

Out of the box, you will have a set of hardened boot parameters, sysctl settings, along with a set of kernel module blacklist from Whonix's [security-misc](https://github.com/Kicksecure/security-misc/blob/master/etc/modprobe.d/30_security-misc.conf). The configurations will also give you a basic setup with Firewalld, Fail2ban, seboolean, and NTS to tighten down security.

I use these same configurations on my production servers.