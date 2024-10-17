# Project Title
MyToken Smart Contract  

**Simple overview of use/purpose:**  
This is a Solidity-based smart contract that allows the minting and burning of custom tokens. It can be used to manage token supply on the Ethereum blockchain.

## Description  
MyToken is a smart contract written in Solidity that provides a basic framework for creating a cryptocurrency-like token system. The contract allows you to define a token name, abbreviation, and manage the total supply. Users can mint new tokens, increasing the total supply, and burn tokens, decreasing it. The mint function increases the supply and adds the minted amount to the user's balance, while the burn function removes tokens from the user's balance, subject to conditions ensuring the user has enough tokens to burn.

## Getting Started

### Installing  
To use this contract, you will need the following:  
- Solidity version 0.8.26 or higher  
- A development environment such as [Remix](https://remix.ethereum.org/) or a local Ethereum development setup with tools like Hardhat or Truffle.

1. **Clone the repository** (if applicable) or simply copy the code to your Solidity development environment.  
2. **No specific modifications** are required to the files or folders. However, you may need to modify the contract parameters like token name and abbreviation if required.

### Executing Program

1. **Deploying the contract**:  
   In Remix, compile the contract using Solidity 0.8.26. After compiling, deploy the contract to your chosen network (e.g., Ethereum testnet, local Ganache, etc.).

2. **Mint tokens**:  
   Once the contract is deployed, you can call the `mint` function to mint new tokens for a given address.  

  ```
    mint(address _address, uint _company)
  ```
3. Burn tokens:
   To burn tokens, use the burn function. Ensure the address has sufficient tokens to burn.

  ```
    burn(address _address, uint _company)
  ```
### Help
 
**Common issues**:
Insufficient balance for burning: Ensure that the address calling the burn function has a token balance greater than or equal to the amount they are trying to burn.
Gas costs: Smart contract functions on the Ethereum network require gas fees. Be sure to have enough ETH for the transaction.
Command to run if program contains helper info:
If using Remix, no additional helper command is needed. All functions can be tested through the Remix UI after deploying the contract.

### Authors
Albert Kobe Serrano
202110970@fit.edu.ph

### License
This project is licensed under the MIT License - see the LICENSE.md file for details.
