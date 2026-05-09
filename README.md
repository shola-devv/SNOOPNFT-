# SnoopNFT

SnoopNFT is a minimal ERC-721 NFT contract built with Solidity and OpenZeppelin.

## Features

- ERC721Enumerable support
- Mint NFTs for `0.01 ETH`
- Max supply of `10 NFTs`
- IPFS metadata support
- Pause/unpause minting
- Owner withdrawal function

## Contract Details

- Name: `SnoopNFT`
- Symbol: `SNOOP`
- Max Supply: `10`
- Mint Price: `0.01 ETH`

## Mint

Users can mint one NFT per transaction: mint()

## Requirements

-Contract must not be paused
-Correct ETH amount must be sent
-Max supply must not be exceeded
-Metadata

## Metadata is generated using:

baseURI + tokenId + ".json"

-Example: ipfs://bafybeid2zmpbpubntnyrygvooo56q3thbcpucz77b7hgtqzgx7mbh6eoxu/

-metadata files are included in the folder, named 1-5


## Owner Functions
-Pause / Unpause: setPaused(bool val)
-Withdraw Contract Funds: withdraw()

##  conract Address 

0x33017A80c991e707458e0163dAfC9d5B92123e4B

## Built With

Solidity
OpenZeppelin Contracts

## License

MIT



