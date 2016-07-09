FROM fujiwarakoubou/centos7-systemd-sshd

RUN yum -y install firewalld
RUN yum clean all

RUN firewall-cmd --permanent --zone=public --change-interface=eth0
RUN systemctl enable firewalld

CMD ["/usr/sbin/init"]