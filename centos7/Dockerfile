FROM centos:7

RUN yum -y install epel-release \
    && yum repolist \
    && yum -y update

RUN yum -y install \
        tar unzip iproute net-tools rsync \
        tcpdump telnet traceroute curl iperf3 \
        knot-libs openssh-client mtr socat nano \
        vim nmap iputils tree dhclient \
        rdate wget psmisc www-libperl-www lsof

RUN yum clean all

COPY src/etc/sysconfig/network-scripts/ifcfg-eth0 /etc/sysconfig/network-scripts/
COPY src/root/.vimrc /root/
COPY src/root/.bashrc /root/

CMD bash
