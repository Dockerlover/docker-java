# 基础镜像
FROM liuhong1happy/docker-ubuntu:2015.08.21
# 维护人员
MAINTAINER  liuhong1.happy@163.com
# 添加环境变量
ENV USER_NAME admin
ENV SERVICE_ID openjdk-8-jdk
ENV LANG C.UTF-8
ENV JAVA_VERSION 8u66
ENV JAVA_DEBIAN_VERSION 8u66-b01-1~bpo8+1
ENV CA_CERTIFICATES_JAVA_VERSION 20140324
# 安装jdk
RUN echo 'deb http://httpredir.debian.org/debian jessie-backports main' > /etc/apt/sources.list.d/jessie-backports.list
RUN set -x && apt-get update && apt-get install -y openjdk-8-jre-headless="$JAVA_DEBIAN_VERSION" \
        ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION"  && rm -rf /var/lib/apt/lists/*
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# 暴露80端口
EXPOSE 80
# 运行supervisord
CMD ["/usr/bin/supervisord"]