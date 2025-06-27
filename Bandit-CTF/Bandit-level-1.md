What I Had to Do
In this level, the goal was to find a password that’s stored in a file called - (a single dash). The challenge here was that the filename could be confused with a command-line option, so I had to figure out how to read it correctly.

How I Solved It
I connected to the server the same way as before, but this time with the credentials for Level 1:

ssh bandit1@bandit.labs.overthewire.org -p 2220
It asked for a password, and I used the one I got from Level 0:

ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
After logging in, I ran:
ls
I saw a file named -, which I knew might be tricky because the dash is often used for command-line options. If I just typed cat -, it would wait for input from the terminal instead of reading the file.

To get around that, I used either of these two options:
cat ./-
or
cat -- -
Both worked. They told the terminal to treat - as a filename instead of an option.

Password Found
263JGJPfgU6LtdEvgfWU1XP5yac29mFx
What I Learned
This level taught me how file names that look like command-line options can be handled properly using special syntax. I also learned about --, which signals the end of options in many Unix tools — something that will definitely be useful in future levels.
