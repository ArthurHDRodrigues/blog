---
layout: post
title: "A compatibility layer from linux to redox"
date: 2025-03-02 15:02:35 +0300 
---

## Long story short

The basic idea is to develop a compatibility layer to run linux modules on redox-os.
It'd be something similar to [Wine](https://www.winehq.org/), but to be a layer between linux and redox-os.

The objective is to "port" all linux's device drivers to redox at once.

## The idea

I had this interesting idea some weeks ago and
I don't know if it is possible, so I'll write about it here and maybe some day work toward a proof of concept.

[Linux](https://en.wikipedia.org/wiki/Linux) is the most used kernel in the world and [Mars](https://www.fosslinux.com/45797/linux-lands-on-mars-a-victory-for-open-source.htm).
This popularity implies in (and is possible by) a large range of supported machines and thus in drivers implemented for linux.
Actually the majority of kernel code is device drivers.

But it is not the only open source OS out there.
[Redox-os](https://www.redox-os.org/) is a fairly new kernel/OS written in Rust that uses the microkernel architecture.
It'd be nice if redox-os supported as much hardware as linux, but it lacks the necessary drivers and of course
rewrite all linux's drivers is a massive task to implement and maintain.

Then I came up with an idea that I must point out again that I don't know if it is possible.
The idea is to develop a compatibility layer to run linux modules on redox-os.

This compability layer would provide a virtualized enviroment for linux modules to run in redox-os just as another userspace process.
It wouldn't be a virtual machine, because we are not virtualizing hardware.
It'd be something similar to [Wine](https://www.winehq.org/), but this layer would virtualize not only the linux's syscalls (as Wine implements the Windows syscalls), but also all other resources a module needs (such as global .

The problem is that I don't know which resources a linux module needs.
I presume that there should be some global variables and internal API that this layer needs to virtualize.

If this layer succeeds, it will port all linux's device drivers to redox-os at once with reduced maintenance cost, that is, instead of maintaining all drivers, we just maintain the compatibility layer.
