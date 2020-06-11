**X-File**
===================  
[Challenge Link](https://hubchallenges.s3-eu-west-1.amazonaws.com/Forensics/dump.txt)  

> Someone is hiding a secret in this file.. Can you help me to recover the flag from the secret?   

We got some hexdump.. I used this [site](http://tomeko.net/online_tools/hex_to_file.php?lang=en) to convert it to file.  
After downloading the output I couldn't extract it because it was password protected.  
You can use [John the Ripper](https://www.openwall.com/john/) or this [site](https://www.lostmypass.com/file-types/zip/) to crack the password then you would get the flag.
