# eth-avalanche-madule1-project
# Error Handling
In this project, we have a simple smart contract called errorhandling. The contract has a public variable value, and three functions, each using one of the error handling functions (require, assert, and revert).
# Description
*    withdraw(uint price): This function allows a user to withdraw funds from the contract. It checks if the requested price to withdraw is less than or equal to the amount available in the contract. If it's not, it throws an error with the message "There is not enough amount in the account" using the require statement.

*    deposit(uint price): This function allows a user to deposit funds into the contract. It increases the amount by the price. However, before completing the deposit, it checks if the updated amount would exceed 200. If it does, the contract reverts with the message "My amount cannot be exceeded more than 200" using the revert statement.

 *   isempty(): This is a read-only function that checks if the amount in the contract is 0. It uses the assert statement to ensure the condition holds. If amount is not 0, it will indicate a bug in the contract code, leading to a failure.
