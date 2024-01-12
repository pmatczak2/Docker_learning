Docker Logs

Pull a fresh image
Run # docker inspect nginx: Now we can see detailed information about an image by using a command called docker inspect. Now, this is not logs, this is metadata of the image in JSON format.

# Docker run -d -P nginx: runs entry point CMD 
by running the command docker logs. I see docker logs. I can give the container name or
ID and it shows the output. 

purpose is troubleshooting, when you build your own images, which we will be doing. And when you run containers from your own custom built images, you might make some mistake and your container won't start.

How do you figure out what is the problem by looking at the output of the process and
that you can do it through docker logs command.

# docker run -d -P msql:5.7
# docker ps -a : container is in status exited
# docker logs “had logs of the container you ran” And we see the logs of this container.
So you see it says error entry point. It was running something in the entry point.
And it says database is uninitialized and password option is not specified.

# docker run -d -P -e MYSQL_ROOT_PASSWORD=mypass mysql:5.7

The process that starts the process output is the log. So if something goes wrong while the
process starts, you can check docker logs and you can find out the problem.
