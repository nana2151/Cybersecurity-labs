# Bandit Level 10 → Level 11

## What I Had to Do  
The password was stored in a text file, but **obfuscated using ROT13** — a simple letter substitution cipher.

---

## How I Solved It  
Logged in with:

```bash
ssh bandit10@bandit.labs.overthewire.org -p 2220
```

Password used:
```
FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
```

Decoded with:

```bash
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```

---

## Password Found  
```
dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr
```

Used to log in to **Bandit 11**.

---

## What I Learned  
Practiced using `tr` to decode a simple substitution cipher (ROT13). It’s a foundational concept in CTFs and text obfuscation.
