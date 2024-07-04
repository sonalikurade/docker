# Docker command 
## The Most Usefull docker command  
* docker ps :- Only Running docker container

* docker images :- To list the local machine images 

* docker image ls :- To list the local machine images

* docker pull nginx :- To pull the images from docker hub

* docker run nginx :- To run the nginx continer in attached format or in foreground

* docker run -d nginx :- To run the container in dettached format or in background.

* docker ps -a :- All details of container which are running or stopped or killed.

* docker stop es28 :- (es28 is container id)  This command is used to stop the running container

* docker stop es28/container name :- (es28 is container id)  This command is used to start the stoped container or killed container.

* docker run -d --name Matfly httpd :- This command is used to give the name to httpd container. Matfly is httpd container name given by devloper.

* docker ps -q -a :- To find only id of all container which are present in the machine.

* docker ps -q :- To show id of only running container.

* docker inspect ef8 :- (ef8 is container id) This command is used for to view the full information about the perticular container.

* docker run -d -P nginx :- To give public access to nginx container for any browser access. Allocate the port from docker. Docker post start from 32768 and end with 65536.

* docker run -d -p 8080:80 nginx :- Small p is for user defined port. To access our website publicly. 

* docker exec -it a7623 ls :- (a7623 is container id) (-it is insert into) This command is used for to view the container information without entering into that container.

*  docker exec -it a7623 bash :- To go inside the contaier 

* exit or control + d :- To exit the container.

* docker commit 7634 :- Image created from that(7634) container.

* docker run -d 628 :- Running docker container created by image.

* docker tag 6789 my-image:version1 :- To give the name and tag for that image.

* docker kill 6812 :- To kill the running process. When we kill the process we get 137 code. when we stop the process we get 0 (zero) code.

* docker rm 2266 :- To remove or delete the container permantly

* docker kill `docker ps -q` :- To kill the all container in one time which are running.

* docker start `docker ps -a -q` :- To start all the container at one time which are stoped.

* docker start `docker ps -aq` :- To start all the container at one time which are stoped.

* docker rm `docker ps -a -q` :- To delete all the container at one time which are stoped.

* docker logs 2678 :- To view the docker container logs

* docker cp index.html 2687:/usr/share/nginx/html/index.html :- To copy file from local host to container.

* docker cp 2687:/usr/share/nginx/html/index.html  index.html:- To copy file from container to local host.
