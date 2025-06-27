# Bandit Level 15 → Level 16

## What I Had to Do  
This time, the port I had to connect to required me to **provide the password and read a response** — a simple client/server communication.

---

## How I Solved It  
Logged in using:

```bash
ssh bandit15@bandit.labs.overthewire.org -p 2220 
```

Password used:
```
8xCjnmgoKbGLhHFAZlGE5Tmu4M2tK2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJDx
```

Used this command to connect and read:

```bash
openssl s_client -connect localhost:30001
# Then pasted the password when prompted
```

---

## Password Found  
```
x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO
```

---

## What I Learned  
Used `openssl s_client` to connect to SSL ports and interact with encrypted services.
