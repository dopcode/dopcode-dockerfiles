FROM docker.io/centos:7
USER root
RUN yum clean all \
 && yum repolist \
 && yum -y update \
 && yum -y install epel-release tar unzip vim \
	iproute bind-clients iperf3 mtr socat \
	openssh-client tcpdump telnet mtools traceroute \
 && yum clean all
CMD ["/bin/bash"]
