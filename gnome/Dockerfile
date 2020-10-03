FROM dopcode/centos7
RUN yum -y group install "Server with GUI"
RUN yum -y group install "GNOME Desktop"
USER root
COPY Xwrapper.config /etc/X11/
CMD startx
