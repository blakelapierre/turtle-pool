FROM ubuntu

RUN apt-get update
RUN apt-get install -y wget

RUN wget https://github.com/turtlecoin/turtlecoin/releases/download/v0.3.0/TurtleCoin-v0.3.0-linux-static-CLI.tar.gz
RUN tar -xvzf TurtleCoin-v0.3.0-linux-static-CLI.tar.gz


CMD cd TurtleCoin-v0.3.0-linux-static-CLI && ./TurtleCoind --data-dir /daemon-data