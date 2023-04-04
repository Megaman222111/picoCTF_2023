# Special

**Special (PicoCTF 2023):**

**Team: The\_Dream\_Team (6100 points) (160th place global)**

**Description:**

Don't power users get tired of making spelling mistakes in the shell? Not anymore! Enter Special, the Spell Checked Interface for Affecting Linux. Now, every word is properly spelled and capitalized... automatically and behind-the-scenes! Be the first to test Special in beta, and feel free to tell us all about how Special streamlines every development process that you face. When your co-workers see your amazing shell interface, just tell them: That's Special (TM)

Start your instance to see connection details.

Solution:

SSHing into the server, we see that no normal commands will work such as, ls, cat, and more. These get autocorrected.

![Command-Line](<../.gitbook/assets/0 (4).png>)

Looking a bit deeper into the question, we can see that it is possible to run files or commands using their full path. Going on Google to see the apth of the ls command, we find out that ls is located in ‘/usr/bin/ls’ and cat is located in ‘/usr/bin/cat’. We try running these and we realize that they work.

![Command-Line](<../.gitbook/assets/1 (2).png>)

Using ls, we see that there is a directory called ‘blargh’. We try to mention this as an argument for the ls command.

![Command-Line](<../.gitbook/assets/2 (1).png>)

BINGO! We see a flag.txt file, and now we can use cat to read the flag.txt file in the ‘blargh’ directory.

![Command-Line](<../.gitbook/assets/3 (1).png>)
