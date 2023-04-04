# useless

**useless (PicoCTF 2023):**

**Team: The\_Dream\_Team (6100 points) (160th place global)**

**Description:**

There's an interesting script in the user's home directory

The work computer is running SSH. We've been given a script which performs some basic calculations, explore the script and find a flag.

Solution:

SSHing into the server, we see a script name “useless” in the user’s home directory. We can try running the file using ./useless .

![Command-Line](<../.gitbook/assets/0 (2).png>)

Now we read the code using cat useless , and find something very interesting. The code tells us to read the manual of the game. There is a command named man which gives us the manual of a code, and we run man useless this to get the flag after a few enter presses.

![Command-Line](<../.gitbook/assets/1 (1).png>)
