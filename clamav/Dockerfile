FROM docker.io/centos:centos7.9.2009
RUN rm -rf /etc/yum.repos.d/*.repo; \
    curl -o /etc/yum.repos.d/CentOS-Base.repo https://mirrors.tencent.com/repo/centos7_base.repo ;\
    curl -o /etc/yum.repos.d/epel.repo https://mirrors.tencent.com/repo/epel-7.repo  ;\
    yum clean all && yum makecache; \
    yum install -y clamav clamd clamav-update && freshclam
