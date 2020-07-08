FROM ubuntu:18.04
RUN apt update &&  apt remove python2.7 && apt autoremove && apt install -y wget python3 perl g++ make libboost-all-dev zlib1g-dev python3-setuptools language-pack-en 
RUN wget https://github.com/ablab/quast/releases/download/quast_5.1.0rc1/quast-5.1.0rc1.tar.gz
RUN tar xzvf quast-5.1.0rc1.tar.gz
ENV LC_CTYPE en_US.UTF-8
WORKDIR quast-5.1.0rc1
RUN python3 setup.py install
