# Vagrant Boxes - Rocky Linux

## Overview

This repository contains Packer templates for creating Rocky Linux Vagrant boxes.

## Current Boxes

- [Rocky Linux](https://rockylinux.org/download/)

## Building the Vagrant boxes with Packer

To build all the boxes, you will need installed requires the software listed below.  

- VMware
  - [Fusion](https://www.vmware.com/products/fusion)
  - [Workstation](https://www.vmware.com/products/workstation)

We make use of JSON files containing user variables to build specific version of Ubuntu.  
You tell `packer` to use a specific user variable file via the `-var-file=` command line option.  

For example, to build on VMware Platform, use the following:

```bash
# rocky linux on VMware
$ FEDORA_VERSION=8.3 make build
```
