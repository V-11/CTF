**JTAG Dump**
===================  
[Challenge Link](https://s3-eu-west-1.amazonaws.com/hubchallenges/Forensics/Jtag-dump.bin)  

> This is a JTAG mobile extraction for a handset in a criminal case.. Catch the flag.

The file was quite large so there should be copressed files.  
I used the command `binwalk -e Jtag-dump.bin` to extract all files.  
I got hundreds of other compressed/corrupted files and of course I would never analyze them all.  
I googled and found a similar extraction command on Stack Overflow which is `binwalk -D='.*' Jtag-dump.bin`.  
It took a lot of time to extract so I killed the process after few minutes.  
Going through the extracted pictures.. **9ABFF** has the flag.
