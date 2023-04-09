##  Exercises

You work as a senior digital forensic investigator for an intelligence agency that specializes in investigating cybercriminals. Recently, they made a major breakthrough in a case against a notorious ransomware gang and were able to apprehend several members of the gang, including their leader. In the course of the arrest, the team acquired memory dumps of each of the gang members' computer.

It is suspected that the leader was using Windows 7 at the time, and had been hiding some secret information related to the gang's operations on his computer. Being a senior member of the team, the intelligence agency has trusted you with the memory dump of the leader's computer and has tasked you with finding the secret information which could potentially be hidden in the following places:

    It may have been copied to the clipboard.
    It may have been searched for on the internet.
    It may have been saved in an environment variable.
    It may have been executed as a command.
    It may have been drawn using MSPaint.

The secret information you are looking for is in the form of a flag with the format flag{xxxx}, where xxxx represents a set of alphanumeric characters that make up the flag. There are a total of 5 flags that you need to find. Good luck!

The memory dump can be downloaded from https://drive.google.com/file/d/1Gm7huRq0aa1is1dv0LqJcABcRYlS-Sqn/view?usp=sharing.


##  Flag 1 :
As the hint suggesed that it may be copied in the clipboard. So, I tried "clipboard" flag and found the flag.
![clip](https://user-images.githubusercontent.com/123714177/230758658-5bc7286d-376c-4cf4-919a-e9f6d23955b5.png)



##  Flag 2 :
For this flag, we have to check the browser history. I skim the flag options to find any relatable flag but I could not find as there were a lot of options. Then, I tried grep command and search for the string "history" and fortunately found "iehistory" flag.
![history](https://user-images.githubusercontent.com/123714177/230760222-5f2bc402-1f0b-4e7b-b6a2-b1fac7428afc.png)

I used the "iehistory" and found the flag.
![iehistory](https://user-images.githubusercontent.com/123714177/230760493-62ce108e-b969-4664-9464-b7cf74314269.png)



##  Flag 3 :
Again, it was hinted to check environment variables. So, I used "envars" flag and found the flag.
![envars](https://user-images.githubusercontent.com/123714177/230759100-1aa7108e-e25e-411a-b8e0-d286cf25949e.png)



##  Flag 4 :
We have to find the executed command. I tried "cmdscan" flag and I found a base64 encoded string.
![cmd](https://user-images.githubusercontent.com/123714177/230759424-4f132883-f6e9-40b2-9d67-37ed1c4a4ab5.png)

I used cyberchef to deccode the string and found the flag.
![cmdCyberChef](https://user-images.githubusercontent.com/123714177/230759305-c7f1db7f-15df-47d4-a0ff-9dcf34631b18.png)



##  Flag 5 :
The hint says that it may be drawn using MSPaint. So, I tried searching for the word "paint" in the help section lol. Of course I could not find anything. Then, I 

