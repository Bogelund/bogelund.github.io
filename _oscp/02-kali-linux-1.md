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

## find Commands

| What                                              | Example                                                  |
|---------------------------------------------------|----------------------------------------------------------|
| Find files based on filename                      | find /home/Andy -type f -name sales.txt                  |
| Find Directory based on directory name            | find /home/Andy -type d -name pictures                   |
| Find files based on size                          | find /home/Andy -type f -size 10c<br>(c for bytes, k for kilobytes, M megabytes, G for gigabytes) |
| Find files based on username                      | find /etc/server -type f -user john                      |
| Find files based on group name                    | find /etc/server -type f -group teamstar                 |
| Find files modified after a specific date         | find / -type f -newermt '6/30/2020 0:00:00'              |
| Find files based on date modified                 | find / -type f -newermt 2013-09-12 ! -newermt 2013-09-14 |
| Find files based on date accessed                 | find / -type f -newerat 2017-09-12 ! -newerat 2017-09-14 |
| Find files with a specific keyword                | grep -iRl '/folderA/flag'                                |
| Find files with a specific pattern (ex. IP)       | <code>cat * \| grep -Eo "([0-9]{1,3}[\.]){3}[0-9]{1,3}"</code>        |
| read the manual for the find command              | man find                                                 |
