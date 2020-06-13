**Ambush Mission**
-------------
[Challenge Link](https://mega.nz/#!TKZ3DabY!BEUHD7VJvq_b-M22eD4VfHv_PPBnW2m7CZUfMbveZYw)  

> Our team had intercepted the communication between the target with his fellow and found this image.  
> It looks like they are going to meet in specific place, but we still don't know the time yet. Can you help me?

I tried `strings`, `exiftool` and `binwalk` but found nothing interesting.  
I tried some [Forensically](https://29a.ch/photo-forensics/) tools till I got a string.  
The two equal signs meant it was a base64 encoded string but reversed.. Reverse then Decode and you will get the flag.
