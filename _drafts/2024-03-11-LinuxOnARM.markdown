---
layout: post
title: "Working with Linux in an ARM64 laptop"
date: 2024-03-11 18:51:00 +0300 
---


## Hardware information

## Relevant Link

- A quick search on YT shows [this video](https://www.youtube.com/watch?v=sMRur1pCW9Q), which show a Debian installed on our target hardware. The image used was from an experimental project called [imagebuilder](https://github.com/hexdump0815/imagebuilder/blob/main/systems/snapdragon_7c_woa/readme.md). Releases
  - [230308-01](https://github.com/hexdump0815/imagebuilder/releases/tag/230308-01)
  - [240107-01](https://github.com/hexdump0815/imagebuilder/releases/tag/240107-01)
supports our target machine. The author documents this experiments in this [README](https://github.com/hexdump0815/imagebuilder/blob/main/systems/snapdragon_7c_woa/readme.md) and this [issue](https://github.com/hexdump0815/imagebuilder/issues/136).
- [armbian](https://www.armbian.com/).  [this post](https://forum.armbian.com/topic/24464-samsung-go-book/#comment-153460) links to our next point of interest.
-  [aarch64-laptops](https://github.com/aarch64-laptops/debian-cdimage/releases):The repository contains the Debian CD image releases for AArch64 Laptops. In particular issue [#21](https://github.com/aarch64-laptops/debian-cdimage/issues/21#) relates to Samsung Book Go.
-  amcduffee's [fork of linux](https://github.com/amcduffee/linux/tree/galaxy-book-go) contains a partial device tree of target machine.

## Official Debian Links
- [Debian port page](https://www.debian.org/ports/arm/)
- [Debian cdimage repository (weekly build)](https://cdimage.debian.org/cdimage/weekly-builds/arm64/iso-cd/)
- [Debian cdimage repository (rrelease)](https://cdimage.debian.org/cdimage/current/arm64/iso-cd/)
- [Debian ARM email list](https://lists.debian.org/debian-arm/), but it doesn't seem to reference Samsung Book Go.


## Misc Links

- [Diolinux forum](https://plus.diolinux.com.br/t/instalacao-do-linux-no-notebook-samsung-galaxy-book-go/46864)


## Testing candidates
The following is a list of possibles canditates and my notes about testing them

### debian-cdimage Release 0.4
- Source: [Github Release page](https://github.com/aarch64-laptops/debian-cdimage/releases/tag/v0.4)
#### Installing
#### Reproducing

### imagebuilder Release 230308-01
- Source: [Github Release page](https://github.com/hexdump0815/imagebuilder/releases/tag/230308-01)
#### Installing
#### Reproducing

### imagebuilder Release 240107-01
- Source: [Github Release page](https://github.com/hexdump0815/imagebuilder/releases/tag/240107-01)
#### Installing
#### Reproducing

## Build tools
This tools don't necessary support the target, but are well established.

### debos
- Source: [Github Source page](https://github.com/go-debos/debos)
#### Building
#### Testing

### buildroot
- Source: [Github Source page](https://github.com/go-debos/debos)
#### Building
#### Testing

### meta-debian
- Source: [Github Source page](https://github.com/meta-debian/meta-debian)
### Building
### Testing




