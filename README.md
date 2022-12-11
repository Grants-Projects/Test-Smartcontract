# DeadManSwitch
Dead Man Switch that transfers Balance from Wallet A to Wallet B after 3 months.
This contract defines a DeadManSwitch struct with wallet_a, wallet_b, and deployment_timestamp fields. The DeadManSwitch struct is initialized with the wallet_a and wallet_b addresses in the constructor. The deployment_timestamp is set to the current timestamp when the contract is deployed.

The transfer_balance() function calculates the difference between the current timestamp and the deployment_timestamp, and checks if the difference is greater than or equal to 3 months (in seconds). If it is, the function transfers the balance from wallet_a to wallet_b, and returns true to indicate that the transfer was successful. If the difference is less than 3 months, the function returns false to indicate that the transfer was not performed.
