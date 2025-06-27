# Bandit Level 4 → Level 5

## What I Had to Do  
In this level, the goal was to find a file in the `inhere` directory that matched specific conditions:  
- Human-readable  
- 1033 bytes in size  
- Not executable  
- Located somewhere inside `inhere`

## How I Solved It  
I first logged in using the password I found in Level 3:

```
ssh bandit4@bandit.labs.overthewire.org -p 2220
2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
cd inhere
find . -type f -size 1033c ! -executable -exec file {} \; | grep "ASCII text"
cat ./-file07
```
Password Found
**4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw**

What I Learned
I learned how to:
Use the find command with size, type, and permission filters
Chain find with file and grep to inspect content types
Filter only readable files and ignore permission denied errors
This was a great intro to practical Linux file searching.
