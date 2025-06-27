# Bandit Level 17 → Level 18

## What I Had to Do  
In this level, I had to create a file named **`~/passwords/new_password`** containing the current password, and set the permissions so that **only the owner can read and write**.

---

## How I Solved It  
Logged in with:

```bash
ssh bandit17@bandit.labs.overthewire.org -p 2220
```

Password used:
```
cGWpMaKXVwDUNgPAVJbWYuGHVn9zl3j8
```

Commands used:

```bash
mkdir -p ~/passwords
echo cGWpMaKXVwDUNgPAVJbWYuGHVn9zl3j8 > ~/passwords/new_password
chmod 600 ~/passwords/new_password
```

After that, the system automatically validated the challenge.

---

## Password Found  
```
0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO
```

---

## What I Learned  
Learned how to create and set strict file permissions using `chmod`, which is crucial for securely managing sensitive data.
