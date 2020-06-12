**Binwalk**
-------------
[Challenge Link](https://mega.nz/#!qbpUTYiK!-deNdQJxsQS8bTSMxeUOtpEclCI-zpK7tbJiKV0tXYY)  

> Here is a file with another file hidden inside it, Can you extract it?

Let's check the file type.

![](images/binwalk.png)

We gotta change its extension.  
I extracted its compressed files using `binwalk -D='.*'`  
I got two pictures.. one of the had the flag.
