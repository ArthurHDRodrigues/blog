---
layout: post
title: "A compatibility layer from linux to redox"
date: 2025-03-02 15:02:35 +0300 
---

## Long story short

The basic idea is to develop a compatibility layer to run linux modules on redox-os.
It'd be something similar to [Wine](https://www.winehq.org/), but to be a layer between linux and redox-os.

The objective is to "port" all device drivers to redox at once.

## Introduction

[Linux](https://en.wikipedia.org/wiki/Linux) is the most used kernel used in the world and [Mars](https://www.fosslinux.com/45797/linux-lands-on-mars-a-victory-for-open-source.htm).
This popularity implies in a large range of supported machines and thus in drivers implemented for linux.
Actually the majority of kernel code is device drivers.

[Redox-os](https://www.redox-os.org/) is a fairly new kernel/OS, so it lacks drivers.
Write drivers for all hardware supported by linux is a massive task to implement and maintain.

Since this task is herculean, we need to think about another solution.
The idea is to develop a compatibility layer to run linux modules on redox-os.

It'd be something similar to [Wine](https://www.winehq.org/), but not exactly equal.
Wine implements the Windows syscalls.
It'd be a relative small binary that virtualize an enviroment to run 

## Goal

Port all linux's device drivers to redox at once.

## Initial stuff to do

* Compile redox.
* Write a redox module.

## How I got this idea

* Minimize linux size
* Refactor linux as a microkernel
* write a compatibility layer for that
* notice that a compatibility layer from linux to linux doesn't make sense.
* get another kernel to be target of the translation layer.
* choose redox since it seems a nice os and fits the current friction in the rust for linux project.
