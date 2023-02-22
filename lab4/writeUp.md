# Task 1
What IP address does the attack seem to be originating from?

    192.168.0.106

# Task 2
Which vulnerabilities do you think are being exploited, and what evidence do you have to support your findings?
    
    SQLi

# Task 3
How can we determine what web browser the attacker is using?

    We can chech in logs that attacker is using "Firefox 102.0" web browser.
    
# Task 4
Did the attacker use any automated tools during the attack? If so, can you identify the name of the tool and its purpose?
    
    SQLmap
    It is used to detect and exploit SQL injection flaws automatically.
    
# Task 5
Which file was the attacker trying to access but couldn't due to limited server access?
    
    /etc/shadow

# Task 6
Did the attacker gain access to any confidential data? If yes, how much data was compromised?

    Yes. The attackers gained access to /etc/passwd. Users details have been compromised.
    
# Task 7
An important secret was compromised. Can you figure it out? Hint: The secret you're looking for is not in a .sql or a .php file.

    Yes. The compromised file is "important_note.txt"

# Task 8
The attacker left a message for the server administrator. Find out what the message said, and also mention how you were able to find it.

    The message : flag{h1pp1ty_h0pp1ty_y0ur_w3bs1t3_1s_n0w_my_pr0p3rty!}
    I checked modsec_audit.log and these I saw a sentence "Gentlemen......" and a string was concatenated through ASCII codes. I converted from ASCII         codes to text, and found a ciphertext. I took help from cyberchef and I got a flag but it was not completed. Then, I searched for the word "Gentlemen"     in modsec_audit.log again using grep command and there I found a URL kinda thing. Repeated the same what I did earlier and managed to get the complete     flag this time.

# Task 9
What were some indicators that confirmed that an attack had taken place? What were your key takeaways from this attack?

# Task 10
Based on this attack, what indicators of compromise can be used to detect future attacks?
    
    We can use IDS to detect and set alarms when there's any attack in the future. And we can restrict access of unauthorized users to sensitive files by setting appropriate permissions check as we have for /etc/shadow.
