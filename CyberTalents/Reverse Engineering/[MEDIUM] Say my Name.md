**Say my Name**
===================  
[Challenge Link](https://s3-eu-west-1.amazonaws.com/hubchallenges/Reverse/a.out)

> Can you find my name?  

We got an ELF binary.. Let's open it with IDA.  
Starting with the main function.

![](images/say-may-name1.png)

It takes 2 inputs from the user (first name and last name) with the limit of 7 characters then it starts to loop.

![](images/say-may-name2.png)

1- It loops 7 times.  
2- Every time it xors a character from `firstname` with its equivalent index charachter from `lastname`.  
3- It stores the result in `s1` array.  
4- It checks if the values in `s1` are equal to the values in `unk_97F`.  
Let's jumpt to check it out.

![](images/say-may-name3.png)

`unk_97F` values = [0x5, 0x1D, 0x0D, 0x4, 0x10, 0x72, 0x0]

The following script got me the flag. 

![](images/say-may-name4.png)
