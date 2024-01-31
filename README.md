Building on Avalanche-Degen Token

## Overview
For Solidity-Gagan Token (G) Smart Contract

This repository contains a Solidity smart contract for the Gagan Token (G). The Gagan token is an ERC-20 token that includes features for minting, burning, and ownership management. The contract is based on OpenZeppelin's ERC-20, ERC-20 Burnable, and Ownable contracts. It is licensed under the MIT License.

For Deploy-Degen Token (DGN) Smart Contract

This repository contains a Solidity smart contract for the Degen Token (DGN). The Degen token is an ERC-20 token that includes features for minting and ownership management. The contract is based on OpenZeppelin's ERC-20 and Ownable contracts. It is licensed under the MIT License.

## Description
For Solidity-Features:
ERC-20 Standard:Implements the ERC-20 standard for fungible tokens.
Supports functions such as transfer, approve, and transferFrom.
Burnable:Extends the ERC20Burnable contract from OpenZeppelin for burning (destroying) tokens.
The commented-out burn function allows the owner to burn a specific amount of tokens.
Ownable:Extends the Ownable contract from OpenZeppelin to manage ownership.
Ensures that only the owner can perform certain functions, such as minting new tokens.
Minting:Includes a mint function that allows the owner to mint (create) new tokens and assign them to a specific address.

For Deploy-Features:
ERC-20 Standard:Implements the ERC-20 standard for fungible tokens.
Supports functions such as transfer, approve, and transferFrom.
Ownable:Extends the Ownable contract from OpenZeppelin to manage ownership.
Ensures that only the owner can perform certain functions, such as minting new tokens.
Minting:Includes a mint function that allows the owner to mint (create) new tokens and assign them to a specific address.

## Executing program

For Solidity-Import Statements:
The contract imports two OpenZeppelin contracts: ERC20 for the standard ERC-20 functionality and Ownable for ownership management.
Contract Declaration:The DegenToken contract inherits from ERC20 and Ownable.
Constructor:The constructor initializes the token with the name "Degen" and the symbol "DGN".
Mint Function:The mint function allows the owner to mint new tokens and assign them to a specified address. This function is restricted to the contract owner, as indicated by the onlyOwner modifier.

For Deploy-Import Statements:
The script imports the hardhat module, which provides the Hardhat development environment.
Async Function main():The main function is marked as async to allow the use of await for asynchronous operations.
Inside main, the getContractFactory method is used to retrieve the factory for the DegenToken contract.
Contract Deployment:The DegenToken contract is deployed using the deploy method, and the deployed instance is stored in the variable degen.
Display Contract Address:The script logs the address of the deployed DegenToken contract to the console.
Error Handling:The script utilizes a catch block to log errors to the console and set the process exit code to 1 in case of an error.
Execution:The main function is called at the end of the script to initiate the deployment process.

## Help
For Solidity-
1.Understanding ERC-20 Tokens:
Familiarize yourself with the ERC-20 standard. It defines a set of rules for creating tokens on the Ethereum blockchain.
2. Review OpenZeppelin Contracts:
Understand the roles of ERC20 and Ownable contracts from OpenZeppelin.
ERC20 provides the standard ERC-20 token functionality.
Ownable ensures that certain functions can only be executed by the owner.
3. Minting Function:
Review the mint function. It allows the contract owner to create and assign new tokens to a specified address.
Minting is a common method to create and distribute new tokens.

For Deploy-
1. Setting Up Hardhat:
Ensure Hardhat is installed globally or as a development dependency (npm install --save-dev hardhat).
2. Understanding the Deployment Script:
The script uses Hardhat's ethers module to deploy the smart contract.
It uses the getContractFactory method to get the factory for the DegenToken contract.
3. Running the Script:
Execute the deployment script using Hardhat: npx hardhat run <script-name>.
4. Troubleshooting:
In case of errors, check the error message logged to the console.
Review Hardhat's configuration and ensure that it is set up properly.
5. Deployment to Networks:
The script is designed for local development. For deployment to Ethereum mainnet or testnets, you may need to modify the Hardhat configuration.
6. Dependencies:
Ensure that the necessary dependencies are installed, such as @openzeppelin/contracts and ethers.
7. Project Structure:
Confirm that the smart contract file (DegenToken.sol) is present in the project directory.

## Authors
H N GAGAN
gaganhn2004@gmail.com

## License
This project is licensed under the MIT License
