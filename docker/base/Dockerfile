FROM ubuntu

MAINTAINER Todd Garza "todd.garza@gmail.com"

# The env variable DEBIAN_FRONTEND=noninterctive suprresses unneeded warnings:
# http://askubuntu.com/questions/506158/unable-to-initialize-frontend-dialog-when-using-ssh
ENV DEBIAN_FRONTEND=noninteractive

RUN printf "\nPROVISION 1: UPDATING DEBIAN AND INSTALLING PACKAGES\n" && \
    apt-get update && \
    apt-get install -y \
    build-essential \
    libssl-dev \
    libffi-dev \
    libreadline-dev \ 
    libbz2-dev \ 
    libsqlite3-dev \
    libncurses5-dev \ 
    python-pip \ 
    python-dev

RUN pip install crossbar[all]
