# Med-Auth

Commands to run:
1. cd minor3
2. ../bin/cryptogen generate --config=./crypto-config.yaml
3. export FABRIC_CFG_PATH=$PWD
4. ../bin/configtxgen -profile ThreeOrgsOrdererGenesis -channelID byfn-sys-channel -outputBlock ./channel-artifacts/genesis.block
5. export CHANNEL_NAME=basicchannel  && ../bin/configtxgen -profile TwoOrgsChannel -outputCreateChannelTx ./channel-artifacts/channel.tx -channelID $CHANNEL_NAME

Upcoming work:
1. Creating docker and docker-compose files to be able to run network
2. Creation of ledger for each peer
3. CouchDB configuration
4. Smart contracts
