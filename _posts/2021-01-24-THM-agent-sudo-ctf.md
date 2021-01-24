---
title: "THM writeup - Agent Sudo"
date: 2021-01-24T14:00:00+02:00
categories:
  - THM Writeups
tags:
  - sudo
  - writeup
  - THM
---

Agent Sudo is a relatively easy and beginner friendly room. To complete this room we need to do some enumration, hash cracking, steganography, and privilege escalation. It going to bwe a lot of fun, so let's get started.

>Thanks to tryhackme.com for creating such an amazing platform for the cyber security community

![](/assets/images/2021-01-24-14-54-28.png)

Always - let's start out with having nmap doing a port scan

![](/assets/images/2021-01-24-15-16-20.png)


When port 80 is open it is always a good thing to start with inspecting the website

![](/assets/images/2021-01-24-15-38-06.png)

After we modified the User-Agent with **C** and forwarded the request, we got an interessting response.

![](/assets/images/2021-01-24-15-55-01.png)

### Task 2: Enumerate

Enumerate the machine and get all the important information

```
3
```

How you redirect yourself to a secret page?

```
???
```

What is the agent name?

```
???
```

