Docker volumes

Containers are generally known for its volatile nature. That's because containers are disposable. The way you make any change in a container is always through the image.
So if you want to add a package or a configuration file or any serious change you want to do
in the container, you don't log in and make changes. That's because they're disposable.
We delete them and we create an updated container from an updated image.

Container Volumes

![Alt text](image-3.png)

# docker pull mysql:5.7

What is the volume directory and what port number process runs.

# docker inspect mysql:5.7
Displays information look for “volumes” , and Entry point” 

# docker run —name vprofiledb -e MYSQL_ROOT_PASSWORD=“GIVE SOME VALUE” -P 3030:3306 -v 

Create a directory
 #—name vprofiledb -d -e MYSQL_ROOT_PASSWORD=“GIVE SOME VALUE” -P 3030:3306 -v -p 3030:3360 -v /home/ubuntu/“name_of_directory:”/var/lib/mysql mysql:5.7

Remove this container

Bind mount is mostly used to inject data from host machine to the container, like code developers are writing.

# Docker volumes
Creates a volume and run

if I happen to delete that container, the data is still in my host machine in a volume, I can attach
it to the new container when it gets created.

#Docker inspect 
docker inspector on a container will give almost similar information with more about container in JSON format.

Docker logs command and the container name, is great for trouble shooting. 