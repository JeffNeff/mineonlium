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
RPC Server: `http://34.132.68.218:8545`
Chain ID: `54321`
Currency Symbol: `MO`
Block Explorer URL: COMING BY THE END OF TODAY!!! 

## Community Pool

API for mining stats will be avalible soon! For now payouts are set to happen every 10min. with a minimum of 1MO. IF you have any issues! Reach out to us on Discord!

```
Coming soon!
```


## Solo Mining

Solo mining will be highly encouraged throughout the project and a full guide on setting up a personal stratum server for solo mining is comming soon!

for those of you that know... use besu, the genesis file below, and this bootnode := `enode://0c53a65b8b98c95698e05b62c97c180b3b6febae1d7b516e7047f7c36c373e0bbed38c2c83b2b9a264a375886fb2c6a44e26938b1bee4c8e23e788938b49e00a@134.215.244.171:60606`

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
