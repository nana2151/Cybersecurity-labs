# Bandit Level 12 → Level 13

## What I Had to Do  
The password was stored in a **hexdump** format and needed to be converted back to binary before being read.

---

## How I Solved It  
Logged in using:

```bash
ssh bandit12@bandit.labs.overthewire.org -p 2220
```

Password used:
```
7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4
```

To reverse the hex dump:

```bash
xxd -r data data.raw
cat data.raw
```

---

## Password Found  
```
FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn
```

---

## What I Learned  
How to reverse a hex-dump using `xxd -r` and work with raw binary data.
