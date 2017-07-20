FROM centos:centos6
MAINTAINER "Tim Hughes" <thughest@thegoldfish.org>
ENV container docker
RUN yum clean all; yum -y install hostname tar git; yum -y update; yum clean all
CMD ["/sbin/init"]

