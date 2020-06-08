**Help Ann**
===================  
[Challenge Link](https://s3-eu-west-1.amazonaws.com/hubchallenges/Forensics/help_ann_please)  

> Ann scanned a QR code of an item.. she tried to open the image but it was corrupted.  
> Can you identify what's her lost item?

Since it's corrupted I opened it with a hex editor to check the file signature.

![](images/help-ann1.png)

PNG? hmm.. I checked this [list](https://en.wikipedia.org/wiki/List_of_file_signatures) to get the correct signature.

![](images/help-ann2.png)

We have to replace `00` with `89`.. Use whatever hex editor you like.. I used [bless](https://github.com/bwrsandman/Bless).  
Save the changes and you would get a QR code.. Scan it however you like.. I used this [site](https://webqr.com/index.html).
