# mineonlium solo node 


Install besu 

```
sudo ufw allow 60606
sudo apt-get update
sudo apt-get install default-jdk unzip
wget https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.7.4/besu-22.7.4.zip
unzip besu-22.7.4.zip
cd besu-22.7.4/bin
export PATH=$PWD:$PATH
```


set up a working directory and create the gensis file

```
cd
mkdir EVMProtocol
cd EVMProtocol
nano genesis.json
```

paste the following:

```
{
    "config": {
    "chainId": 54321,
    "homesteadBlock": 1,
    "eip150Block": 2,
    "eip150Hash": "0x0000000000000000000000000000000000000000000000000000000000000000",
    "eip155Block": 2,
    "eip158Block": 3,
    "byzantiumBlock": 4,
    "constantinopleBlock": 5,
    "petersburgBlock": 6,
    "blockreward": "20000000000000000",
    "berlinBlock": 7,
    "muirglacierblock": 8,
    "ethash": {
        "difficulty": 10
  }
    },
    "nonce": "0x0000000000000042",
    "timestamp": "0x632AB901",
    "extraData": "0x0000000000000000000000000000000000000000000000000000000000000000",
    "gasLimit": "0x5B8D80", 
    "difficulty": "0xA",
    "mixHash": "0x63746963616c2062797a616e74696e65206661756c7420746f6c6572616e6365",
    "coinbase": "0x0000000000000000000000000000000000000000",
    "number": "0x0",
    "gasUsed": "0x0",
    "parentHash": "0x0000000000000000000000000000000000000000000000000000000000000000"
}

```

( to save and quit nano: `ctrl + s, enter, ctrl + x, enter`)

start the node. note these flags expect port 60606 and 8545 are open for p2p and rpc respectively.

```
nohup /home/user/besu-22.7.4/bin/besu --data-path=data --bootnodes=enode://186fc7e1dc26686eaef6c9a57f33cc211650bc22b5152072f32593eb39f93ee3eb2c50e5e8d99905cd3021ff595f4c5b43a9d249d596d776649ba01f6dea8584@34.132.68.218:60606 --genesis-file=genesis.json --miner-stratum-enabled --miner-stratum-host=0.0.0.0 --miner-stratum-port=50001 --miner-enabled=true --miner-coinbase=0x5bbfa5724260Cb175cB39b24802A04c3bfe72eb3 --rpc-http-host=0.0.0.0  --rpc-http-enabled=true  &
```


**NOTE** If installing on HIVE OS you can add the following to the `xinit.user.sh` file in your $HOME to auto start the node when the rig starts
```
cd /home/user/EVMProtocol && nohup /home/user/besu-22.7.4/bin/besu  --data-path=data --bootnodes=enode://186fc7e1dc26686eaef6c9a57f33cc211650bc22b5152072f32593eb39f93ee3eb2c50e5e8d99905cd3021ff595f4c5b43a9d249d596d776649ba01f6dea8584@34.132.68.218:60606 --genesis-file=genesis.json --miner-stratum-enabled --miner-stratum-host=0.0.0.0 --miner-stratum-port=50001 --miner-enabled=true --miner-coinbase=0x5bbfa5724260Cb175cB39b24802A04c3bfe72eb3 --rpc-http-host=0.0.0.0  --rpc-http-enabled=true  &
```

