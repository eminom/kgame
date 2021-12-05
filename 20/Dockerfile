FROM ubuntu:20.04
ARG DEBIAN_FRONTEND=noninteractive
ENV TZ=Asia/Shanghai

MAINTAINER baihai

RUN apt update
RUN apt install -y apt-utils
RUN apt install -y build-essential
RUN apt install -y manpages-dev
RUN apt install -y gcc
RUN apt-get install -y g++
RUN apt-get install -y gdb
RUN apt install -y python3
RUN apt install -y curl
RUN apt install -y python3-distutils
RUN apt install -y python3-apt
RUN apt install -y vim
RUN apt install -y git-core
RUN apt install -y unzip
RUN apt install -y ucommon-utils

RUN curl -sSL https://bootstrap.pypa.io/get-pip.py -o get-pip.py
RUN /usr/bin/python3.8 get-pip.py

#RUN rm /usr/bin/python3
#RUN ln -s /usr/bin/python3.8 /usr/bin/python3

RUN python3 -m pip install six
RUN python3 -m pip install idna
RUN python3 -m pip install numpy
RUN python3 -m pip install pandas
RUN python3 -m pip install sklearn
RUN python3 -m pip install matplotlib
RUN python3 -m pip install notebook
RUN python3 -m pip install jupyter
RUN python3 -m pip install kaggle
RUN python3 -m pip install setuptools
RUN python3 -m pip install jupyterlab
