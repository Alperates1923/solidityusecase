# NFT Minter dApp

## Summary
This project was developed within the scope of the Softtech Solidity Development Program.
With this dApp, users can mint their own NFTs.

# Details

* Application has mainly 4 components. Namely, a React frontend (running on port 3000), an Express backend (running on port 5000), Pinata service for IPFS in order to store binary data off-chain and Sepolia Testnet for Ethereum Blockchain.

* NFT contract created on ERC 721 standard using Solidity via Remix IDE. NFT Contract deployed on Sepolia Testnet. You can find source code of contract in the contracts directory.

Contract address:
```python
0x98d4f97e3874e2d471911981c87e8ffe585a0fe6
```

* There is two components in the UI, Connect to wallet button & NFT Minter form. NFT Minter form displayed after wallet connection. (Tested with MetaMask)

* NFT minter form contains a general info section, meta-data section, and price input section.

* After entering name and uploading NFT file mint button is enabled, these two are required. NFT file and metadata are persisted on IPFS.

* There are 2 wallets in order to build some basic tokenomics:

Liquidity wallet:
```python
0x67934BeFa1f855DF1Ae2F1E89540523eF273f4E6
```

Treasury wallet:
```python
0x71c3b35DfC353a2e544856b89D54067Cb96AB543
```

%10 of the price is royalty fee. When the user mint the NFT, 6% will be transferred to the treasury wallet, 4% to the liquidity wallet.

## Starting Application

To start use the following command in the project directory (./ in the begining of the command is for Linux).

```bash
./start.sh
```
## Exploring NFT

You can explore NFT's by following links:

<a href="https://testnets.opensea.io/collection/nftminter-35">NFT Minter on OpenSea (Testnets)</a>