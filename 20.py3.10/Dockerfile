FROM ubuntu:20.04
ARG DEBIAN_FRONTEND=noninteractive
ENV TZ=Asia/Shanghai

MAINTAINER baihai

RUN apt update -y
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
RUN apt install -y sudo
RUN apt install -y tree
RUN apt install -y ucommon-utils
RUN apt install -y systemd-tests


# Install Python3.10
RUN apt install -y software-properties-common
RUN add-apt-repository -y ppa:deadsnakes/ppa
RUN apt install -y python3.10

RUN curl -sSL https://bootstrap.pypa.io/get-pip.py -o get-pip.py
RUN /usr/bin/python3.10 get-pip.py

RUN rm /usr/bin/python3
RUN ln -s /usr/bin/python3.10 /usr/bin/python3

RUN python3 -m pip install six
RUN python3 -m pip install idna
RUN python3 -m pip install numpy
RUN python3 -m pip install pandas
RUN python3 -m pip install scikit-learn
RUN python3 -m pip install matplotlib
RUN python3 -m pip install notebook
RUN python3 -m pip install jupyter
RUN python3 -m pip install kaggle
RUN python3 -m pip install setuptools
RUN python3 -m pip install jupyterlab
RUN python3 -m pip install opencv-python
RUN python3 -m pip install xgboost
RUN apt install -y libgl1-mesa-glx
