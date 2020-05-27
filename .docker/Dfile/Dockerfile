FROM gcc:latest

MAINTAINER GF_chen@163.com

ENV PATH /usr/bin/gcc:$PATH

RUN  mkdir /home/Data

COPY helloworld.c /home/Data/

WORKDIR /home/Data

RUN gcc helloworld.c

FROM centos

RUN yum install -y curl

ENTRYPOINT [ "curl", "-s", "http://ip.cn" ]
#use github and pull back
