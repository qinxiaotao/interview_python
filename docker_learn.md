docker overview

1. docker 是什么
docker 是一个虚拟机

2. docker的优势是什么
  让你像发布软件一样更新你的基础设施
  可以根据实际扩展和缩小你的基础设施

3. docker的架构
  docker-client -> docker daemon -> docker container 
 
4. docker的产品有哪些
  docker client
  docker daemon
  docker hub
  docker desktop
  docker objects 

5. docker的底层技术
  namespace 和 group

docker python install

Advanced Packaging Tool  apt

# syntax=docker/dockerfile:1 什么意思
 this directive instructs the Docker builder what syntax to use when parsing the Dockerfile, and allows older Docker versions with BuildKit enabled to upgrade the parser before starting the build.


 FROM python:3.8-slim-buster
 we need to add a line in our Dockerfile that tells Docker what base image we would like to use for our application.
 
 WORKDIR /app
  let’s create a working directory. This instructs Docker to use this path as the default location for all subsequent commands.
  
  docker build --tag python-docker . tag:set the name of image
