Bandit Level 0 → Level 1
What I Had to Do
This was my first step into the Bandit CTF. The goal was simple: connect to the server using SSH and find a file in the home directory that contains the password for the next level.

How I Solved It
I started by opening my terminal and used the following command to connect to the Bandit server:

ssh bandit0@bandit.labs.overthewire.org -p 2220
It asked me for a password. I used the one given in the challenge description:

bandit0
Once logged in, I listed the contents of the directory using:

ls
I saw a file named readme. I used the cat command to read it:

cat readme
It displayed the password for the next level.

Password Found
ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
What I Learned
This level taught me how to connect to a remote machine using SSH, which is a critical skill in cybersecurity. I also got familiar with using basic Linux commands like ls and cat to navigate the system and read files.
