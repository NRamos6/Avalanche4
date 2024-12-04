# DegenToken

A custom ERC-20 token with integrated support for in-game items.

## Overview

**DegenToken** (`DGN`) is a smart contract built on Solidity using OpenZeppelin libraries. It supports standard ERC-20 functionality while incorporating features for managing in-game items. Ideal for gaming and blockchain applications.

## Features

- **ERC-20 Token**: Implements standard ERC-20 functionality.
- **Mintable**: Tokens can be minted by the contract owner.
- **In-game Items**:
  - **Infinity Gauntlet**: Cost 30 DGN
  - **Statikk Edge**: Cost 50 DGN
  - **Monkey King Bar**: Cost 90 DGN
- Tracks ownership of in-game items for each user.

## Contract Details

- **Token Name**: Degen
- **Token Symbol**: DGN
- **Decimals**: 18 (default)
- **Access Control**: Only the owner can mint tokens.

## Functions

### ERC-20 Functions
- `mint(address to, uint256 amount)`: Allows the owner to mint tokens to a specified address.
- `decimals()`: Returns the number of token decimals (fixed at 18).

### Game Item Management
- `purchaseItem(uint256 itemId)`: Allows users to purchase in-game items using `DGN` tokens.
- `getOwnedItems(address owner)`: Retrieves the list of in-game items owned by an address.

## Requirements

- **Solidity**: `^0.8.18`
- **Dependencies**: [OpenZeppelin Contracts](https://openzeppelin.com/contracts/)

## License

This project is licensed under the MIT License.
