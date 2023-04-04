# money ware

**money-ware (PicoCTF 2023):**

**Team: The\_Dream\_Team (6100 points) (160th place global)**

**Description:**

Flag format: picoCTF{Malwarename}

The first letter of the malware name should be capitalized and the rest lowercase.

Your friend just got hacked and has been asked to pay some bitcoins to 1Mz7153HMuxXTuR2R1t78mGSdzaAtNbBWX. He doesn’t seem to understand what is going on and asks you for advice. Can you identify what malware he’s being a victim of?

There is the solution that I found for this flag:

Solution:

* Upon searching for the wallet address, the following article came up: [https://www.cnbc.com/2017/06/28/ransomware-cyberattack-petya-bitcoin-payment.html](https://www.cnbc.com/2017/06/28/ransomware-cyberattack-petya-bitcoin-payment.html)
* Looking at the beginning of the article, it mentions a malware on this Bitcoin address called “Petya”

![Command-Line](<../.gitbook/assets/0 (7).png>)

* Entering the flag format (picoCTF{Malwarename}) and inserting “Petya”, making it picoCTF{Petya}, gives us the flag!

![Command-Line](<../.gitbook/assets/1 (3).png>)
