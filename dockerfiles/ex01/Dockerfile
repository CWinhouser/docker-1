FROM debian

MAINTAINER kylet <ktwomey@student.wethinkcode.co.za>

ENV TS3SERVER_LICENSE=accept

WORKDIR /home/teamspeak

EXPOSE 9987/udp 10011 30033

RUN apt-get update && apt-get upgrade -y \
apt-get install -y wget bzip2 \
wget http://dl.4players.de/ts/releases/3.7.1/teamspeak3-server_linux_amd64-3.7.1.tar.bz2 \
tar -vf teamspeak3-server_linux_amd64-3.7.1.tar.bz2

WORKDIR teamspeak3-server_linux_amd64

ENTRYPOINT ["/start.sh"]