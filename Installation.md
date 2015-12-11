# Installation (Mac OSX) [](https://www.ethereum.org/cli)
Assume pre-exsisting Homebrew installation
* brew tap ethereum/ehtereum
* brew install ethereum
* 

# Create private Ehereum chain
Follow http://adeduke.com/2015/08/how-to-create-a-private-ethereum-chain/
* ```geth --genesis ethereumGenesisTest.json --datadir data --networkid 543 --nodiscover --maxpeers 0 console```


* [Create genesis block](https://forum.ethereum.org/discussion/2757/genesis-block-in-private-network)
  * Download [sample genesis block](http://jev.io/example_genesis.json)
  * Modify to add initial allocation entries
  * Final file:
    ```
{
nonce: "0xdeadbeefdeadbeef",
timestamp: "0x0",
parentHash: "0x0000000000000000000000000000000000000000000000000000000000000000",
extraData: "0x686f727365",
gasLimit: "0x8000000",
difficulty: "0x400",
mixhash: "0x0000000000000000000000000000000000000000000000000000000000000000",
coinbase: "0x3333333333333333333333333333333333333333",
alloc: { }
}
    ```