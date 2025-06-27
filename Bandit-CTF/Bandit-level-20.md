# Bandit Level 20 → Level 21

## What I Had to Do  
I needed to communicate with a program running on `localhost` at a certain port, sending the password and reading the response.

---

## How I Solved It  
Logged in with:

```bash
ssh bandit20@bandit.labs.overthewire.org -p 2220
```

Password used:
```
tRae0UfB9v0UzbCdn9cY0gQnds9GF58Q
```

I created a simple script that connected and handled the challenge:

```bash
./suconnect 12345
```

Then followed any prompts to enter the password.

---

## Password Found  
```
0Zf11ioIjMVN551jX3CmStKLYqjk54Ga
```

---

## What I Learned  
Practiced basic client-server interaction on the same host using a local port and authentication challenge.
