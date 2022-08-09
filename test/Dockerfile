FROM continuumio/miniconda3:latest
RUN apt update
RUN apt-get clean
RUN apt install -y locales
RUN locale -a && locale
RUN sed -i "s/# en_GB.UTF-8 UTF-8/en_GB.UTF-8 UTF-8/" /etc/locale.gen
RUN locale-gen
RUN locale -a && locale
