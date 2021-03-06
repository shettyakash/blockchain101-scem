# Setup the Ethereum ecosystem

The Ethereum  ecosystem can be setup locally for development purpose or we can connect to a real blockchain.
The local blockchain can be setup using an in-memory blockchain called Ganache.

Make sure that you have a latest version of `nodejs` and `npm`. Here is a [install guide](https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-16-04) for Ubuntu system.

## Install local blockchain (Ganache)

`npm install ganache-cli web3@0.20.2`


## Install mainnet/testnet blockchain client (Optional)

Mac OSX:
```
brew tap ethereum/ethereum
brew install ethereum
```

Ubuntu:

```
sudo apt-get install software-properties-common
sudo add-apt-repository -y ppa:ethereum/ethereum
sudo apt-get update
sudo apt-get install ethereum
```

## Run the Ethereum node:

```
geth --rinkeby --syncmode "fast" --rpc --rpcapi db,eth,net,web3,personal --cache=1024  --rpcport 8545 --rpcaddr 127.0.0.1 --rpccorsdomain "*"
```

# Setup a development environment

We can start the Ethereum development from scratch or use an existing framework such as truffle.
 

## Truffle framework

Truffle framework makes the development and deployment process smoother by creating a framework for development.
The the framework will help to easily create and deploy the DApp.

```
npm install -g truffle

```

## Hello World smart contract

```truffle init
   
   truffle migrate
   
   truffle console

```

## Proof of Ownership DApp

```truffle unbox react
   
   truffle migrate
   
   npm start

```