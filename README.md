BIP39 Mnemonics for Bitcore-Finite
=======

[![NPM Package](https://img.shields.io/npm/v/bitcore-mnemonic-finite.svg?style=flat-square)](https://www.npmjs.org/package/bitcore-mnemonic-finite)
[![Build Status](https://img.shields.io/travis/finitecoin/bitcore-mnemonic-finite.svg?branch=master&style=flat-square)](https://travis-ci.org/finitecoin/bitcore-mnemonic-finite)
[![Coverage Status](https://img.shields.io/coveralls/finitecoin/bitcore-mnemonic-finite.svg?style=flat-square)](https://coveralls.io/r/finitecoin/bitcore-mnemonic-finite)

A module for [bitcore-finite](https://github.com/finitecoin/bitcore-finite) that implements [Mnemonic code for generating deterministic keys](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki).

## Getting Started

This library is distributed in both the npm and bower packaging systems.

```sh
npm install bitcore-mnemonic-finite
bower install bitcore-mnemonic-finite
```

There are many examples of how to use it on the developer guide [section for mnemonic](http://bitcore.io/guide/module/mnemonic/index.html). For example, the following code would generate a new random mnemonic code and convert it to a `HDPrivateKey`.

```javascript
var Mnemonic = require('bitcore-mnemonic-finite');
var code = new Mnemonic(Mnemonic.Words.SPANISH);
code.toString(); // natal hada sutil año sólido papel jamón combate aula flota ver esfera...
var xpriv = code.toHDPrivateKey();
```

## Contributing

See [CONTRIBUTING.md](https://github.com/finitecoin/bitcore-finite/blob/master/CONTRIBUTING.md) on the main bitcore-finite repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/bitpay/bitcore/blob/master/LICENSE).

Copyright 2013-2015 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.
