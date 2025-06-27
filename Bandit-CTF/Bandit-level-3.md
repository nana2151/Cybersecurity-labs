What I Had to Do
In this level, I had to find a hidden file inside a directory. The hint was that the file was stored invisible to standard tools, so I knew it might be a hidden file or inside a hidden directory.

How I Solved It
First, I connected using SSH with the credentials from Level 3:

ssh bandit3@bandit.labs.overthewire.org -p 2220
Password used:

**MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx**
Once logged in, I listed the contents of the directory:

ls
I saw a folder named **inhere**. I moved into it:

cd inhere
Running ls showed nothing. So I tried:

ls -a
This showed a hidden file:

.hidden
I used the cat command to read it:

cat .hidden
Password Found
**2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ**

What I Learned
This level helped me understand how to work with hidden files and directories in Linux using ls -a. Knowing how to find hidden files is important in cybersecurity, especially during forensic investigations or CTFs.
