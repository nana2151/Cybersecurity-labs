# Bandit Level 16 → Level 17

## What I Had to Do  
This level required me to use an SSH private key to log in as **bandit17**, but instead of being given a password, I had to use the private key file found in the previous level.

---

## How I Solved It  
Logged in to Bandit 16 with:

```bash
ssh bandit16@bandit.labs.overthewire.org -p 2220
```

Password used:
```
x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO
```

Then I copied the RSA private key from the `key` file and saved it to `/tmp/bandit17.key`.

```bash
chmod 600 /tmp/bandit17.key
ssh -i /tmp/bandit17.key bandit17@localhost -p 2220
```

---

## Password Found  
```
cGWpMaKXVwDUNgPAVJbWYuGHVn9zl3j8
```

---

## What I Learned  
I learned how to log in to an SSH server using a private key instead of a password, and how to secure that key with proper permissions.
