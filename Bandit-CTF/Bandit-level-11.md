# Bandit Level 11 → Level 12

## What I Had to Do  
The password was stored in a file that had been compressed multiple times using different formats (gzip, bzip2, tar, etc.). My job was to **unpack it step by step** until I reached the plain text file.

---

## How I Solved It  
Logged in using:

```bash
ssh bandit11@bandit.labs.overthewire.org -p 2220
```

Password used:
```
dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr
```

I copied `data.tar` to `/tmp`, and then used a series of commands:

```bash
cp data.tar /tmp
cd /tmp
file data.tar
# Extract based on file type, e.g.:
tar -xf data.tar
# then keep checking and decompressing: gzip -d, bzip2 -d, etc.
```

Repeated this process until I could finally `cat` the final file.

---

## Password Found  
```
7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4
```

---

## What I Learned  
Learned how to identify and extract nested archive formats using `file`, `tar`, `gzip`, and `bzip2`.
