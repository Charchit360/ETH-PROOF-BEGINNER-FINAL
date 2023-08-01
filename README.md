# MyToken Smart Contract

This is a simple Solidity smart contract named "MyToken" that implements a basic ERC20-like token functionality. The contract allows the creation, destruction, and management of custom tokens with specific functionalities.


## Description
MyToken is a Solidity smart contract that implements a basic ERC20 token. It allows users to mint new tokens and burn existing tokens. The contract keeps track of the token name, token abbreviation, total supply, and individual balances of addresses by using mapping.
## Code Explanation

The contract includes the following features:

1. **Public Variables:**
   - `tokenName`: A public string variable representing the name of the token.
   - `tokenAbbr`: A public string variable representing the abbreviation of the token.
   - `totalSupply`: A public uint variable representing the total supply of tokens.

2. **Mapping of Balances:**
   - `balances`: A mapping that associates addresses with their corresponding token balances.

3. **Mint Function:**
   - `mint(address _address, uint _value)`: A function used to mint new tokens. It takes two parameters: `_address` (the address to mint tokens for) and `_value` (the number of tokens to mint). It increases the total supply by `_value` and updates the balance of the `_address`.

4. **Burn Function:**
   - `burn(address _address, uint _value)`: A function used to burn existing tokens. It takes two parameters: `_address` (the address to burn tokens from) and `_value` (the number of tokens to burn). It decreases the total supply by `_value` and updates the balance of the `_address`. It also includes conditionals to ensure that the balance of the `_address` is greater than or equal to the amount that is supposed to be burned.

## Author
The MyToken contract is authored by Charchit (21BCG1028).

## License
This project is licensed under the MIT License.
