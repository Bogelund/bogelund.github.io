---
title: "Kali Linux - General Commands"
permalink: /oscp/kali-linux-1/
excerpt: "My humble version of an OSCP Survival Guide"
last_modified_at: 2020-02-01
toc: true
---

## General

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

## String Manipulation

* Count number of lines in file\
`wc -l index.html`