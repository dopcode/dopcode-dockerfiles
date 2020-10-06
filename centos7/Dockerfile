FROM centos:7

RUN yum -y install epel-release \
        && yum repolist \
        && yum -y update \
        && yum -y group install "Minimal Install" \
        && yum clean all

COPY src/etc/sysconfig/network /etc/sysconfig/
COPY src/etc/sysconfig/network-scripts/ifcfg-eth0 /etc/sysconfig/network-scripts/

CMD bash
