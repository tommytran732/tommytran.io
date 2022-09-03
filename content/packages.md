---
title: "Packages"
date: 2022-09-03
---

## pamac-flatpak AUR

![pamac](/images/pamac.png)

I maintain the [pamac-flatpak](https://aur.archlinux.org/packages/pamac-flatpak), [pamac-flatpak-gnome](https://aur.archlinux.org/packages/pamac-flatpak-gnome), and [libpamac-flatpak](https://aur.archlinux.org/packages/libpamac-flatpak) AUR packages. Originally, they were forks of the [pacmac-all](https://aur.archlinux.org/packages/pamac-all) and [libpamac-all](https://aur.archlinux.org/packages/libpamac-nosnap) AUR packages with snapd removed. I found snapd to be quite annoying - it is yet another AUR package I don't need, requires cgroupsv1 for confinement, does not integrate with `gnome-software`, makes lots of loopback mounts, and so on.

Nowadays they are based on the [pamac-nosnap](https://aur.archlinux.org/packages?O=0&K=pamac-nosnap) package with some minor changes to make the build and installation process nicer and be more convenient.