FROM centos:centos6
MAINTAINER "Tim Hughes" <thughest@thegoldfish.org>
ENV container docker
RUN yum clean all; yum -y install hostname tar git; yum -y update; yum clean all
VOLUME [ "/sys/fs/cgroup" ]
CMD ["/sbin/init"]

