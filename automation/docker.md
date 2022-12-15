<div>
<p style = 'text-align:center;'>
<img src="https://developers.redhat.com/sites/default/files/styles/article_feature/public/blog/2014/05/homepage-docker-logo.png?itok=zx0e-vcP" alt="docker" width="200px">
</p>
</div>

# Definition

 is an open source software for creating software containers, which facilitates migration between different systems and guarantees full operation, avoiding any kind of possible dependency problem between software versions of different hosts.

## Container 

Containers are an abstraction at the app layer that packages code and dependencies together.

It is a packaging of a program or software, such as databases, web pages or any other type of software that optimizes the space occupied and facilitates migration between different servers.

<div>
<p style = 'text-align:center;'>
<img src="https://static.platzi.com/blog/uploads/2016/06/image00-1.png" alt="jenkins" width="300px">
</p>
</div>

## Docker Architecture

its structure works with the communication between the client and server, the client is the one who communicates with Docker deamon, which is responsible for building, running and distributing containers, this communication can occur locally or can also be done remotely. 

<div>
<p style = 'text-align:center;'>
<img src="https://geekflare.com/wp-content/uploads/2019/09/docker-architecture-609x270.png" alt="jenkins" width="400px">
</p>
</div>

## main commands

* docker run : runs the container from an image
* docker build: create a Docker image
* docker pull: allows you to download the most recent image from that repository. you can also specify which version of the image you want to download.
* docker commit: Creating a Docker image from a container
* docker ps: shows the active containers
* docker ps -a: shows all containers
* docker inspect "container ID": shows the complete detail of a container
* docker run –-name: renames the ID of a container
* docker rm: to delete a container
* docker container prune: deletes all inactive containers
* docker container kill: Stops a moving container

## Docker file
is a text file containing instructions on how to create a new container image.

an example of its syntax is:
<pre><code># syntax=docker/dockerfile:1
FROM ubuntu:18.04
COPY . /app
RUN make /app
CMD python /app/app.py
</code></pre>

* FROM creates a layer from the OS Docker image.
* COPY adds files from your Docker client’s current directory.
* RUN builds your application with make.
* CMD specifies what command to run within the container.

## installation

https://docs.docker.com/desktop/install/linux-install/