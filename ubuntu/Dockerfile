FROM ubuntu:bionic
RUN apt-get update \
    && apt-get -y --no-install-recommends install \
        tar unzip iproute2 net-tools \
        tcpdump telnet traceroute curl iperf3 \
        knot-host openssh-client mtr-tiny socat nano \
        vim-tiny nmap iputils-ping rdate \
    && rm -rf /var/lib/apt/lists/*
CMD bash
