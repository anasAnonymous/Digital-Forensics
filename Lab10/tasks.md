# HASH-1.  `48bb6e862e54f2a795ffc4e541caed4d`   
I used `hash-identifier` to identify the type of hash and I found out that it was a `MD5` hash.
![hashId1](https://github.com/anasAnonymous/Digital-Forensics/assets/123714177/2c1f3a33-463e-4e99-81d4-55bfef0ec8c7)     

This was the command I used to crack the hash:     
`hashcat -a 3 -m 0 48bb6e862e54f2a795ffc4e541caed4d --show`    

I used `-m 0` for `MD5`.    
![h1](https://github.com/anasAnonymous/Digital-Forensics/assets/123714177/599b24db-0eec-4aa4-928d-8f2e40492347)


# HASH-2.    

`0458ce29e1b0edb36665db68dc96f976dbce98a54696376d7297fce33e56de171d2d7f1ceaa9cbc74dd948c6d13a80dc0d2239ab5abe5f74e4506c9683f13fa7`    
***-----------------------------------------------------------------------------------------------------------------------------------------------------------*****       

 
I used `hash-identifier` to identify the type of hash and I found out that it was a `sha512` hash.
![hashId2](https://github.com/anasAnonymous/Digital-Forensics/assets/123714177/aff7fc9e-283b-4ca1-8396-b9fea016b875)     
I used `hashcat` with  `--increment` option but no luck as no hint was given. It was taking too much time and showing the status as exhausted.        
Then, I deecided to use `john` and this was the command I used:    
`john --wordlist=/usr/share/wordlists/rockyou.txt h2.txt --format=RAW-sha512`    
![h2](https://github.com/anasAnonymous/Digital-Forensics/assets/123714177/2e8ca695-1f72-4b15-a8fa-ddfc7e9bb46e)     
 



3. `11adeb3106116457ba233b1ef0989ff6b15f590cfe1ab0a7ce00401c429bd58c`     
I used `hash-identifier` to identify the type of hash and I found out that it was a `SHA-256` hash.    
![hashId3](https://github.com/anasAnonymous/Digital-Forensics/assets/123714177/f4b7210b-f21a-4d40-ae83-006d3cefc92e)     

This was the command I used.    
`hashcat -a 3 -m 1400 11adeb3106116457ba233b1ef0989ff6b15f590cfe1ab0a7ce00401c429bd58c "?u?d?d?l?s" --force`

I searched for the hash mode for `SHA-256` in hashcat help manual and it was `1400`. I set the characterset according to the hint given.     
![h3](https://github.com/anasAnonymous/Digital-Forensics/assets/123714177/5a927c2d-b125-4d91-8585-8070c16b3fc2)




4. `$6$sup3rstr0ngs4lt$fZt5XYt.hdLFCs7YOlSIXT.0cDaNIhtP5QdDRdYP6OD349oD8hR9mEYueBRxaSAEHtAJ85wYYNyEELJkb0QSW1`    
I tried `hash-identifier` to identify the type of hash but it was unable to guess the hash type. So, I used an online `hash identifier` and found out that it was a `sha512crypt` hash.    
![hashId4](https://github.com/anasAnonymous/Digital-Forensics/assets/123714177/5e60ffc1-377b-4a88-a93a-45ad93e02935)    

This was the command I used to crack the hash:   
`john --wordlist=/usr/share/wordlists/rockyou.txt hhh4.txt --format=sha512crypt`     
![h4](https://github.com/anasAnonymous/Digital-Forensics/assets/123714177/0d6b6d5f-15ae-4b18-83c1-e84083f59d23)



5. `7484c9a3d50e649f50411c58317eb7c6c6e506a94b04ebb87dd8715ce16de0d8e41a4894f9be4bbc7dbc204e1f7103e7b75844f78ce288f89befdfb53f9f5ac8`    
I used `hash-identifier` to identify the type of hash and I found out that it was a `` hash.
![hashId5](https://github.com/anasAnonymous/Digital-Forensics/assets/123714177/8cb27878-2c0b-448f-b6de-dbb4596864b4)

  
