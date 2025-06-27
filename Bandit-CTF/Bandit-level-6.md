# Bandit Level 6 → Level 7

## What I Had to Do  
In this level, the password was not stored in a file like before — it was hidden in a **running process** on the system, and my goal was to find and extract it from the command-line arguments of that process.

---

## How I Solved It  
First, I logged into the Bandit server using the password from Level 5:

```
ssh bandit6@bandit.labs.overthewire.org -p 2220
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
ps aux 
... /some/script --password=thepassword ...
```
Password Found
**morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj**


What I Learned
This level introduced me to inspecting running processes using ps aux. It taught me how sensitive information can sometimes be exposed in command-line arguments, which is a common real-world vulnerability.
