FROM centos:centos7
RUN yum clean all \
 && yum repolist \
 && yum -y update \
 && yum -y install \
	epel-release tar unzip iproute \
	tcpdump telnet traceroute curl iperf3 \
	knot-host openssh-client mtr-tiny socat nano \
	vim-tiny nmap iputils-ping net-tools rdate NetworkManager \
	firefox \
 && yum clean all
CMD bash
