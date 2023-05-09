##  EXERCISES 
To complete the exercise, it is important to first understand what Dockerfiles do. You can find the official Docker documentation on Dockerfiles here[https://docs.docker.com/engine/reference/builder/].

The container image you will be working with was built using the following Dockerfile:

FROM alpine:latest

RUN echo "flag{?????????}" > flag1.txt

COPY flag2-part1.txt flag2-part1.txt

ADD flag2-part2.txt flag2-part2.txt

ENV flag3 flag{?????????}

CMD ["sh", "-c", "echo flag{?????????}"]

 I don't know, this line got corrupted I guess, but I'm sure you'll figure it out
COPY ????????????????????????????????????

 Deleting my secrets, I'm sure nobody will be able to see them now :D
RUN rm flag1.txt flag2-part1.txt flag2-part2.txt

You can download the container image inside the tar archive from here[https://github.com/vonderchild/digital-forensics-lab/blob/main/Lab%2009/files/secrets.tar]. It contains a total of 5 hidden flags that you need to find. Good luck!



## FLAGS 


## Flag 1:
`flag{th1s_w4s_4n_34sy_0n3}`   
I extracted `layer.tar` which was placed in the first folder named `27e0b1ed433ce34a49a3c82c08fcf171910dff9ecf6470cd5d48de3e865302f3` and got a file named `flag1.txt`   

![f1_extracted](https://user-images.githubusercontent.com/123714177/235437515-ca23ada3-1c60-4940-8535-a0e59abd647e.png)    

And I found the flag inside that `flag1.txt` file.


## Flag 2:
`flag{c0ngr4ts_0n_f1nd1ng_th3_n0t_s0_w3ll_h1dd3n_s3cr3t}`   
I extracted `layer.tar` which was placed in the folder named `78f5e7ff9b9409eaadf09d30285307e4f88f792209ba718b4104bb3767d40fbf` and got another folder named `var` then another folder named `log` and then inside that folder a file named `secret.txt` was placed.    


I found a string inside `secret.txt`.    
![fl2_secretTxt](https://user-images.githubusercontent.com/123714177/235438926-b242cdb7-2909-4aa2-a423-e981712cd39d.png)   

I decoded that using `cyberchef` and found the `flag`.    
![fl2_cyberchef](https://user-images.githubusercontent.com/123714177/235439182-df811f2f-502e-455f-bbac-6930904ed150.png)     



## Flag 3:
`flag{dr34d_1t_run_f0r_1t_d3st1ny_4rr1v3s_4ll_7h3_s4m3}`    
I extracted `layer.tar` which was placed in the folder named `78323bfdc56789ddb0df6330bc8e3b641752c27aa594e6ca21d0115dd71090e8` and got a file named `flag2-part2.txt`   
![fl3_fl2P2](https://user-images.githubusercontent.com/123714177/235440346-28bc12f5-f3e1-4af6-93f5-65025b42369b.png)


I opened the file `flag2-part2.txt` and found the `2nd part` of the flag.    
![fl3fl2_2](https://user-images.githubusercontent.com/123714177/235440592-6c33e239-f165-4929-afc7-deb94adb8190.png)    


But where is the part 1 ??   

For that, I extracted `layer.tar` which was placed in the folder named `2336840b6581528adfb39f5a9dcd4ee10297e7cccb3d7b7eada4279cf88d027b` and got a file named `flag2-part1.txt`  
![fl3_fl2P1](https://user-images.githubusercontent.com/123714177/235440355-e164b3a5-892b-4204-a8d5-a88c5c0b6eac.png)      


I opened the file `flag2-part1.txt` and found the `1st part` of the flag as well.    
![fl3_fl2P1](https://user-images.githubusercontent.com/123714177/235440635-d4fca7b3-ea26-421c-b335-4a1dbab2f02c.png)    


## Flag 4:
`flag{3nv1r0nm3nt_v4r1abl3s_1ns1d3_c0nta1n3rs}`  

I opened the file named "27b200a787553581f1a9e42556052f7e38113539224093834b7f48a03693c879.json"    
![f4_f5](https://github.com/anasAnonymous/Digital-Forensics/assets/123714177/47eedf94-efd4-44c6-9701-62df88628ba5)    

I found the flag inside the file.   
![f4](https://github.com/anasAnonymous/Digital-Forensics/assets/123714177/419914d8-903e-4223-aa1d-b76af7915869)    


## Flag 5:
`flag{th1s_w4s_4n0th3r_34sy_0n3}`   

I opened the file named "27b200a787553581f1a9e42556052f7e38113539224093834b7f48a03693c879.json"    
![f4_f5](https://github.com/anasAnonymous/Digital-Forensics/assets/123714177/47eedf94-efd4-44c6-9701-62df88628ba5)    

I found the flag inside the file.   
![f5](https://github.com/anasAnonymous/Digital-Forensics/assets/123714177/25f1dcf4-28c7-4997-9d57-82838db980ce)
