# Bandit Level 7 → Level 8

## What I Had to Do  
This level asked me to find a file containing the password, but there was a twist — the file was hidden among many others, and only one of them was **human-readable** and **different**.

---

## How I Solved It  
I logged in using:

```bash
ssh bandit7@bandit.labs.overthewire.org -p 2220
```

Password used:
```
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
```

I listed the files using:

```bash
ls -l
```

Among the files, I looked for one with a smaller size or different permissions, and then used `cat` to open it:

```bash
cat <filename>
```

---

## Password Found  
```
dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc
```

Used to login to **Bandit 8**.

---

## What I Learned  
I practiced spotting outliers in a group of similar files and reviewing their metadata using `ls -l`.
