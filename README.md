# testnetfaucet

testnetfaucet is a simple web app that sends a configurable amount of testnet
HC via an hcrpcclient connection to an instance of hcwallet.

## Installation

## Developing

``` bash
git clone https://github.com/HcashOrg/testnetfaucet.git
cd testnetfaucet
dep ensure
go install
```

Start hcwallet with the following options.  

```bash
hcwallet --testnet -u USER -P PASSWORD --rpclisten=127.0.0.1:19111 --rpccert=$HOME/.hcwallet/rpc.cert
```

Configure and start testnetfaucet

```bash
mkdir ~/.testnetfaucet
cp sample-testnetfaucet.conf ~/.testnetfaucet/testnetfaucet.conf (and edit appropriately)
testnetfaucet
```

## Contact

If you have any further questions you can find us at:

- https://forum.h.cash

## Issue Tracker

The
[integrated github issue tracker](https://github.com/HcashOrg/testnetfaucet/issues)
is used for this project.

## License

testnetfaucet is licensed under the [copyfree](http://copyfree.org) ISC License.

