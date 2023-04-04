# chrono

**chrono (PicoCTF 2023):**

**Team: The\_Dream\_Team (6100 points) (160th place global)**

**Description:**

How to automate tasks to run at intervals on linux servers?

Solution 1 (The way you were supposed to do the challenge):

* Looking at the challenge hint, I figured out that it is hinting towards cron tasks, stored in the /etc/crontabs file. I used cat /etc/crontab/ to find the flag now.

![Command-Line](<../.gitbook/assets/0 (3).png>)

Solution 2 (The unintended but easier way):

* I first did ls to find any files currently in my directory.

![Command-Line](<../.gitbook/assets/1 (5).png>)

* Seeing nothing, I tried to cd .. 2 times, eventually ending up at the base directory. Seeing a challenge directory, I ended up doing cd into the directory to find any files. There is a metadata.json file here, as seen.

<figure><img src="../.gitbook/assets/3 (2).png" alt=""><figcaption><p>Command-Line</p></figcaption></figure>

* Seeing a metadata.json file, I did cat metadata.json to view what was inside of the file. Here was the flag:
