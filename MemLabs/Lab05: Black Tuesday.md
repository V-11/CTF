**Black Tuesday**
===================  
[Challenge Link](https://github.com/stuxnet999/MemLabs/tree/master/Lab%205)  

> We received this memory dump from our client recently. Someone accessed his system when he was not there and he found some rather strange files being accessed. Find those files and they might be useful.  
> Note: There're 3 flags in this challenge, you will get the stage 2 flag only when you have the stage 1 flag.

Let's use the [imageinfo](https://github.com/volatilityfoundation/volatility/wiki/Command-Reference#imageinfo) command to get the suggested profile which we will pass as the parameter to `--profile` when using other plugins.

![](images/Lab5_01.png)  

Let's check the active processes when this memory dump was taken.. to do so, I will use the [pslist](https://github.com/volatilityfoundation/volatility/wiki/Command-Reference#pslist) plugin.

![](images/Lab5_02.png)  

Since `WinRAR.exe` is active, there must be a `.rar` file somewhere, let's find it!  
To do so, I will use the [filescan](https://github.com/volatilityfoundation/volatility/wiki/Command-Reference#filescan) plugin.

![](images/Lab5_03.png)  


Good, let's dump it.. to do so, I will use the [dumpfiles](https://github.com/volatilityfoundation/volatility/wiki/Command-Reference#dumpfiles) plugin and pass the physical address as a parameter to `-Q`

![](images/Lab5_04.png)  

I tried to extract it but it was password-protected.  
The author said ***you will get the stage 2 flag only when you have the stage 1 flag*** so let's find the 1st stage's flag.  
After some googling I found the [iehistory](https://github.com/volatilityfoundation/volatility/wiki/Command-Reference#iehistory) plugin which we can use to browse the history of recently-accessed files.  
Going through the output I noticed the following:

![](images/Lab5_05.png)  

Base64 encoded string, decoding it got me the first flag :D  

> **flag{!!_w3LL_d0n3_St4g3-1_0f_L4B_5_D0n3_!!}**

I used this flag as a password for the `.rar` file we already dumped and it got me the second flag :D

![](images/Lab5_06.png)  

As you can see in the previous picture, the lab is done, but the author claimed otherwise.  
I spent a lot of time analysing and searching for the 3rd flag but found nothing, I messaged the author but he didn't respond *yet*.  
If any of you got the 3rd flag please hmu with a hint on twitter @0x1411

--------------------------------------------
