---
title: "THM writeup - Agent Sudo"
date: 2021-01-24T14:00:00+02:00
categories:
  - blog
tags:
  - sudo
  - writeup
  - THM
---

Agent Sudo is a relatively easy and beginner friendly room. To complete this room we need to do some enumeration, hash cracking, steganography, and privilege escalation. It going to bwe a lot of fun, so let's get started.

>Thanks to tryhackme.com for creating such an amazing platform for the cyber security community

{% include figure image_path="/assets/images/2021-01-24-14-54-28.png" alt="" caption="" %}

Always - let's start out with having nmap doing a port scan

{% include figure image_path="/assets/images/2021-01-24-15-16-20.png" alt="" caption="" %}

When port 80 is open it is always a good thing to start with inspecting the website

![](/assets/images/2021-01-24-15-38-06.png)

After we modified the User-Agent with **C** and forwarded the request, we got an interessting response.

![](/assets/images/2021-01-24-15-55-01.png)

In the browser

![](/assets/images/2021-01-24-16-04-05.png)

### Task 2: Enumerate

Enumerate the machine and get all the important information
>3

How you redirect yourself to a secret page?
>User-Agent

What is the agent name?
>chris

Now it's time to do some brute forcing. We have port 21 open, and our user is **chris*

```
hydra -l chris -P /usr/share/wordlists/rockyou.txt ftp://10.10.159.16
```

after a few minutes we get the password for chris - which is __crystal__

![](/assets/images/2021-01-24-16-15-09.png)


### Task 2: Hash cracking and brute-force

FTP password
>crystal

Zip file password
>???

steg password
>???