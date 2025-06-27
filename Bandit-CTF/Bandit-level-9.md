# Bandit Level 9 → Level 10

## What I Had to Do  
The file in this level was a **hex dump**. I needed to convert it back to raw text and extract the password.

---

## How I Solved It  
Logged in using:

```bash
ssh bandit9@bandit.labs.overthewire.org -p 2220
```

Password used:
```
4CKMh1JI91bUIZZPXDqGanal4xvAg0JM
```

Used `xxd` and `strings`:

```bash
xxd -r data.txt decoded.txt
strings decoded.txt
```

---

## Password Found  
```
FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
```

Used to log in to **Bandit 10**.

---

## What I Learned  
Learned to reverse hex-dumped files using `xxd -r` and extract plain text using `strings`.
