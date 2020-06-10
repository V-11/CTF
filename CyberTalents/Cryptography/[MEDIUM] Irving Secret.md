**Irving Secret**
===================  
[Challenge Link](https://hubchallenges.s3-eu-west-1.amazonaws.com/Forensics/secret.pcapng)  

> Irving asks Tyrell to send the secret encoded by ROT13.. Can you find that secret?  
> Format: flag{md5(secret)}

I got a pcap-ng capture file.. I opened it with [Wireshark](https://www.wireshark.org/).  
I got very few packets using TCP protocol.. I followed the stream.. `Ctrl+Alt+Shift+T`.  
I got an extremely long string.. Since the description said it was encoded using ROT13.. I used this [site](https://rot13.com/) to decrypt it.  
I didn't know what to do with the output.. after some googling I thought of converting it to file.. I used this [site](http://tomeko.net/online_tools/hex_to_file.php?lang=en).  
It worked! I got a picture.. Its MD5 hash is the flag.
