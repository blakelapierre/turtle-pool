FROM blakelapierre/turtlepool-base

EXPOSE 8070
VOLUME daemon-data
VOLUME wallet-data

CMD cd coin && if [ ! -f /wallet-data/container ]; then ./walletd --data-dir /wallet-data -g -w /wallet-data/container; fi; ./walletd --daemon-address turtlepool-daemon --daemon-port 11898 --data-dir /wallet-data -w /wallet-data/container