---
title: "Packages"
date: 2022-09-03
---

## Synapse
![Matrix](/images/matrix.jpg)

I have a [simple fork](https://github.com/tommytran732/Synapse-Docker) of [Wonderfall's hardened Synapse Docker image](https://github.com/Wonderfall/docker-synapse) with the [Mjolnir module](https://github.com/matrix-org/mjolnir/blob/main/docs/synapse_module.md) support and the default (as opposed to light) variant of the [Hardened Memory Allocator](https://github.com/GrapheneOS/hardened_malloc).

You can obtain the image by pulling `ghcr.io/tommytran732/synapse`.

## pamac-flatpak AUR

![pamac](/images/pamac.png)

I maintain the [`pamac-flatpak`](https://aur.archlinux.org/packages/pamac-flatpak), [`pamac-flatpak-gnome`](https://aur.archlinux.org/packages/pamac-flatpak-gnome), and [`libpamac-flatpak`](https://aur.archlinux.org/packages/libpamac-flatpak) AUR packages. Originally, they were forks of [`pacmac-all`](https://aur.archlinux.org/packages/pamac-all) and [`libpamac-all`](https://aur.archlinux.org/packages/libpamac-nosnap) with snapd removed. I found snapd to be quite annoying - it is yet another AUR package I don't need, requires `cgroupsv1` for confinement, does not integrate with `gnome-software`, makes lots of loopback mounts, and so on.

Nowadays, they are based on the [`pamac-nosnap`](https://aur.archlinux.org/packages?O=0&K=pamac-nosnap) package with some minor changes to make the build and installation process nicer and more convenient.