FROM ubuntu
MAINTAINER reponte <qmmreponte@tip.edu.ph>

#skip prompts
ARG DEBIAN-FRONTEND=noninteractive

# update packages
RUN apt update; apt dist-upgrade

#install packages
RUN apt install -y apache2 mariadb-server

#set entrypoint
ENTRYPOINT apache2ctl -D FOREGROUND
