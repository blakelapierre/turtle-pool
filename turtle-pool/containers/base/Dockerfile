FROM ubuntu

RUN apt-get update
RUN apt-get install -y wget

RUN wget https://github.com/turtlecoin/turtlecoin/releases/download/v0.4.2/turtlecoin-v0.4.2-linux.tar.gz
RUN tar -xvf turtlecoin-v0.4.2-linux.tar.gz
RUN mkdir /coin && cp turtlecoin-v0.4.2/* /coin


CMD cd coin && ./TurtleCoind --data-dir /daemon-data