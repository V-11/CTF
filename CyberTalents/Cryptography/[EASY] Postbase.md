**Postbase**
===================  
[Challenge Link](https://cybertalents.com/challenges/cryptography/postbase)  

> We got this letters and numbers and we don't understand them. Can you?  
> R[corrupted]BR3tCNDUzXzYxWDdZXzRSfQ==

This challenge got me thinking a lot.. A. L. O. T.

I tried to decode BR3tCNDUzXzYxWDdZXzRSfQ== but I could not get anything readable.. I know it's **Base64** but it needs the corrupted part to get decoded.

After a lot of googling and failed tries.. I got it.. How?  
I tried to encode **FLAG{**.. Guess what.. It's **RkxBR3s=** so the corrupted part is **kx** lol.. so clever.

I used [this site](http://www.utilities-online.info/base64/) to encode/decode.
