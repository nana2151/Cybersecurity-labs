# Bandit Level 19 → Level 20

## What I Had to Do  
This time, I had to run a **binary executable** that would only give me the next password if I ran it with the **correct argument** — my current password.

---

## How I Solved It  
Logged in with:

```bash
ssh bandit19@bandit.labs.overthewire.org -p 2220
```

Password used:
```
EeoULMCra2q0dSkYj561DX7s1CpBuOBt
```

Then I ran:

```bash
./bandit20-do cat /etc/bandit_pass/bandit20
```

---

## Password Found  
```
tRae0UfB9v0UzbCdn9cY0gQnds9GF58Q
```

---

## What I Learned  
I learned how to use a SUID program to act as another user (like `sudo`) and securely extract restricted data.
