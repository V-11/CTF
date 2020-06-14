**Brute Force is Fun!**
-------------
[Challenge Link](https://mega.nz/#!vf43RCyC!NNpuYjB3d-gevhsHXefwAAAmzk4tJHxUZr0GnrSDI_c)  

> You'll need Brute Force to solve this.  
> e82a4b4a0386d5232d52337f36d2ab73

I didn't know what to do with this hash but I cracked it anyway using this [site](https://hashes.com/en/decrypt/hash).  
I downloaded the picture.. It was kinda large so I thought there might be some compressed files.. I was right.  
I extracted them using the command `binwalk -D='.*'`  
I got a huge number of folders and a password-protected `flag.zip`  
I tried the cracked hash and it was correct.  
I got a base64 encoded string.. I decoded it using this [site](https://www.base64decode.org/).

I don't know what is *hard* in this challenge.
