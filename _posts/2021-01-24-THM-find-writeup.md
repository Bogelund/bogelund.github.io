---
title: "THM writeup - The find command"
date: 2021-01-23T10:00:00+02:00
categories:
  - blog
tags:
  - find
  - writeup
  - THM
---

>Thanks to tryhackme.com for creating such an amazing platform for the cyber security community

![](/assets/images/2021-01-24-13-28-56.png)

[This is a writeup for the find room](https://tryhackme.com/room/thefindcommand)

### Task 01: Start finding

No questions here

### Task 02: Be more specific

Find all files whose name ends with ".xml"

```
find / -type f -name "*.xml"
```


Find all files in the /home directory (recursive) whose name is "user.txt" (case insensitive)

```
find /home -type f -iname user.txt
```

Find all directories whose name contains the word "exploits"

```
find / -type d -name *exploits*
```


### Task 03: Know exactly what you're looking for

