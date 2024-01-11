Docker Introduction
![Alt text](image.png)

We isolate our services. Now, when I'm saying here services, I mean services like Tomcat or Apache or NGINX or MySQL, any kind of service that we run on the operating system. What does it really mean by isolate?
Well, if we are setting up an infrastructure or application stack, we will set up web
service on a different operating system, on different machine engines, on a different machine, Tomcat on a different machine, MySQL on a different machine. We can take a big machine and put all the services in that. But then the services are not isolated.They will be interfering with each other's business like their libraries binaries their configuration or resources.Ram CPU will be shared same process tree, so they'll be interfering with each other. So we isolate our services and for high availability we put them into multiple servers.
And to isolate our service to host our application, we need the infrastructure.
to isolate our service to host our application, we need the infrastructure.
We can use virtual machines or cloud computing. Even in cloud computing we'll be using
instances which will be again VMs. So every VM will have its own operating system.
We run the service on that and then it is isolated. So your operating system is the boundary to isolate it. Now because of isolation we end up setting up multiple VMs or instances or multiple servers. But we have to do that to achieve high availability, performance, security.
VMs or the ec2 instances we are talking will be over provisioned. high capital expenditure and high operational expenditure. You have to upfront purchase things like if we
talk about operating system, licensing of multiple operating systems you have to purchase, then there will be operational expenditure, regular maintenance, cost, cooling power, admin team, operations team to manage all that.

![Alt text](image-1.png)

We need to do all the nurturing operating system needs licenses if you're going with licensed operating system.
And also operating system takes time to boot. So like for example in an auto scaling
group, the instances scale automatically, but it takes time to come up complete operating system is booted and then the service comes up.
Now, VMs are portable. We can move VMs from one place to other place.
It's nothing but set of files. So you can move it from cloud to
local, local to cloud, but they're bulky. Like if you have to move the entire stack.
Let's say you have five to seven services, so you need five to seven images.
And that images distributing is possible, but because of its huge size, it's not
possible to distribute to everyone.VM is running the operating system and
operating system needs resources, ram, CPU, network, disk, space, all of that.
And remember, all this we are doing so we can isolate our service.

![Alt text](image-2.png)

Keep that point in mind, few other points or all the other points.
Now take a note, isolating services are important and we need operating systems for that.
Operating system creates the boundary for isolation. We want high availability, so we will
need multiples of the VMs, like multiple NGINX, multiple Tomcat, multiple RabbitMQ.
That is increasing the cost more further. Now, portability matters to this time.
How about I'm able to ship the entire image every time I'm making changes, instead of doing all the automation and provisioning everything from the scratch.
Instead of that, how about for every change we have the image and we can distribute it.
Images can be directly replacing your existing VMs. In dev QA staging production environment it is easier, but because of VMs bulky size, we cannot do it.

![Alt text](image-3.png)
![Alt text](image-4.png)

Keep in mind, container is a kernel trick. There's no magic about it. Of course it needs the resources, it needs Ram CPU as any process would need. So every container that is running in the operating system, all these containers are going to share the operating systems kernel and kernel will provide the right resources to the process. And because of that is happening, you don't need a separate operating system running in the container. So container you can also treat like a  package which has all the necessary things.

![Alt text](image-5.png)
![Alt text](image-6.png)

