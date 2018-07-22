# Bitcore-Alarmx

[![NPM Package](https://img.shields.io/npm/v/bitcore-alarmx.svg?style=flat-square)](https://www.npmjs.org/package/bitcore-alarmx)
[![Build Status](https://img.shields.io/travis/alarmxcore/bitcore-alarmx.svg?branch=master&style=flat-square)](https://travis-ci.org/alarmxcore/bitcore-alarmx)

Infrastructure to build Alarmx and blockchain-based applications for the next generation of financial technology.

**Note:** If you're looking for the Bitcore-Alarmx Library please see: https://github.com/alarmxcore/bitcore-lib-alarmx

## Getting Started

Before you begin you'll need to have Node.js v4+ installed. There are several options for installation. One method is to use [nvm](https://github.com/creationix/nvm) to easily switch between different versions, or download directly from [Node.js](https://nodejs.org/).

```bash
npm install -g bitcore-alarmx
```

Spin up a full node and join the network:

```bash
npm install -g bitcore-alarmx
bitcored
```

You can then view the Insight block explorer at the default location: `http://localhost:3001/insight`, and your configuration file will be found in your home directory at `~/.bitcore`.

Create a transaction:
```js
var bitcore = require('bitcore-alarmx');
var transaction = new bitcore.Transaction();
var transaction.from(unspent).to(address, amount);
transaction.sign(privateKey);
```

## Applications

- [Node-Alarmx](https://github.com/alarmxcore/bitcore-node-alarmx) - A full node with extended capabilities using Alarmx Core
- [Insight API-Alarmx](https://github.com/alarmxcore/insight-api-alarmx) - A blockchain explorer HTTP API
- [Insight UI-Alarmx](https://github.com/alarmxcore/insight-ui-alarmx) - A blockchain explorer web user interface
- [Wallet Service](https://github.com/alarmxcore/bitcore-wallet-service-alarmx) - A multisig HD service for wallets
- [Wallet Client](https://github.com/alarmxcore/bitcore-wallet-client-alarmx) - A client for the wallet service
- CLI Wallet - A command-line based wallet client
- Angular Wallet Client - An Angular based wallet client
- Copay - An easy-to-use, multiplatform, multisignature, secure Alarmx wallet

## Libraries

- [Lib-Alarmx](https://github.com/alarmxcore/bitcore-lib-alarmx) - All of the core Alarmx primatives including transactions, private key management and others
- Payment Protocol - A protocol for communication between a merchant and customer
- [P2P-Alarmx](https://github.com/alarmxcore/bitcore-p2p-alarmx) - The peer-to-peer networking protocol
- [Mnemonic-Alarmx](https://github.com/alarmxcore/bitcore-mnemonic-alarmx) - Implements mnemonic code for generating deterministic keys
- Channel - Micropayment channels for rapidly adjusting Alarmx transactions
- [Message-Alarmx](https://github.com/alarmxcore/bitcore-message-alarmx) - Alarmx message verification and signing
- [ECIES-Alarmx](https://github.com/alarmxcore/bitcore-ecies-alarmx) - Uses ECIES symmetric key negotiation from public keys to encrypt arbitrarily long data streams.

## Documentation

The complete docs are hosted here: [bitcore documentation](http://bitcore.io/guide/). There's also a [bitcore API reference](http://bitcore.io/api/) available generated from the JSDocs of the project, where you'll find low-level details on each bitcore utility.

- [Read the Developer Guide](http://bitcore.io/guide/)
- [Read the API Reference](http://bitcore.io/api/)

To get community assistance and ask for help with implementation questions, please use our [community forums](http://bitpaylabs.com/c/bitcore).

## Security

We're using Bitcore in production, as are [many others](http://bitcore.io#projects), but please use common sense when doing anything related to finances! We take no responsibility for your implementation decisions.

If you find a security issue, please email security@bitpay.com.

## Contributing

Please send pull requests for bug fixes, code optimization, and ideas for improvement. For more information on how to contribute, please refer to our [CONTRIBUTING](https://github.com/alarmxcore/bitcore-alarmx/blob/master/CONTRIBUTING.md) file.

This will generate files named `bitcore.js` and `bitcore.min.js`.

## License

Released under the MIT license, under the same terms as AlarmxCore itself. See [LICENSE](LICENSE) for more info.
