# Supply-Chain

Commands to run:
1. cd minor3
2. ../bin/cryptogen generate --config=./crypto-config.yaml
3. export FABRIC_CFG_PATH=$PWD
4. ../bin/configtxgen -profile TwoOrgsOrdererGenesis -channelID byfn-sys-channel -outputBlock ./channel-artifacts/genesis.block
5. export CHANNEL_NAME=basicchannel  && ../bin/configtxgen -profile TwoOrgsChannel -outputCreateChannelTx ./channel-artifacts/channel.tx -channelID $CHANNEL_NAME