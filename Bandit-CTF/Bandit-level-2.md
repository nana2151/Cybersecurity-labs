What I Had to Do
This level asked me to find a file called spaces in this filename that contains the password for the next level. The challenge was dealing with spaces in filenames using the terminal.

How I Solved It
I connected to the Bandit server using the credentials from Level 2:

ssh bandit2@bandit.labs.overthewire.org -p 2220
Password used:
**263JGJPfgU6LtdEvgfWU1XP5yac29mFx**
Once inside, I listed the files:

ls
There was a file named:

spaces in this filename
To read it, I had to use quotes or escape the spaces. Either of the following worked:

cat "spaces in this filename"
or
cat spaces\ in\ this\ filename
**MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx**
What I Learned
I learned how to handle file names that contain spaces using quotes or escape characters. This is a common thing in Linux, and knowing how to deal with special characters makes working in the terminal smoother
