# Blockchain Todo List

Simple and secure todo list powered by smart contracts.

## New Technologies:
* [Solidity](https://docs.soliditylang.org/en/v0.5.3/) - High-level language for implementing Smart Contracts 
* [Truffle Framework](https://www.trufflesuite.com/truffle) - Ethereum DApps 
* [Ganache](https://www.trufflesuite.com/ganache) - Personal Ethereum blockchain on your local machine
* [Metamask](https://metamask.io/) Ethereum Wallet - Chrome Extension 
* [web3.js](https://web3js.readthedocs.io/en/v1.3.4/) - Library for interacting with Ethereum blockchain 
* [Node.js](https://nodejs.org/en/)

## Deployment 
1. Install Metamask browser extension to securely connect to Ethereum blockchain. <br>Metamask allows for managing our personal account when connecting to the blockchain, as well as manage ETH funds needed to pay for transactions. 
2. Install Ganache to set up our own blockchains that we will use to secure the todo list items. Its a Local development blockchain used to mimic the behavior of a public blockchain. Allows for deploying smart contracts, develop applications, and run tests.
3. Install nodejs and npm.
4. Configure npm to work without sudo:
> 1. Create a directory for global packages

```sh
mkdir "${HOME}/.npm-packages"
```

> 2. Tell `npm` where to store globally installed packages

```sh
npm config set prefix "${HOME}/.npm-packages"
```

> 3. Ensure `npm` will find installed binaries and man pages

Add the following to your `.bashrc`/`.zshrc`:

```sh
NPM_PACKAGES="${HOME}/.npm-packages"

export PATH="$PATH:$NPM_PACKAGES/bin"

# Preserve MANPATH if you already defined it somewhere in your config.
# Otherwise, fall back to `manpath` so we can inherit from `/etc/manpath`.
export MANP
5. Other deployment steps:
```bash
# Installing dependencies 
$ npm install -g truffle@5.0.2
$ npm install
# Migrate the smart contract 
truffle migrate --reset
# Run the app
$ npm run dev
```
