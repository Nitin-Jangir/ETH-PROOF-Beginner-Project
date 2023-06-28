# MyToken Solidity Contract
This Solidity contract implements a basic token contract with the ability to mint and burn tokens. It allows for the creation and management of a custom token on the Ethereum blockchain.
## Requirements
1. The contract has public variables that store the details about the token, including the token name, token abbreviation, and total supply.
2. It utilizes a mapping data structure to store the balances of addresses that hold the tokens.
3. The contract includes a mint function that increases the total supply by a specified value and adds the corresponding amount to the balance of a designated address.
4. The contract includes a burn function that decreases the total supply by a specified value and deducts the corresponding amount from the balance of a designated address, given that the balance is sufficient.

## Usage
1. Deploy the contract to an Ethereum network of your choice (e.g., using Remix or Truffle).
2. Set the token details by providing the token name, abbreviation, and total supply in the constructor during contract deployment.
3. Interact with the contract using the following functions:
   * mint(address recipient, uint256 value): Increases the total supply by the specified value and adds the same amount to the balance of the recipient address.
   * burn(address sender, uint256 value): Decreases the total supply by the specified value and deducts the same amount from the balance of the sender address, provided that the sender has a sufficient balance.

## Examples
![image](https://github.com/Nitin-Jangir/ETH-PROOF-Beginner-Project/assets/137036246/b7813b9f-36a8-4991-8a83-199c3fbba156)
![image](https://github.com/Nitin-Jangir/ETH-PROOF-Beginner-Project/assets/137036246/2032e9c3-b2c7-41be-9ae1-c61bdd2f70e4)

## Notes
* Ensure that the sender of the transactions has the necessary balance to perform token burning, as the burn function includes a check for the sufficient balance.
* The contract does not include additional functionality like token transfers or allowance management, as it focuses solely on the minting and burning of tokens.

## License
This project is licensed under the MIT License.
