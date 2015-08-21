# docker-java

Docker化Java

## 镜像特点

- 2015/08/21 继承基础镜像docker-ubuntu

## 使用方法

- 获取代码并构建

        git clone https://github.com/Dockerlover/docker-java.git
        cd docker-java/openjdk-7-jre
        docker build -t docker-java:openjdk-7-jre .
        ...
        cd docker-java/openjdk-6-jre
        docker build -t docker-java:openjdk-6-jre .
