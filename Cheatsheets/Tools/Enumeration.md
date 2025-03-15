# Nmap

Basic nmap scan:

nmap -vv -sC -sV -oN nmap.log $IP

Complete nmap scan:

nmap -vv -A -p- -oN nmap-complete.log $IP

See my nmap cheatsheet for other personal favorites.

# Web Directory and Query Parameters Bruteforce

Using gobuster:

gobuster dir -w /usr/share/dirbuster/wordlists/directory-list-2.3-medium.txt -o gobuster.log -t 200 -u $URL

Using wfuzz:

wfuzz -w /usr/share/dirbuster/wordlists/directory-list-2.3-medium.txt -t 200 --hc 404 http://www.host.name/FUZZ

Using wfuzz to bruteforce query parameters:

wfuzz -c -w /usr/share/dirbuster/wordlists/directory-list-2.3-medium.txt -t 200 --hc 404 http://www.host.name/?parameter=FUZZ

Recursive directory scan with wfuzz:

wfuzz -c -w /usr/share/dirbuster/wordlists/directory-list-2.3-small.txt -t 200 --hc 404 -R $DEPTH http://www.host.name/FUZZ