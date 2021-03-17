FROM rocker/verse:3.6.3


## Install CyVerse VICE Depends

RUN apt-get update && apt-get install -y lsb-release wget apt-transport-https python2.7 python-requests curl supervisor nginx gnupg2 libfuse2 nano htop


RUN curl "http://ftp.se.debian.org/debian/pool/main/o/openssl/libssl1.0.0_1.0.1t-1+deb8u8_amd64.deb" -O && \

    dpkg -i libssl1.0.0_1.0.1t-1+deb8u8_amd64.deb && \

    rm libssl1.0.0_1.0.1t-1+deb8u8_amd64.deb


### iCommands

RUN wget https://files.renci.org/pub/irods/releases/4.1.10/ubuntu14/irods-icommands-4.1.10-ubuntu14-x86_64.deb && dpkg -i *.deb
