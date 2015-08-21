# 基础镜像
FROM liuhong1happy/docker-ubuntu:2015.08.21
# 维护人员
MAINTAINER  liuhong1.happy@163.com
# 添加环境变量
ENV USER_NAME admin
ENV SERVICE_ID openjdk-6-jdk
ENV LANG C.UTF-8
ENV JAVA_VERSION 6b36
ENV JAVA_DEBIAN_VERSION 6b36-1.13.8-1~deb7u1
# 安装uzip和openjdk-6-jdk
RUN apt-get update && apt-get install -y openjdk-6-jdk="$JAVA_DEBIAN_VERSION" && rm -rf /var/lib/apt/lists/*
