# Candy Machine UI for NFT Minting

This repository contains the setup guide and resources to create a user interface (UI) for minting NFTs using a Candy Machine powered by an SPL token. This UI enables users to mint NFTs by connecting their Phantom wallets.

## Description

This guide walks you through the step-by-step process of setting up the Candy Machine UI. It assumes you have already configured a Candy Machine and created an SPL token. The UI allows users to mint NFTs by paying with the SPL token through their Phantom wallets.

## Prerequisites

Ensure you have the following before proceeding:

- A configured Candy Machine with details in the `config.json` file.
- An existing SPL token.
- A Phantom wallet for minting.

## Setup Steps

### 1. Set Up the SPL Token

If you haven't already, create the SPL token following guidelines from Lesson Three. Note down the SPL token's address.

### 2. Update Candy Machine Config

- Update `splTokenAccount` with the SPL token account address.
- Update `splToken` with the SPL token address in the `config.json` file.

### 3. Set Up the UI

Follow the steps from the "Quick Node: Set Up a Minting Site" tutorial to create a UI for your Candy Machine. This UI facilitates NFT minting via Phantom wallets using the SPL token.

### 4. Modify Minting Logic

Adjust the minting logic in your SPL project to direct minted NFTs to the Phantom wallet address instead of `fromWallet`. Alternatively, modify the transfer function to send NFTs to your Phantom wallet.

### 5. Testing

Test the setup by transferring or minting your SPL token to a Phantom account. Use the created UI to ensure users can successfully mint NFTs by paying with the configured SPL token.

## Authors

- **Subran**

## Resources

- [The SPL Token Program by MetaCrafters](https://github.com/Metacrafters/Module2-create-spl-token-js.git)
- Ensure addresses and token details in `config.json` match those created.

**Note:** Provide clear instructions in your UI for users to connect their Phantom wallets and mint NFTs. Include troubleshooting tips and potential issues users might encounter during the setup process.

Feel free to contribute, report issues, or suggest improvements to this repository!
