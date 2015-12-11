# Installation (Mac OSX) [](https://www.ethereum.org/cli)
Assume pre-exsisting Homebrew installation
* brew tap ethereum/ehtereum
* brew install ethereum
* 

# Create private Ehereum chain
Follow http://adeduke.com/2015/08/how-to-create-a-private-ethereum-chain/

````
geth --genesis ethereumGenesisTest.json --datadir data --networkid 543 --nodiscover --maxpeers 0 console
````

````
> personal.newAccount("password")
"0x7fa91c044d6019d98ee1fef31c78e5cf6deb5e6f"
````

* [Create genesis block](https://forum.ethereum.org/discussion/2757/genesis-block-in-private-network)
  * Download [sample genesis block](http://jev.io/example_genesis.json)
