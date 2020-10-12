**Pressure**
===================  
[Challenge Link](https://s3-eu-west-1.amazonaws.com/hubchallenges/crypto/output)

> High-pressure encryption! Break it!

One of my friends once told me about [Zlib Compression](https://zlib.net/zlib_how.html) and I used it to solve this challenge.  
I uploaded the file to [CyberChef](https://gchq.github.io/CyberChef/) and noticed there were some readable characters in it.  
I tried [Zlib Deflate](https://gchq.github.io/CyberChef/#recipe=Zlib_Deflate('Dynamic%20Huffman%20Coding')) and [Zlib Inflate](https://gchq.github.io/CyberChef/#recipe=Zlib_Inflate(0,0,'Adaptive',false,false)) but they both resulted an error.  
I used a text editor to delete these readable characters then tried again but failed.  
I used a hex editor to delete the bytes of these readable characters then tried again and got the flag :)
