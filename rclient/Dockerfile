FROM centos:latest
MAINTAINER info@bytesmith.de
ADD http://aka.ms/rclientlinux /tmp/
RUN yum clean all \
    && cd /tmp/MRC_Linux \
    && ./install.sh -a -s -m \ 
    && rm -rf /tmp/MRC_Linux/
ENTRYPOINT ["Revo64"]