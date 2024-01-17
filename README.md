# AshishKumar Token

AshishKumar Token (symbol: AKR) is a simple ERC-20 token implemented on the Ethereum blockchain. This token extends the OpenZeppelin ERC20 and ERC20Burnable contracts and includes additional ownership functionality through the Ownable contract.

## Overview

- **Token Name:** AshishKumar
- **Token Symbol:** AKR
- **Decimals:** Configurable (default: 18)

## Contracts

### `AshishKumar`

The main contract represents the AshishKumar token, implementing the ERC-20 standard. It includes basic token functionalities such as transfers and approvals.

#### Features

1. **Token Minting:** The initial token supply is minted to the contract creator (initial owner) during deployment.

### `ERC20Burnable`

This contract extends the ERC20 contract and provides additional functionality to burn (destroy) tokens.

#### Features

1. **Token Burning:** The contract allows token holders to burn (destroy) their own tokens, reducing the total token supply.

### `Ownable`

The Ownable contract is used to manage ownership of the AshishKumar token contract.

#### Features

1. **Owner Only:** Certain functions, such as token minting, can only be executed by the owner of the contract.

2. The AshishKumar token contract is deployed with an initial supply minted to the specified initial owner. The decimals parameter is set to the default value of 18.

## Token Minting

The contract owner has the ability to mint additional tokens by calling the `mint` function, providing the destination address (`to`) and the amount of tokens to be minted (`amount`).
