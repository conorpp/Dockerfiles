FROM ubuntu:14.04
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update -y
RUN apt-get install -y weechat tor wget
RUN wget https://github.com/conorpp/Dockerfiles/raw/master/Weechat_Tor/weechat.tar
RUN tar xvf weechat.tar -C ~
CMD /etc/init.d/tor start && bash -c "weechat --run-command '/connect oftc'"


MAINTAINER Conor Patrick
