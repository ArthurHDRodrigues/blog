---
layout: post
title:  "My first contributions to Guix System"
date:   2025-05-17 14:08:20 +0000
categories: guix
---

## My first contributions to Guix System

Guix System is a fairly new GNU System or GNU/Linux distribution,
the pure GNU version ships with the [Hurd kernel](https://en.wikipedia.org/wiki/GNU_Hurd),
while the Linux version ships with [linux-libre](https://en.wikipedia.org/wiki/Linux-libre)
a linux fork with all of the binary blobs, obfuscated code and portions of code under proprietary licenses removed.

It is the GNU implementation of [the pure functional deployment model](https://edolstra.github.io/pubs/phd-thesis.pdf),
inaugurated by Nix and NixOS.

As I can see, Guix cares much more about reprodutibility than NixOS and it has a dedicated HPC team.
But since it is less mature, it is kind of rough around the edges, so I decided to contribute to it!

## First bug report

My first contact with the community was [this bug report](https://issues.guix.gnu.org/78274), 
which was quickly closed, because it was not considered a bug.

## First patch

Guix is, by default, a source based distribution, thus a package is actually a recipe to build a given software.
This recipes are stored in the folder `gnu/packages`.

My first [submitted patch](https://issues.guix.gnu.org/78393) proposed the addition of the Golang library [jwt](https://github.com/golang-jwt/jwt).
The recipe for Golang libraries are very simple, because no compilation is required, to install a Golang library, you just need to download its source files. 

Before sending the patch to the mailing list I checked the file `golang-xyz.scm`, that constains a lot of Golang libraries and didn't find jwt.
But after submitting it, a contributer pointed out that this project is already present using guix's [packages search tool webpage](https://packages.guix.gnu.org/packages/go-github-com-golang-jwt-jwt/3.2.2/).
This web page shows the location of the library as being `golang-crypto.scm`, a simple grep in guix's source code confirms that.
So my patch was not accepted.

## Current Contribution

Now I'm updating the Docker package, the current package is version [20.10.27](https://packages.guix.gnu.org/packages/docker/20.10.27/), which is two years old.
I will write another post about it later. 

## Future Contributions 

In the futere I also plan to add the package [act](https://github.com/nektos/act) and ghidra.
Also configure a default wallpaper for Gnome, currently there is no default wallpaper and a blank dark blue backgroud is the default behavior.
