![Alt text](image.png)

So docker engine is a daemon It's a service running in the operating system. 

Docker Containers:

Docker containers that run on Docker Engine:

Standard: Docker created the industry standard for containers, so they could be portable anywhere

Lightweight: containers share the machines OS system kernel and therefore do not require and OS per application, driving higher server efficiencies and reducing server and licensing costs. 

Secure: Application are safer in containers and cooker provides the strongest default isolation capabilities in the industry.

Step Detail

Let's learn by really doing it now so we will take an ec2 instance
we'll install docker engine on that. We'll take Ubuntu operating system, we'll install
docker engine on that and then we’ll run some containers on it.

Docker setup:

AWS lunch EC2 instance with ubuntu services.
Download and install, follow docker documentation for those instructions.
SSH to your docker engine you started in EC2.
Follow Docker documentation how to download Docker for your Linux ubuntu service.
Follow all the commands in Docker documentation and execute them.
Check docker service (systemctl status docker)
Add your ubuntu user to docker group
Validate this by running a test. Run “docker run hello-world” pulls a image form docker hub.

Docker Commands & concepts:

Start with docker hub. It is the back bone of docker. This is a place where there are lots of official images.

Docker Image:

A Docker image is a lightweight, standalone, and executable package that includes everything needed to run a piece of software, including the code, runtime, libraries, dependencies, and system tools. Docker is a containerization platform that allows you to package applications and their dependencies into containers, which are isolated environments that can run consistently across different environments.

A stopped container like vm image.
Consist of multiple layers. 
An app will be bundled in an Image.
Containers runs form images.
Images are called as Repositories in Registries.

![Alt text](image-1.png)

Creating Container:

# docker run

![Alt text](image-2.png)

Back form Docker hub find Nginix.
Pull the image
In CLI # docker pull nginx
Running the nginx network globally asking a host port
Access you CE2 access to the host port

