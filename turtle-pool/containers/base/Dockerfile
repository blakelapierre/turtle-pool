FROM ubuntu

RUN apt-get update
RUN apt-get install -y wget

RUN wget https://github.com/turtlecoin/turtlecoin/releases/download/v0.3.2/turtlecoin-v0.3.2-linux-staticboost.tar.gz
RUN tar -xvzf turtlecoin-v0.3.2-linux-staticboost.tar.gz
RUN mv turtlecoin-v0.3.2 turtlecoin


CMD cd turtlecoin && ./TurtleCoind --data-dir /daemon-data