# Bandit Level 14 → Level 15

## What I Had to Do  
The password for the next level had to be submitted to a port via `netcat`.

---

## How I Solved It  
Logged in using:

```bash
ssh bandit14@bandit.labs.overthewire.org -p 2220
```

Password used:
```
MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS
```

Then used `nc` to send the password to the port:

```bash
echo MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS | nc localhost 30000
```

---

## Password Found  
```
8xCjnmgoKbGLhHFAZlGE5Tmu4M2tK2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJDx
```

---

## What I Learned  
Practiced using `netcat (nc)` to send and receive data from a specific port — a common CTF and pentesting technique.
