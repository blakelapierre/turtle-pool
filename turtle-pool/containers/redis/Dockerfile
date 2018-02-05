FROM blakelapierre/turtlepool-base

EXPOSE 8070
VOLUME daemon-data
VOLUME wallet-data

CMD cd TurtleCoin-v0.3.0-linux-static-CLI && if [ ! -f /wallet-data/container ]; then ./walletd --data-dir /wallet-data -g -w /wallet-data/container; fi; ./walletd --daemon-address turtlepool-daemon --data-dir /wallet-data -w /wallet-data/container