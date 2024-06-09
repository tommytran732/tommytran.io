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

## Linux Setup Scripts

![Glitched Tux](/images/glitched-tux.jpg)

These are setup [scripts I run on my Linux systems](https://github.com/TommyTran732/Linux-Setup-Scripts), and serve as the basis for my other setups. You can adapt them to deploy yours. 

Features include, but are not limited to:
- Removal of unnecessary packages
- Hardened boot parameters
- Hardened sysctl settings
- Kernel module blacklist from Whonix's [security-misc](https://github.com/Kicksecure/security-misc/blob/master/etc/modprobe.d/30_security-misc.conf)
- Mac Address randomization for desktop installations
- SSH client and server hardening
- Installation of Hardened Malloc on Red Hat systems
- Installation and configuration of Microsoft Edge policies for desktop installations
- NTS setup
- Firewall setup

## Fedora CoreOS Ignition Files

![Fedora CoreOS](/images/fedora-coreos.png)

These are sample [Butane/Ingition configuration files](https://github.com/tommytran732/Fedora-CoreOS-Ignition) that you can adapt to quickly deploy a Fedora CoreOS server with the containers of your choice. They share the same hardening as the Linux Setup Scripts.

On Fedora CoreOS, I have also included systemd services to:
- Install and update gVisor at boot
- Update containers in a Docker Compose stack once a week.

## Arch Setup Script
![Arch Linux](/images/archlinux.jpg)

The [Arch Setup Script](https://github.com/TommyTran732/Arch-Setup-Script) is a script that I wrote to automate my Arch Linux installation which mimics openSUSE's setup with BTRFS and Snapper. At the time, there was no other installer that does this nicely because they all use the same flat layout as recommended in the Arch Wiki. The downside of using this layout is that snapper rollback does not work properly and the user has to get into the Arch ISO to manually rollback their system. This could be solved by using the openSUSE's layout for BTRFS, and I forked Easy Arch to do just that.

Over time, I have been adding more security/privacy related settings. Most them which are ported from the Linux Setup Scripts repo.

## Microsoft Egde Policies

![Microsoft Edge](/images/microsoft-edge.png)

These are Microsoft Edge enterprise for the most secure web browsing experience. 

You can read through them [here](https://github.com/TommyTran732/Microsoft-Edge-Policies).