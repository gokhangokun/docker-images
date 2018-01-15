FROM centos:centos7

LABEL name="Nodejs Base Image"
LABEL version="1.0"
LABEL description="Nodejs Base Image  Python - Nodejs - PM2 on CentOS 7"

LABEL maintainer="gokhan.gokun@trendyol.com"

RUN yum -y update; yum clean all

RUN yum -y install epel-release; yum clean all

RUN yum -y install python-pip; yum clean all

RUN yum -y install nodejs npm; yum clean all

RUN npm install -g pm2
RUN npm cache clean