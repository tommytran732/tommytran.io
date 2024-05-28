---
title: "Packages"
date: 2022-09-03
---

## Synapse
![Matrix](/images/matrix.jpg)

I have a [simple fork](https://github.com/tommytran732/Synapse-Docker) of [Wonderfall's hardened Synapse Docker image](https://github.com/Wonderfall/docker-synapse) with the [Mjolnir module](https://github.com/matrix-org/mjolnir/blob/main/docs/synapse_module.md) support and the default (as opposed to light) variant of the [Hardened Memory Allocator](https://github.com/GrapheneOS/hardened_malloc).

You can obtain the image by pulling `ghcr.io/tommytran732/synapse` or `quay.io/tommytran732/synapse`.

## Matrix.to

I made an Alpine Docker container for [Matrix.to](https://matrix.to) that you obtain by pulling `ghcr.io/tommytran732/matrix.to`. The default instance has been changed from [Element.io](https://app.element.io) to [ArcticFoxes.net](https://element.arcticfoxes.net).