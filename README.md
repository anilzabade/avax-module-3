# MyToken Contract

## Overview

MyToken is an Ethereum smart contract written in Solidity. It implements a basic ERC-20 token with additional functionalities. The contract allows the creation, burning, and transfer of tokens, with special access control for the owner.

## Features

- **Token Information:**
  - Token Name: MyToken
  - Token Symbol: MTK
  - Decimals: 18

- **Ownership:**
  - The contract is owned by the deployer.

- **Access Control:**
  - Only the owner can mint new tokens.

- **Functions:**
  1. **Minting:**
     - Function: `mint(address to, uint256 size)`
     - Description: Mint new tokens and assign them to a specified address.
     - Access: Only the owner can perform this operation.

  2. **Burning:**
     - Function: `burn(uint256 size)`
     - Description: Burn a specified amount of tokens.
     - Access: Any account can burn their own tokens.

  3. **Transferring:**
     - Function: `transfer(address to, uint256 size)`
     - Description: Transfer tokens to a specified address.
     - Access: Any account can transfer tokens if they have a sufficient balance.

  4. **Check Remaining Funds:**
     - Function: `leftFunds(address account) view returns (uint256)`
     - Description: Check the remaining token balance of a specified account.

## Usage

1. **Deploy Contract:**
   - Deploy the contract to an Ethereum network.

2. **Mint Tokens:**
   - The owner can mint new tokens using the `mint` function.

3. **Burn Tokens:**
   - Any account can burn a specified amount of their own tokens using the `burn` function.

4. **Transfer Tokens:**
   - Any account can transfer tokens to another account using the `transfer` function.

5. **Check Balance:**
   - Use the `leftFunds` function to check the remaining token balance of an account.

## Author 

Anurag

Anilzabade5@gmail.com
