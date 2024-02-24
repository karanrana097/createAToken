# MyToken Solidity Contract

This Solidity contract, named `MyToken`, implements a basic ERC20-like token with functionalities for minting and burning tokens. Below are the details of the contract:

## Contract Overview

The `MyToken` contract implements a simple token with the following features:

1. **Token Details**:
   - `tokenName`: A public variable storing the name of the token.
   - `tokenAbbrv`: A public variable storing the abbreviated name of the token.
   - `totalSupply`: A public variable storing the total supply of the token.

2. **Balances Mapping**:
   - `balances`: A mapping of addresses to token balances, where each address corresponds to the balance of tokens held by that address.

3. **Minting Functionality**:
   - `mint(address _address, uint _value)`: A function to mint new tokens. It takes an address and a value as parameters, increases the total supply by the specified value, and increases the balance of the given address by that amount.

4. **Burning Functionality**:
   - `burn(address _address, uint _value)`: A function to burn existing tokens. It takes an address and a value as parameters, deducts the specified value from the total supply, and decreases the balance of the given address by that amount. This function includes conditionals to ensure that the balance of the sender is greater than or equal to the amount intended to be burned.

## Usage

1. **Deploy the Contract**:
   - Deploy this contract on an Ethereum-compatible blockchain network.

2. **Interact with the Contract**:
   - Use the `mint` function to create new tokens by providing an address and the desired token amount.
   - Use the `burn` function to destroy existing tokens by providing an address and the amount of tokens to be burned.

## License

This contract is licensed under the MIT License. You can find the license text in the contract file itself under the SPDX-License-Identifier tag.

## Note

This contract serves as a basic template for a token implementation and lacks many features typically found in production-ready token contracts, such as access control, transfer restrictions, and event logging. Ensure to extend and modify it according to your specific requirements and security considerations.
