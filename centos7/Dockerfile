FROM centos:latest

MAINTAINER Steve Dalby <steve.dalby@mongodb.com>

RUN yum -y update; yum clean all
ADD ./mongodb-org-3.2.repo /etc/yum.repos.d/mongodb-org-3.2.repo
RUN yum install -y mongodb-org
RUN mkdir -p /data/db

EXPOSE 27017
ENTRYPOINT ["/usr/bin/mongod"]
