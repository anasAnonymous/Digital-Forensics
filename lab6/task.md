# Utilize the disk image from the section Analyzing a Disk Image to answer the following questions:

##  Q#1 : What are the MD5 and SHA1 hashes of the note.txt file?
MD5 : c91e969e9184267c35ddc3ff45f795d3
SHA1 : c61dce75ba83f186471297e2e0568ddd0cefe022

##  Q#2 : What's the MFT record number of the note.txt file? The answer may vary depending on the method used.
MFT record number : 40 (40960)

##  Q#3 : Can you determine the parent directory of the file named $Txf? You can use either analyzeMFT or MFTECmd to inspect the contents of the $MFT file to answer this question.
.\$Extend\$RmMetadata


##  Q#4 : The meme.jpeg image was originally downloaded from a twitter URL. Can you use MFTECmd to determine the original URL?
https://pbs.twimg.com/media/FadAHVAUUAAVp2Q?format=jpg&name=small


##  Q#5 : Can you analyze the $Boot file and determine the volume serial number in raw hexadecimal format?


