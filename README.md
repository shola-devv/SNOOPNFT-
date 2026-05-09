# SnoopNFT

An ERC-721 NFT smart contract built with Solidity and OpenZeppelin libraries for the SNOOP NFT collection.

## Overview

SnoopNFT is an NFT collection contract that enables minting of non-fungible tokens on the Ethereum blockchain. The contract includes enumerable support, configurable metadata, and administrative controls for managing the collection.

## Contract Details

| Property | Value |
|----------|-------|
| Name | SnoopNFT |
| Symbol | SNOOP |
| Standard | ERC-721 Enumerable |
| Max Supply | 10 NFTs |
| Mint Price | 0.01 ETH |
| Contract Address | 0x33017A80c991e707458e0163dAfC9d5B92123e4B |

## Features

- ERC721Enumerable support for token enumeration
- Mint NFTs for 0.01 ETH per transaction
- Maximum supply limit of 10 NFTs
- IPFS-based metadata support
- Pause/unpause functionality to control minting
- Owner withdrawal function for fund management

## Minting

### How to Mint

Users can mint NFTs by calling the `mint()` function. Each transaction allows minting of one NFT.

### Requirements

To successfully mint an NFT, the following conditions must be met:

- Contract must not be paused
- Correct ETH amount (0.01 ETH) must be sent with the transaction
- Total minted NFTs must not exceed the maximum supply of 10
- Token metadata must be available

### Metadata

Metadata is constructed using the following format:

```
baseURI + tokenId + ".json"
```

**Example base URI:**
```
ipfs://bafybeid2zmpbpubntnyrygvooo56q3thbcpucz77b7hgtqzgx7mbh6eoxu/
```

Metadata files are included in the repository and correspond to token IDs 1-5.

## Administrative Functions

### Pause/Unpause Minting
```
setPaused(bool val)
```
Toggle minting availability. When paused, users cannot mint new NFTs.

### Withdraw Funds
```
withdraw()
```
Transfer contract balance to the contract owner. Only callable by the owner.

## Technology Stack

- **Solidity** - Smart contract language
- **OpenZeppelin Contracts** - Standard-compliant contract implementations
- **Ethereum** - Blockchain network

## Development

This project implements the ERC-721 standard with enumerable extensions as defined by OpenZeppelin. The contract includes safety checks and owner-controlled mechanisms for managing the NFT collection lifecycle.

## License

MIT
