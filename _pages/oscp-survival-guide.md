---
title: "OSCP Survival Guide"
permalink: /oscp/
excerpt: "My humble version of an OSCP Survival Guide"
last_modified_at: 2020-07-31
sidebar:
  title: "OSCP Survival Guide"
  nav: oscp
toc: true
---

# General

* Set the target IP to a $ip system variable
```
export ip=10.10.1.0
```

* Start a service
```
systemctl start ssh
systemctl start apache2
```

* Have a service start at boot
```
systemctl enable ssh
```

* Stop a service
```
systemctl stop ssh
```

* Unzip a gz file  
```
gunzip file.gz
```

* Unzip a tar.gz file
```
tar -xzvf file.tar.gz
```


# String Manipulation

* Count number of lines in file
```
wc -l index.html
```


## Hashing & Password Cracking

[hashes.com: Identify hash types](https://hashes.com/en/tools/hash_identifier)  
[crackstation.net: Free Password Hash Cracker](https://crackstation.net/)

### Crypto

[CyberChef](https://gchq.github.io/CyberChef/)


#### Reverse Shells

[GTFOBins](https://gtfobins.github.io/)

