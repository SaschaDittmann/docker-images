FROM centos:latest
MAINTAINER info@bytesmith.de
ADD http://aka.ms/rclientlinux /tmp/microsoft-r-client.tar.gz
RUN yum clean all \
	&& cd /tmp \
	&& tar zxvf microsoft-r-client.tar.gz \
    && cd /tmp/MRC_Linux \
    && ./install.sh -a -s -m \ 
    && rm -rf /tmp/MRC_Linux/ \ 
    && rm -rf /tmp/microsoft-r-client.tar.gz
ENTRYPOINT ["Revo64"]