# Bandit Level 5 → Level 6

## What I Had to Do  
This time, I needed to search the entire filesystem (`/`) for a file that met **three specific conditions**:
- Owned by user `bandit6`
- Owned by group `bandit6`
- Exactly 33 bytes in size

---

## How I Solved It  
I first logged in using the password I found from Level 4:

```
ssh bandit5@bandit.labs.overthewire.org -p 2220
4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
find / -user bandit6 -group bandit6 -size 33c 2>/dev/null
cat /path/to/found/file

```
 Password found 
**HWasnPhtq9AVKe0dmk45nxy20cvUa6EG**

What I Learned
This level helped reinforce my knowledge of the find command, especially:
-How to search by owner and group
-How to filter by exact file size
-How to suppress errors using 2>/dev/null

It’s a skill that’s extremely useful when analyzing file systems.
