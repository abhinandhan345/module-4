# Token Smart Contract

## Introduction

This Solidity smart contract, named "Token," is designed to implement a basic ERC-20 token with additional features such as token minting, burning, and voucher redemption. The contract is built using the OpenZeppelin library, a widely used set of secure and community-reviewed smart contract components.

## Features

### ERC-20 Token Standard

The contract adheres to the ERC-20 token standard, providing the essential functionalities required for interoperability with other tokens and decentralized applications (DApps).

### Minting and Burning

The contract owner has the ability to mint new tokens and burn existing tokens. Minting creates new tokens and assigns them to a specified address, while burning removes tokens from the total supply.

### Voucher System

The contract introduces a voucher system where users can redeem discounts on token transfers based on predefined voucher types. Vouchers are initialized during contract deployment, each with a specific discount value and a limited quantity.

### Voucher Redemption

Users can redeem vouchers by specifying the voucher type and the quantity of items they want to purchase. The contract verifies the validity of the voucher, checks the availability of the required quantity, and deducts the corresponding token amount from the user's balance.

### Ownership

The contract utilizes the Ownable contract from OpenZeppelin, ensuring that certain functions, such as minting and changing voucher quantities, can only be executed by the contract owner.

## Getting Started

### Prerequisites

- Ethereum Development Environment: Ensure you have a development environment set up with Solidity compiler support (e.g., Remix, Truffle, Hardhat).

### Deployment

1. Deploy the contract on an Ethereum-compatible blockchain.
2. Upon deployment, the contract initializes four predefined vouchers with different discount levels.

## Usage

### Minting Tokens

- The contract owner can mint new tokens and assign them to a specified address using the `mintTokens` function.

### Burning Tokens

- The contract owner can burn a specified amount of tokens from their own balance using the `burnTokens` function.

### Transferring Tokens

- Users can transfer tokens to another address using the standard ERC-20 `transfer` function.

### Redeeming Vouchers

- Users can redeem vouchers by providing the voucher type and the quantity of items they want to purchase using the `redeemVoucher` function.

### Changing Voucher Quantities

- The contract owner can update the quantity of available vouchers using the `changeVoucherQuantity` function.

## Security Considerations

- Ensure that only trusted entities have ownership of the contract.
- Regularly audit and test the contract code for security vulnerabilities.

## License

This smart contract is released under the MIT License. See the [LICENSE](./LICENSE) file for details.

## Author

belgaliabhinandan@gmail.com
