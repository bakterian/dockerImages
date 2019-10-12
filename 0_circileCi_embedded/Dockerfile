FROM circleci/python:3.7.1-stretch

USER root

RUN apt-get update && apt-get install jq unzip sed build-essential

RUN mkdir -p ~/workspace

RUN cd /var && wget -O YAML-1.24.tar.gz http://search.cpan.org/CPAN/authors/id/T/TI/TINITA/YAML-1.24.tar.gz

RUN cd /var && tar -xzvf YAML-1.24.tar.gz 

RUN cd /var/YAML-1.24 && perl Makefile.PL

RUN cd /var/YAML-1.24 && make

RUN cd /var/YAML-1.24 && make install
