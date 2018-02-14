FROM ubuntu:14.04

RUN apt-get update && apt-get install -y git build-essential redis-server libboost1.55-all-dev nodejs-dev nodejs-legacy npm cmake libssl-dev

RUN git clone https://github.com/blakelapierre/turtle-pool

RUN cd turtle-pool && npm update

EXPOSE 8117
EXPOSE 3333

ADD config.json /turtle-pool/config.json

CMD cd turtle-pool/turtle-pool && node init.js