---
layout: post
title: "Working with Linux in an ARM64 laptop"
date: 2024-03-11 18:51:00 +0300 
---


## Info de hardware

## Relevant Link

- A quick search on YT shows [this video](https://www.youtube.com/watch?v=sMRur1pCW9Q), which show a Debian installed on our target hardware. The image used was from an experimental project called [imagebuilder](https://github.com/hexdump0815/imagebuilder/blob/main/systems/snapdragon_7c_woa/readme.md). The release [230308-01](https://github.com/hexdump0815/imagebuilder/releases/tag/230308-01) supports our target machine.
- [armbian](https://www.armbian.com/).  [this post](https://forum.armbian.com/topic/24464-samsung-go-book/#comment-153460) links to our next point of interest.
-  [aarch64-laptops](https://github.com/aarch64-laptops/debian-cdimage/releases):The repository contains the Debian CD image releases for AArch64 Laptops. In particular issue [#21](https://github.com/aarch64-laptops/debian-cdimage/issues/21#) relates to Samsung Book Go.

## Official Debian Links
- [Debian port page](https://www.debian.org/ports/arm/)
- [Debian cdimage repository (weekly build)](https://cdimage.debian.org/cdimage/weekly-builds/arm64/iso-cd/)
- [Debian cdimage repository (rrelease)](https://cdimage.debian.org/cdimage/current/arm64/iso-cd/)
- [Debian ARM email list](https://lists.debian.org/debian-arm/), but it doesn't seem to reference Samsung Book Go.


## Misc Links

- [Diolinux forum](https://plus.diolinux.com.br/t/instalacao-do-linux-no-notebook-samsung-galaxy-book-go/46864)
