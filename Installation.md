# Installation (Mac OSX) [](https://www.ethereum.org/cli)
Assume pre-exsisting Homebrew installation
* brew tap ethereum/ehtereum
* brew install ethereum

# Create private Ehereum chain
Follow http://adeduke.com/2015/08/how-to-create-a-private-ethereum-chain/

````
geth --genesis ethereumGenesisTest.json --datadir data --networkid 543 --nodiscover --maxpeers 0 console
````

````
> personal.newAccount("password")
"0x7fa91c044d6019d98ee1fef31c78e5cf6deb5e6f"
````

Final genesis block with initial account and allocation.
````
{
	"nonce": "0xdeadbeefdeadbeef",
	"timestamp": "0x0",
	"parentHash": "0x0000000000000000000000000000000000000000000000000000000000000000",
	"extraData": "0x0",
	"gasLimit": "0x8000000",
	"difficulty": "0x400",
	"mixhash": "0x0000000000000000000000000000000000000000000000000000000000000000",
	"coinbase": "0x3333333333333333333333333333333333333333",
	"alloc": {
		"0x7fa91c044d6019d98ee1fef31c78e5cf6deb5e6f": {
			"balance": "10000000000000000000"
		}
	}
}
````
