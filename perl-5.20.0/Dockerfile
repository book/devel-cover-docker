FROM ubuntu:latest

MAINTAINER Paul Johnson <paul@pjcj.net>

ENV TERM xterm

RUN apt-get update && apt-get -y install wget build-essential

WORKDIR /usr/local/src
RUN wget http://www.cpan.org/src/5.0/perl-5.20.0.tar.gz -O - | tar xzf -
RUN cd perl-5.20.0 && ./Configure -des && make install
