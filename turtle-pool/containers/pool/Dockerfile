FROM ubuntu:14.04

RUN apt-get update && apt-get install -y git build-essential redis-server libboost1.55-all-dev nodejs-dev nodejs-legacy npm cmake libssl-dev

RUN git clone https://github.com/turtlecoin/turtle-pool
RUN cd turtle-pool && git reset --hard f8a9689

RUN cd turtle-pool && npm update

EXPOSE 8117
EXPOSE 3333

ADD config.json /turtle-pool/config.json

CMD cd turtle-pool && node init.js