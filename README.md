VaultSafe
VaultSafe is a smart contract built on Ethereum using Solidity. It works like a digital savings vault where users can deposit and withdraw Ether (ETH) securely.

Features
Deposit ETH: You can send ETH into the contract and store it.
Withdraw ETH: You can take ETH out of the contract at any time, as long as there is enough balance.
Check Vault Balance: You can check how much ETH is currently stored in the vault.
How It Works
Deposit: You can send ETH to the contract, and it will be stored in the vault. The contract automatically accepts the ETH.
Withdraw: You can request to withdraw a specific amount of ETH. The contract will check if there is enough balance and transfer the ETH to you.
View Balance: You can check how much ETH is in the vault by calling the getVaultBalance function.
Functions
1. deposit()
Description: This function allows you to deposit ETH into the vault.
Usage: Just send ETH to the contract (no extra steps needed).
2. withdraw(uint256 amount)
Description: This function allows you to withdraw a specific amount of ETH from the vault.
Usage: Call the function with the amount of ETH you want to withdraw.
3. getVaultBalance()
Description: This function returns the current balance of the contract (how much ETH is stored in the vault).
Usage: Call this function to view the vault's balance.
How to Interact with the Contract
Deploy the contract on an Ethereum network (like the testnet or mainnet).
Deposit ETH by sending ETH to the contract using the deposit() function.
Withdraw ETH by specifying the amount you want to withdraw with the withdraw() function.
Check the Vault Balance by calling getVaultBalance().
Example Usage
Deposit ETH
To deposit ETH, simply send ETH to the contract, or call deposit() in your interface.

Withdraw ETH
To withdraw ETH, call the withdraw() function and specify how much ETH you want to withdraw. For example:

solidity
Copy
vaultSafe.withdraw(1 ether); // This will withdraw 1 ETH
Check Vault Balance
To see how much ETH is stored in the vault, you can call:

solidity
Copy
vaultSafe.getVaultBalance(); // This will return the current balance
Security
The contract checks if there is enough balance to fulfill a withdrawal request.
It does not allow withdrawing more than the contract’s available balance
0x6060861d31aA16b2d1f28aBeeC73C26316a0dF55
