FROM docker.io/centos:7
USER root
RUN yum clean all \
 && yum repolist \
 && yum -y update \
 && yum -y install \
	epel-release tar unzip iproute inet-tools \
	tcpdump telnet traceroute curl iperf3 \
	knot-host openssh-client mtr-tiny socat nano \
	vim-tiny nmap iputils-ping
 && yum clean all
CMD ["/bin/bash"]
