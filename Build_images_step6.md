Build Images

Now we will learn how to build images, docker images.
So far we have taken official docker images from Docker Hub and we ran them. But as per our requirements, we need to make changes so we can take an official image, make some changes and build our own customized image.

To build docker images, you need to write docker file B capital. We provide instructions in this file of how to build the image, what should it contain, what packages it should install, what volume to export. And then we run docker build command which
will create an image from the docker file. Just like we have palm XML for Maven which builds the artifact.

![Alt text](image-4.png)

![Alt text](image-5.png)

![Alt text](image-6.png)

And for this one, let's take a website from tooplate.com a template from that and we'll run it.
Or we'll host it in Apache2 service running in an Ubuntu container.