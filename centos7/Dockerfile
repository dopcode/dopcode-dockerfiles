FROM centos:7
RUN yum clean all \
 && yum repolist \
 && yum -y update \
 && yum -y install \
	epel-release tar unzip iproute net-tools \
	tcpdump telnet traceroute curl iperf3 \
	knot-libs openssh-client mtr socat nano \
	vim nmap iputils \
 && yum clean all
CMD bash
