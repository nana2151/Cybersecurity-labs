# Bandit Level 8 → Level 9

## What I Had to Do  
In this level, the password was stored in a file but **encoded using Base64**. My task was to decode it.

---

## How I Solved It  
Logged in with:

```bash
ssh bandit8@bandit.labs.overthewire.org -p 2220
```

Password used:
```
dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc
```

Then I decoded the data using:

```bash
base64 -d data.txt
```

---

## Password Found  
```
4CKMh1JI91bUIZZPXDqGanal4xvAg0JM
```

Used to log in to **Bandit 9**.

---

## What I Learned  
Gained experience decoding Base64 — a common encoding scheme used in web and security contexts.
