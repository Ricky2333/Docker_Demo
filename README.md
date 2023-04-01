# Docker

Hey, guys.

I'm Ricky, a college student majoring in Computer Science. 🧑🏻‍💻

Recently, I have been learning Docker and I came across [Docker Crash Course for Absolute Beginners](https://youtu.be/pg19Z8LL06w) on YouTube. I found this tutorial to be an excellent resource for anyone who is just starting out with Docker.

I really appreciate the way [TechWorldwithNana](https://www.youtube.com/@TechWorldwithNana) teaches in the video. So I decide to share it with you. 😊

In this repository, I have listed the learning resources I use and my personal notes about it .

I hope this will be helpful for your understanding of Docker. 😄



## Links

### Video Tutorial 🎥

+ Crash Course - Docker in 1 Hour:  [https://youtu.be/pg19Z8LL06w](https://youtu.be/pg19Z8LL06w)
+ Complete Course - Docker Zero to Hero:  [https://youtu.be/3c-iBn73dDE](https://youtu.be/3c-iBn73dDE)



### Others

+ Docker Official Website: [https://www.docker.com/](https://www.docker.com/)
+ Docker Download Page: [https://docs.docker.com/get-docker/](https://docs.docker.com/get-docker/)

+ Original Repo: [https://gitlab.com/nanuchi/docker-in-1-hour](https://gitlab.com/nanuchi/docker-in-1-hour)



## Notes

+ **Basic Concepts of Docker**
  + Image
  + Container
  + Registry
+ **Basic Docker Command Line**
  + Image
    + `docker build -t [image_name] [directory_of_dockerfile]` 
      + build dockerfile to image
    + `docker images` 
      + show all the images you have on your local machine
    + `docker pull [image_name]:[version]`
      + pull a image from registry
  + Container
    + `docker ps` && `docker ps -a`
      + show all the containers you have on your local machine
    + `docker run --name [container_name] -d -p [host port]:[container port] image_name`
      + create a container based on a image ( `-d` → run it in background; `-p` → port binding)
      + 🍉 PS: Every time you use `docker run`, it will create a container. So if you want to re-run the existed containers, use `docker start` instead
    + `docker logs [container_id / name]`
      + logs about container
    + `docker stop [container id / name]`
      + stop running this container
    + `docker start [container id / name]`
      + start running this container
+ **Hands-on Demo**
  + **Clone** the demo repository ([Crash Course Repo](https://gitlab.com/nanuchi/docker-in-1-hour))
  + **Test** this code using Docker
    + Learning *how to write Dockerfile*
    + Use `docker build -t [image_name] .` to build Dockerfile to Docker image
    + Create a container based on that image
    + Open `localhost:3000` on web browser to check if the container is working properly
