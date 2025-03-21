---
type: {notes/writeup}
tags: [{PLATFORM NAME/CTF NAME}, {box/challenge}, {linux/win}, {easy/medium/hard}, {services}, {cve-number}, {tooling}, {techniques}]
reference: {URL}
category: {blackbox/web/rev-engineering/rooting/coding/hardware/blockchain/misc/steg/etc}
title: "{BOX NAME}"
difficulty: {easy, medium, hard}
user-voted: {easy, medium, hard}
date: {YYYY-MM-DD}
author: {AUTHOR NAME}
contact: {AUTHOR CONTACT}
---

# Lookup

Target IP = 10.10.155.203
Tun0 IP = 10.6.15.244

---

## Information Gathering

### Open Ports & Running Services

```sh
PORT   STATE SERVICE VERSION
22/tcp open  ssh     OpenSSH 8.2p1 Ubuntu 4ubuntu0.9 (Ubuntu Linux; protocol 2.0)
| ssh-hostkey: 
|   3072 44:5f:26:67:4b:4a:91:9b:59:7a:95:59:c8:4c:2e:04 (RSA)
|   256 0a:4b:b9:b1:77:d2:48:79:fc:2f:8a:3d:64:3a:ad:94 (ECDSA)
|_  256 d3:3b:97:ea:54:bc:41:4d:03:39:f6:8f:ad:b6:a0:fb (ED25519)
80/tcp open  http    Apache httpd 2.4.41 ((Ubuntu))
|_http-title: Did not follow redirect to http://lookup.thm
|_http-server-header: Apache/2.4.41 (Ubuntu)
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

```


```

```
**OS:** linux 

---

## Exploitation

### {PORT } - {SERVICE NAME}

### {Step#}

Tooling: {TOOL NAME}
Description: {GOALS}

```sh
{COMMAND}


```

{SCREENSHOTS}

---

### {Step#}

Tooling: {TOOL NAME}
Description: {GOALS}

```sh
{COMMAND}

```

{SCREENSHOTS}

---

> [!USER FLAG]
> {USER FLAG}

{SCREENSHOT}

---

## Privilege Escalation

### {Step#}

Tooling: {TOOL NAME}
Description: {GOALS}

```sh
{COMMAND}

```

{SCREENSHOTS}

---

### {Step#}

Tooling: {TOOL NAME}
Description: {GOALS}

```sh
{COMMAND}

```

{SCREENSHOTS}

---

> [!ROOT FLAG]  
> {ROOT FLAG}  

{SCREENSHOT}

---

## SUCCESS

---

### Conclusion

{SCREENSHOT FINAL SCREEN}

---

## TODO

[ ] Share on Twitter  
[ ] Revise notes + Links to Notebook  
[ ] Export to HTML  
[ ] Publish on Medium  
[ ] Convert to PDF  
[ ] Push on GitHub  