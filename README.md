# mineonlium
This project was started with the vision of a truly fair start crypto-economy. Too many fake projects are poping up all over the place. Lets come together and build our own community without the massive whales and dev fees/pre-alloc's.


This project is highly WIP and is currently in the pre-alpha stage. Over the next few months this space will change rapidly as our project grows. 


Join the Discord! -> https://discord.gg/wt3WYhtw 

# Features

* No pre-mine
* %0 Dev fees
* %0 Pre-allocation
* %100 of mineonlium's currency is created, and owned by, the miners. 
* Free pool
* Easy solo pool setup
* ... more coming soon



# Getting Started:

## Wallet

Recomeded: Metamask

Network Name: `Mineonlium`
RPC Server: `http://34.87.231.138:8545`
Chain ID: `54321`
Currency Symbol: `MO`
Block Explorer URL: `http://134.215.244.171/dashboard`

## Community Pool

API for mining stats will be avalible soon! IF you have any issues! Reach out to us on Discord!

```
stratum+tcp://34.132.68.218:4073
```


## Solo Mining

Solo mining will be highly encouraged throughout the project and a full guide on setting up a personal stratum server for solo mining is comming soon!

for those of you that know... use besu, the genesis file below, and this bootnode := `enode://186fc7e1dc26686eaef6c9a57f33cc211650bc22b5152072f32593eb39f93ee3eb2c50e5e8d99905cd3021ff595f4c5b43a9d249d596d776649ba01f6dea8584@34.132.68.218:60606`

If you need help please reach out to me on the Discord -> https://discord.gg/wt3WYhtw

MO Genesis file
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
