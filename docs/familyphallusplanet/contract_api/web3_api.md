---
sidebar_position: 1
---

# Web3 API

In this project we are using [ethers](https://docs.ethers.io/v5/) library.

## Get started

`>npm i ethers`

```js title="contract.js"
const { ethers } = require("ethers");

// A Web3Provider wraps a standard Web3 provider, which is
// what MetaMask injects as window.ethereum into each page
const provider = new ethers.providers.Web3Provider(window.ethereum);

// The MetaMask plugin also allows signing transactions to
// send ether and pay to change state within the blockchain.
const signer = provider.getSigner();
```
