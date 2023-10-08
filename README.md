# **DeFi Kingdom Clone**

This repository has two Solidity smart contracts: `ERC20` and `vault` which are deployed using Avalanche custom EVM subnet in Avalanche CLI.

## **ERC20 Contract**

### **Overview**
The `ERC20` contract is an implementation of the ERC-20 token standard. The following are the attributes of the token:

- **Name**: Solidity by Example
- **Symbol**: SOLBYEX
- **Decimals**: 18
- **Total Supply**: Variable ehich is initialized to 0

### **Functions**
1. **`transfer`**
    The transfer function allows the user to transfer tokens to another account.
   
2. **`approve`**
    The approve function allows the owner to approve another account to spend tokens on its behalf.

3. **`transferFrom`**
    This function allows an approved spender to transfer tokens from one account to another.

4. **`mint`**
    The mint function allows the contract owner to create new tokens and add them to their balance.

5. **`burn`**
    this function allows an account to burn (destroy) a specified number of their tokens.


## **Vault Contract**

### **Overview**
The `Vault` contract acts as a vault for storing ERC-20 tokens securely. It implements a mechanism to deposit and withdraw tokens while minting and burning corresponding shares for users.

### **Constructor**
 **`constructor`**: Initializes the contract with the address of the ERC-20 token to be stored in the vault.

### **Functions**
1. **`deposit`**
    Allows users to deposit ERC-20 tokens into the vault and calculates the number of shares to mint based on the user's deposit and existing shares.

2. **`withdraw`**
    Allows users to withdraw ERC-20 tokens from the vault by burning shares and calculates the amount of tokens to be withdrawn based on the number of shares burned.

### **State Variables**
- **`token`**: Stores the address of the ERC-20 token that the vault holds.
- **`totalSupply`**: Tracks the total number of shares in the vault.
- **`balanceOf`**: A mapping that records the number of shares held by each user.

### **Authors**  
Akash
Email: vermakash876@gmail.com

  ### **Licence**
  This smart contract is licensed under MIT license. Check licence.md file for more information.
