**Keep Calm**
===================  
[Challenge Link](https://hubchallenges.s3-eu-west-1.amazonaws.com/Forensics/scatter.gif)  

> Keep calm and submit the flag!!

I got a fast GIF.. I used this [site](https://ezgif.com/speed) to slow it down then I was able to see 5 short strings.  
I noticed `MAo=` so my first guess was a base64 encoded string and this is the last piece.  
I got the string then I tried to submit it but it wasn't correct.  
I decoded then submitted it but again it wasn't correct.  
I thought of generating all possbile sets of the 5 strings.. You can use this [site](https://textmechanic.com/text-tools/combination-permutation-tools/permutation-generator/).  
Hint: Generate all possible sets but without `MAo=` because it will always be in the end.. This is how you get fewer sets.  
I had to decode them to check if I would get the flag.. You can use this [site](https://www.base64decode.org/).  
I got a long list of strings but only few of them are readable.. I decided to try them.. One of them was correct.  
Hint: It starts with a number :D
