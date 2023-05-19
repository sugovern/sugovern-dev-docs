The Migrations contract is a simple contract that stores the last completed migration. The contract has a `setCompleted` function that sets the `last_completed_migration` variable to the value passed in as a parameter. However, this function can only be called by the contract owner.

The restricted modifier restricts the function so that only the owner of the contract can call it. If a non-owner account attempts to call the function, an exception is thrown and the transaction is reverted.

The contract also has an `owner` variable that is initialized with the address of the contract deployer. This address is used in the restricted modifier to check that the calling account is the owner of the contract.

This contract can be used as a base contract for contract migrations.
