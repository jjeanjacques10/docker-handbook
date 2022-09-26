# Docker Handbook

<br />
<p align="center">
    <img src="https://www.docker.com/wp-content/uploads/2022/03/Moby-logo.png.webp" width="200" alt="Logo">
    <p align="center">
    This is a collection of Docker-related articles and tutorials. It is a work in progress.
      <br />
      <a href="https://github.com/jjeanjacques10/docker-handbook/blob/main/examples/README.md"><strong>Explore the examples »</strong></a>
    </p>
</p>

<p align="center">
   <a href="https://www.linkedin.com/in/jjean-jacques10/">
      <img alt="Jean Jacques Barros" src="https://img.shields.io/badge/-JeanJacquesBarros-25ABE1?style=flat&logo=Linkedin&logoColor=white" />
   </a>
  <img alt="Repository size" src="https://img.shields.io/github/repo-size/jjeanjacques10/docker-handbook?color=25ABE1">

  <a href="https://github.com/jjeanjacques10/docker-handbook/commits/master">
    <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/jjeanjacques10/docker-handbook?color=25ABE1">
  </a>
  <img alt="License" src="https://img.shields.io/badge/license-MIT-25ABE1">
  <img alt="GitHub Pull Requests" src="https://img.shields.io/github/issues-pr/jjeanjacques10/docker-handbook?color=25ABE1" />
  <a href="https://github.com/jjeanjacques10/docker-handbook/stargazers">
    <img alt="Stargazers" src="https://img.shields.io/github/stars/jjeanjacques10/docker-handbook?color=25ABE1&logo=github">
  </a>
</p>

## Table of Contents

- [Docker Handbook](#docker-handbook)
  - [Useful commands](#useful-commands)
  - [Docker-compose examples](./examples/README.md)
    - MySQL
    - Redis
    - SQS
    - DynamoDB
    - Kafka

## Useful Commands

- Download an image

``` bash
docker pull <image>
```

- Start and stop the container

``` bash
docker [start|stop] <container>
```

- Run a container with configs

``` bash
docker run -d -p 80:80 --name webserver nginx
```

- Stop or remove all containers

``` bash
docker [rm|stop] $(docker ps -a -q)
```

## Interacting with Containers

- Run a command in a container

``` bash
docker exec -it <container> <command>
```

It's possible run a script:

``` bash
docker exec -it <container> command.sh
```

- Copy files from a container

``` bash
docker cp <container>:<path> <path>
```

## Images

- Delete all images

``` bash
docker rmi $(docker images -q)
```

- Remove all unused images

``` bash
docker image prune
```

---
Developed by [Jean Jacques Barros](https://github.com/jjeanjacques10)
