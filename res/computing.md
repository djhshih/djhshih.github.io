---
layout: single
title: Computing
permalink: /res/computing/
---

## Background

While R and Python can be used with any operating system (OS), data
pre-processing and bioinformatic analyses are most efficiently done in
the Linux environment due to availability of software tools and offerings
by high performance computing centers.
Therefore, familiarity with the Linux environment is critical for
research projects in our lab.

### Linux

There are a myriad of other Linux variants (i.e. distributions).
They fall into three main families:

1. Red Hat, CentOS Stream, Fedora)
2. Debian, Ubuntu
3. Arch Linux

Most computing servers run a variants of Linux known as
CentOS (versions 7 or 8), which is the community version of Red Hat Enterprise Linux.
The latter is often used in risk-adverse enterprise environments.
Starting in 2021, CentOS is being replaced with CentOS Stream, which removes
minor versioning. Research organizations such as CERN has adopted CentOS Stream.

Ubuntu and its derivative distributions likely have the best hardware driver support
for laptops.

Arch Linux is a lightweight distributions that embraces a rolling-release model,
under which packages cannot be upgraded individually. Rather, software packages
are continuously released and the distribution mirrors only keep the latest
releases. This simplifies package management and dependency.
I personally prefer this distribution, but it may not be the best choice
for beginners.

There is another Linux distribution that provides reproducible compilation of 
different versions of software tools: NixOS. Its package manager, Nix, can
also be run on other Linux distributions.

### MacOS

MacOS is based on BSD Unix. While it has some similiarties to Linux, it has
many important differences. For example, Linux `coreutils` provide basic command
line tools such as `find` and `grep` that are very different from the tools
provided by MacOS. Bash scripts written for Linux may not work on MacOS.

With Apple's switch from x86 to arm64 CPUs in their latest Macbooks, users will
experience installation or runtime issues with software tools that do
not support arm64, including many R Bioconductor packages.

Given these limitations, MacOS is not an ideal substitute for Linux in 
bioinformatic research projects.

### Recommendation

Beginner Linux users should setup a Fedora virtual machine on their computers using
[Virtual Box](https://www.virtualbox.org/wiki/Downloads).
This would allow users to learn software tools and develop code on their Fedora
virtual machine and transition as seamlessly as possible to server
environments based on CentOS.

Experienced Linux users can consider setting up dual-boot computers or
dedicated computers running Fedora, Arch Linux, or NixOS.

