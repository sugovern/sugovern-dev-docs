The purpose of this contract is to create two types of SUToken and transfer their ownership to the contract that initiated the creation.

- `transfer(address to, uint256 amount)`: This function is used for transfer processes. The function checks the balance of the owner to make sure there are enough credits and gives an option to have a debt if balance is insufficient and modifies the balance amount accordingly.

- `delagation_multiple_getback_all(address to)`: This function allows the user to take back all of the delegated tokens.
