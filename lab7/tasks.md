##  Task (1)
`flag{s0m3_susp1c10us_str1ng}`

![t1cttr](https://user-images.githubusercontent.com/123714177/230892539-9dbcbedc-8c28-41cc-b870-1bb4a7cc47b5.png)
![t1cbrchf](https://user-images.githubusercontent.com/123714177/230892565-acebcd9f-5717-4923-99ea-c6b811af9caa.png)  




##  Task (2)
`flag{sup3r_s1mpl3_x0r}`

I opened the task in `clutter`. There was a prompt `"Enter the first magic number"` and `"hmm" function` was called.
![t2main](https://user-images.githubusercontent.com/123714177/230893587-fba55857-6582-4b52-a952-0fb4345c21a5.png)

Then, I went to analyze `"hmm" function`. There were if conditions which were validating the inputs and upon giving the correct input, it was asking for the next magic number. 

##  Correct inputs :
1st magic number = 0x17(hex)  = `23(dec)`  
2nd magic number = 0x539(hex) = `1337(dec)`  
3rd magic number = 0xfc(hex)  = `252(dec)`
![t2hmm](https://user-images.githubusercontent.com/123714177/230894783-45eedfbb-62b9-45a2-b152-4686f176b411.png)

Then, I run the task2 in terminal and upon entering correct inputs, got the flag.
![t2flag](https://user-images.githubusercontent.com/123714177/230895009-00a42e74-b3ad-456d-a928-ddd8d31c5615.png)  




##  Task (3)
`"flag{r3v3rs3_3ng1n33r1ng_101}"`  


I opened this task using `Cutter` to analyze. There was a function `do_shenanigans();` in the main function. I navigated to this function and found some variables with hex values assigned. I decoded and this was a set of characters `a-z`, `{}` and a `_`.
![t3set](https://user-images.githubusercontent.com/123714177/231559477-ce1db358-e962-458d-8c39-3ef298011b1d.png)


There were some more variables with hex values assigned. I decoded them and used as indices to create a string which was the `flag`.
![t3indices](https://user-images.githubusercontent.com/123714177/231559517-3f852dc4-e0bd-4f3d-8245-17be91ca1d78.png)

I had to increment indices to get the correct flag.  




##  Task (4)
`flag{4_m3d10cr3_m4lw4r3_ch4ll3nge}`
Here, we have a python file which has some variables. I tried decoding hex values assigned to them but could not find anything useful. But when I run the code, the program was asking for a password. I analyzed the code and found out that the variable `a` was printing the `"enter password"` prompt. So, I edited the code and print he varibale `a`.
![t4pyfile](https://user-images.githubusercontent.com/123714177/231499366-4c6b0c09-9757-457c-9d68-0bdd27fb303a.png)


Then, I run the code and this was the output. 
![t4printA](https://user-images.githubusercontent.com/123714177/231500091-b0b9784f-b49d-471e-a467-878a40dfd004.png)


I copied the first hex string I found and decoded using `cyberchef` and I got a `key`.
![t4cbrchf](https://user-images.githubusercontent.com/123714177/231500713-a39d74f0-9395-46dc-9621-29ec4041e296.png)


I entered the key as a password and found the `flag`.  
![t4flag](https://user-images.githubusercontent.com/123714177/231501752-95e110a2-4aa5-4c7e-8a45-52f6498219bd.png)
