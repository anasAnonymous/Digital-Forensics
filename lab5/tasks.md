# 1:  What are the different protocols present in the captured traffic file?
- ICMP
- TCP
- FTP
- HTTP

# 2:  It appears that the attacker is attempting to brute force the user's FTP password. Can you find any evidence of a correct password, and if so, what is it?
PASS batman

# 3:  What additional information was the attacker able to extract from the user's FTP account?
creadentials.txt , bash history

# 4:  What actions did the attacker take with the information obtained from the user's FTP account?
The attacker got the database username and password:
username: myuser
password: P@ssw0rd123456!


# 5:  What's the root account password?
Password: 1amgr000000t!@#$
id
(flag{1_4m_gr00000t!})


# 6:  Can you identify the packet numbers in which the attacker exploited the Remote Code Execution vulnerability to gain access to the system? What was the exact payload used by the attacker?
wget https://raw.githubusercontent.com/vonderchild/digital-forensics-lab/main/Lab%205/files/backdoor.py


# 7:  After gaining access to the system, what does the attacker seem to be doing?
The attacker is trying to start a shell session which spawn new shell process that's bin/bash.


# 8:  The attacker read a file from root's home directory. What was in that file?
File Name is : "gr00t.txt"
Content in the file : "Congrats on getting here. But that's not it, the real test starts now! ;)

Btw, here's your flag for this stage: flag{1_4m_gr00000t!}"


# 9:  The attacker downloaded a file inside root's home directory. What's the purpose of that file?
Downloaded file : backdoor.py
The program first asks for the username and password from the user as inputs, and upon successful login, it then asks for a message. The message is passed to a function which decrypts the message using a key "super_secret_key" and then the decrypted message is executed as a command.


# 10: What information was transmitted through the attacker's covertly established channel of communication?
flag{c0ngrats_1f_y0u_m4d3_1t_t1ll_h3r3_ch4mp} 
(The feeeelingggggggg <3333)
