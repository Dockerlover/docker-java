# 基础镜像
FROM liuhong1happy/docker-ubuntu:2015.08.21
# 维护人员
MAINTAINER  liuhong1.happy@163.com
# 添加环境变量
ENV USER_NAME admin
ENV SERVICE_ID openjdk-7-jre
ENV LANG C.UTF-8
ENV JAVA_VERSION 1.7.0_79
ENV JAVA_DEBIAN_VERSION 7u79-2.5.6-0ubuntu1.14.04.1
# 安装uzip和openjdk-6-jdk
RUN apt-get update && apt-get install -y openjdk-7-jre-headless="$JAVA_DEBIAN_VERSION" && rm -rf /var/lib/apt/lists/*
# 暴露80端口
EXPOSE 80
# 运行supervisord
CMD ["/usr/bin/supervisord"]
