# Crypto Devs

Crypto Devs is a Solidity smart contract for creating non-fungible tokens (NFTs) on the Ethereum blockchain. It inherits ERC721Enumerable and Ownable contracts provided by OpenZeppelin.

CryptoDevs is a smart contract written in Solidity that implements the ERC721 standard. It allows users to mint and own unique tokens called CryptoDevs.

## Features

- Implements the ERC721 standard for non-fungible tokens (NFTs)
- Supports a presale period for whitelisted addresses
- Allows users to mint 1 NFT per transaction after the presale has ended
- Has an owner who can pause/unpause the contract and withdraw Ether from it
- Has a maximum supply of 20 NFTs
- Includes a base URI for computing token URIs

## Usage

To use CryptoDevs, you must first deploy it to the Ethereum network. Once deployed, you can interact with it using any Ethereum wallet or web3 provider.

The owner of the contract can start a presale by calling `startPresale()`. During this period, whitelisted addresses can call `presaleMint()` to mint 1 NFT per transaction. After the presale has ended, users can call `mint()` to mint 1 NFT per transaction.
The owner of the contract can pause/unpause it by calling `setPaused(bool val)` and withdraw Ether from it by calling `withdraw()`.

## Getting started

These instructions will help you to compile, deploy and test the Crypto Devs contract in your local environment and the public blockchain.

## Prerequisites

1. NodeJS
2. Hardhat Framework
3. Metamask

This project demonstrates a basic Hardhat use case. It comes with a sample contract, a test for that contract, and a script that deploys that contract.

Try running some of the following tasks:

## Cloning and Compiling with Hardhat

1. Clone the repository from Github: `git clone https://github.com/Patrick-Ehimen/NFT-Collection.git`
2. Install Hardhat: `npm install -g @nomiclabs/hardhat`
3. Install dependencies: `npm install`
4. Compile the contracts: `npx hardhat compile`
5. Deploy the contracts to the Ethereum network: `npx hardhat run scripts/deploy.js --network mumbai`

Once deployed, you can interact with it using any Ethereum wallet or web3 provider.

The owner of the contract can start a presale by calling `startPresale()`. During this period, whitelisted addresses can call `presaleMint()` to mint 1 NFT per transaction. After the presale has ended, users can call `mint()` to mint 1 NFT per transaction.
The owner of the contract can pause/unpause it by calling `setPaused(bool val)` and withdraw Ether from it by calling `withdraw()`.
