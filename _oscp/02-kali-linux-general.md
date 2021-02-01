---
title: "OSCP Survival Guide"
permalink: /oscp/kali-linux-general/
excerpt: "My humble version of an OSCP Survival Guide"
last_modified_at: 2020-07-31
sidebar:
  title: "OSCP Survival Guide"
  nav: oscp
toc: true
---

# Hello World from 02-kali-linux-general

# General

* Set the target IP to a `$ip` system variable\
`export ip=10.10.1.0`

* Start a service\
`systemctl start ssh`

* Have a service start at boot\
`systemctl enable ssh`

* Stop a service\
`systemctl stop ssh`

* Unzip a gz file\
`gunzip file.gz`

* Unzip a tar.gz file\
`tar -xzvf file.tar.gz`

# String Manipulation

* Count number of lines in file\
`wc -l index.html`
