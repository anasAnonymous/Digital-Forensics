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


## Flag 2:
``


## Flag 3:
``


## Flag 4:
``


## Flag 5:
``
