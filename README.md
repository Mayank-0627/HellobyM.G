VaultSafe
VaultSafe is a simple Ethereum smart contract designed to securely store and manage Ether (ETH). It allows users to easily deposit and withdraw ETH, while also providing transparency about the vault's balance.

Smart Contract Address
0x6060861d31aA16b2d1f28aBeeC73C26316a0dF55

Features
Deposit ETH: Send ETH to the vault for safekeeping.
Withdraw ETH: Withdraw ETH from the vault anytime, as long as there's enough balance.
Check Balance: View the current balance of the vault.
How to Use
1. Deposit ETH
Send ETH to the contract using the deposit() function. Your ETH will be safely stored in the vault.

2. Withdraw ETH
Withdraw ETH by specifying the amount using the withdraw(uint256 amount) function.

3. Check Vault Balance
Use the getVaultBalance() function to check how much ETH is stored in the vault.

Example Usage
Deposit ETH:
Simply send ETH to the contract or use the deposit() function.

Withdraw ETH:
Call the withdraw(1 ether) function to withdraw 1 ETH.

Check Vault Balance:
Use the getVaultBalance() function to see the current balance in the vault.
