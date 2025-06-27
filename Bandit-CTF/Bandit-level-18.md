# Bandit Level 18 → Level 19

## What I Had to Do  
This level was unique — I had to **log out immediately after logging in** to trigger the retrieval of the next password from a script.

---

## How I Solved It  
Logged in with:

```bash
ssh bandit18@bandit.labs.overthewire.org -p 2220
```

Password used:
```
0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO
```

Then I immediately logged out:

```bash
exit
```

After logging out, the password was printed in the shell.

---

## Password Found  
```
EeoULMCra2q0dSkYj561DX7s1CpBuOBt
```

---

## What I Learned  
This level taught me how `.bashrc` and `.bash_logout` can be used to trigger scripts on login/logout — useful in security monitoring and traps.
