If we have to analyze a malware, we will use VM not docker.

VM has separate `kernel` & `RAM` etc but DOCKER does not have.


sudo su
docker run -it alpine sh
echo "hi-world" > hi_world


NEW TAB
sudo su
docker ps
docker ps -all
docker export 99fd330531e5[id] -o output.tar
ls
mkdir newfolder
mv output.tar newfolder
cd newfolder
tar -xf output.tar
ls
docker diff 99fd330531e5
docker inspect 99fd330531e5
docker inspect --format='{{range .NetworkSettings.Networks}}{{.MacAddress}}{{end}}' 99fd330531e5[id]
docker inspect --format='{{.State.Pid}}' 99fd330531e5[id]
ps -fp 8686

