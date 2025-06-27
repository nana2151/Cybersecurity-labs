# Bandit Level 13 → Level 14

## What I Had to Do  
This level gave me a private SSH key which could be used to log into the next level.

---

## How I Solved It  
Logged in using:

```bash
ssh bandit13@bandit.labs.overthewire.org -p 2220
```

Password used:
```
FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn
```

I then copied the private key to `/tmp/mykey`, gave it the right permissions:

```bash
chmod 600 mykey
ssh -i mykey bandit14@localhost -p 2220
```

---

## Password Found  
```
MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS
```

---

## What I Learned  
Learned how to use an SSH private key securely and change its permission with `chmod 600`.
