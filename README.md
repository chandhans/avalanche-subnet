# Readme for Vault Contract

## Vault Contract Overview

The `Vault` contract is an Ethereum smart contract designed to manage the deposit and withdrawal of ERC-20 tokens in a secure and efficient manner. It acts as a vault for a specific ERC-20 token, allowing users to deposit tokens to receive vault shares and withdraw tokens by redeeming these shares.

### Functions

1. **`deposit(uint _amount)`**
   - Allows users to deposit ERC-20 tokens into the vault, receiving shares in proportion to their deposit.
   - Implements a mathematical formula to calculate the number of shares to mint based on the current total supply and token balance of the vault.

2. **`withdraw(uint _shares)`**
   - Allows users to redeem a specified number of shares for the equivalent amount of ERC-20 tokens.
   - Implements a mathematical formula to calculate the amount of tokens to withdraw based on the current total supply and token balance of the vault.

### Variables

- `token`: An instance of the ERC-20 token interface representing the token managed by the vault.
- `totalSupply`: Total shares minted by the vault.
- `balanceOf`: Mapping of user addresses to their respective share balances.

## Readme for ERC20 Contract

# ERC-20 Token Contract

The `ERC20` contract provides a basic implementation of the ERC-20 token standard on the Ethereum blockchain. It enables the creation of a fungible token with functionalities such as transfers, allowances, approvals, minting, and burning.

### Key Features

- **`transfer`**: Allows users to transfer tokens to another address.
- **`approve`**: Permits users to approve another address to spend tokens on their behalf.
- **`transferFrom`**: Allows a delegated transfer of tokens from one address to another based on previous approval.
- **`mint`**: Enables the creation of new tokens by increasing the total supply.
- **`burn`**: Allows the destruction of tokens by reducing the total supply.

### Variables

- `totalSupply`: The total supply of the ERC-20 token.
- `balanceOf`: Mapping of user addresses to their respective token balances.
- `allowance`: Mapping of owner addresses to spender addresses and the allowed token amounts.

### Event Emission

- **`Transfer`**: Triggered when tokens are transferred from one address to another.
- **`Approval`**: Triggered when an owner approves another address to spend tokens on their behalf.

### Token Details

- `name`: The name of the ERC-20 token ("Solidity").
- `symbol`: The symbol representing the ERC-20 token ("SOL").
- `decimals`: The number of decimals for token representation (18).

## Author

Chandan S
