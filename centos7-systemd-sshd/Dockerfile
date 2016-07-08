FROM fujiwarakoubou/centos7-systemd

RUN yum -y install openssh-server
RUN yum -y install firewalld
RUN yum clean all
RUN systemctl enable sshd
RUN systemctl enable firewalld

CMD ["/usr/sbin/init"]