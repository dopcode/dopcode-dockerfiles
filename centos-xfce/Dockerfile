#FROM centos:7
FROM dopcode/centos

#RUN yum clean all
#RUN yum -y update
#RUN yum -y install epel-release




#RUN yum -y install x11vnc firefox xorg-x11-server-Xvfb xorg-x11-twm tigervnc-server xterm xorg-x11-font dejavu-sans-fonts dejavu-serif-fonts xdotool; yum clean all
RUN yum -y group install "Server with GUI" "Xfce"
#RUN yum -y group install "X Window System"
#RUN yum -y group install "GNOME"
#RUN yum -y group install "Xfce"
#RUN yum -y install firefox




#RUN yum clean all

# Add the xstartup file into the image
#ADD ./xstartup /

#RUN mkdir /.vnc
#RUN x11vnc -storepasswd 123456 /.vnc/passwd
#RUN  \cp -f ./xstartup /.vnc/.
#RUN chmod -v +x /.vnc/xstartup
#RUN sed -i '/\/etc\/X11\/xinit\/xinitrc-common/a [ -x /usr/bin/firefox ] && /usr/bin/firefox &' /etc/X11/xinit/xinitrc

#EXPOSE 5901

#CMD    ["vncserver", "-fg" ]
# ENTRYPOINT ["vncserver", "-fg" ]

#CMD firefox


#RUN systemctl set-default graphical.target


#USER root

#RUN adduser dopcode
#RUN passwd -d dopcode
#USER dopcode



#CMD gnome-session & gnome-panel & gnome-terminal &
#CMD gnome-panel & gnome-session & gnome-menu & gnome-manager & gnome-terminal & gnome-settings-daemon & metacity & nautilus

CMD startxfce4
