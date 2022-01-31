<p align="center">
  <img src="./images/script-logo.jpg" alt="logo" height="200"/>
</p>

[![Build Status](https://travis-ci.org/murray-distributed-technologies/bitcoinscript.png?branch=master)](https://travis-ci.org/murray-distributed-technologies/bitcoinscript)
[![ISC License](http://img.shields.io/badge/license-ISC-blue.svg)](http://copyfree.org)
[![GoDoc](https://godoc.org/github.com/murray-distributed-technologies/bitcoinscript?status.png)](http://godoc.org/github.com/murray-distributed-technologies/bitcoinscript)

Package bitcoinscript implements the bitcoin transaction script language.  There is
a comprehensive test suite.

This package has intentionally been designed so it can be used as a standalone
package for any projects needing to use or validate bitcoin transaction scripts.

## Bitcoin Scripts

Bitcoin provides a stack-based, FORTH-like language for the scripts in
the bitcoin transactions.  This language is not turing complete
although it is still fairly powerful.  A description of the language
can be found at https://en.bitcoin.it/wiki/Script

## Installation and Updating

```bash
$ go get -u github.com/murray-distributed-technologies/bitcoinscript
```

## Examples

* [Standard Pay-to-pubkey-hash Script](http://godoc.org/github.com/murray-distributed-technologies/bitcoinscript#example-PayToAddrScript)  
  Demonstrates creating a script which pays to a bitcoin cash address.  It also
  prints the created script hex and uses the DisasmString function to display
  the disassembled script.

* [Extracting Details from Standard Scripts](http://godoc.org/github.com/murray-distributed-technologies/bitcoinscript#example-ExtractPkScriptAddrs)  
  Demonstrates extracting information from a standard public key script.

* [Manually Signing a Transaction Output](http://godoc.org/github.com/murray-distributed-technologies/bitcoinscript#example-SignTxOutput)  
  Demonstrates manually creating and signing a redeem transaction.

## License

Package bitcoinscript is licensed under the [copyfree](http://copyfree.org) ISC
License.
