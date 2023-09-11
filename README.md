## Wod Chain Project

Official Golang implementation of the WodChain protocol.

This project was forked from the  go-ethereum. And made a lot of changes  to work with wodchain.

And We are working on.

Automated builds are available for stable releases and the unstable master branch. Binary
archives are published at https://www.wod.ai/download.

## Building the source

Building `gwod` requires both a Go (version 1.17 or later)  . You can install
them using your favourite package manager. Once the dependencies are installed, run

```shell
cd cmd
cd gwod
go build
```



## Executables

The gwod programe is Our main wodchain CLI client. It is the entry point into the wod network , capable of running as a full node (default), archive node (retaining all historical state) or a light node (retrieving data live).  

You can run it as a node to sync and query chain-data for the wodchain.

Use this genesis file.

```
{
  "config": {
    "chainId": 787878,
    "homesteadBlock": 0,
    "eip150Block": 0,
    "eip150Hash": "0x0000000000000000000000000000000000000000000000000000000000000000",
    "eip155Block": 0,
    "eip158Block": 0,
    "byzantiumBlock": 0,
    "constantinopleBlock": 0,
    "petersburgBlock": 0,
    "istanbulBlock": 0,
    "clique": {
      "period": 3,
      "epoch": 30000
    }
  },
  "nonce": "0x0",
  "timestamp": "0x6348ebfe",
  "extraData": "0x000000000000000000000000000000000000000000000000000000000000000074c33a57ddc9b497a04c9bb719ea5f208cce99360000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000",
  "gasLimit": "0xffffffff",
  "difficulty": "0x1",
  "mixHash": "0x0000000000000000000000000000000000000000000000000000000000000000",
  "coinbase": "0x0000000000000000000000000000000000000000",
  "alloc": {
    "0xe90920E2cCaa9603694fb479441773D614dA083b": {
      "balance": "0x19d971e4fe8401e74000000"
    }
  },
  "number": "0x0",
  "gasUsed": "0x0",
  "parentHash": "0x0000000000000000000000000000000000000000000000000000000000000000",
  "baseFeePerGas": null
}
```



Forgenet connect only import the belivable nodes.To do our  AI transformer work to mine out.

Need at least  8 * A100 to  run as a  POC miner