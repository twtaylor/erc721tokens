# ETH SF notes

1) Spin up own testnet
2) Create smaller application
3) Get it running

# Genesis init

> Init our genesis block

geth init Genesis.json --datadir "ethsfChain" --keystore keystore

> Attach the console

geth --nodiscover --maxpeers 1 --networkid 4444 --datadir "ethsfChain" --keystore keystore console 

> Set our etherbase

miner.setEtherbase("3a3d39d2ae53eb539b44f72f8bb13f01bd9e0f21")

> Start mining

miner.start()

# To connect to multiple nodes

geth --nodiscover --networkid 4444 --port 3000 --datadir "ethsfChain" console 

geth attach --rpcapi "db,eth,net,web3"  --identity "EthSfMain"

# Accounts (and passwords)

3a3d39d2ae53eb539b44f72f8bb13f01bd9e0f21
"wakandaforever"

12264aa620c6d67a825aa47de378f60e83179357
"never"






