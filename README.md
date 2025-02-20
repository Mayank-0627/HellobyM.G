// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract SavingsVault {

    // Deposit function that allows users to deposit ETH
    function deposit() external payable {
        // No need for anything else, the contract will automatically receive ETH
    }

    // Withdraw function that allows users to withdraw ETH
    function withdraw(uint256 amount) external {
        // Ensure the contract has enough balance to fulfill the withdrawal
        require(address(this).balance >= amount, "Insufficient balance in vault");
        
        // Transfer the specified amount to the caller
        payable(msg.sender).transfer(amount);
    }

    // View function to check the balance of the contract
    function getVaultBalance() external view returns (uint256) {
        return address(this).balance;
    }
}
0x6060861d31aA16b2d1f28aBeeC73C26316a0dF55
