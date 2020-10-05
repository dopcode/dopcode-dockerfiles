FROM centos:7
RUN yum clean all \
        && yum -y install epel-release \
        && yum repolist \
        && yum -y update \
        && yum -y install \
	        initscripts tar unzip iproute net-tools \
	        tcpdump telnet traceroute curl iperf3 \
	        knot-libs openssh-client mtr socat nano \
	        vim nmap iputils tree dhcp* dhclient \
        && yum clean all
COPY src/etc/sysconfig/network /etc/sysconfig/
COPY src/etc/sysconfig/network-script/ifcfg-eth* /etc/sysconfig/network-script/
CMD bash
