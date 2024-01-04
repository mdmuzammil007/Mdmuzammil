# Mutual Investment Fund 

## Overview

This Solidity smart contract, named `InvestmentFund`, is designed to manage an investment fund on the Ethereum blockchain. The contract allows investors to contribute funds through a systematic investment plan (SIP) and specifies rules for withdrawal.

## Features

### Manager

The contract has a designated manager, initially set to the address deploying the contract. The manager is responsible for overseeing the investment fund.

### Investors and SIP

Investors can participate in the fund by calling the `mutualFund` function. This function requires a tenure (investment duration) and a SIP amount. The SIP amount must be at least 5000 ethers.

### Minimum Tenure Requirement

The contract enforces a minimum tenure requirement for investments. Investors must hold their funds for a minimum period of 5 years (`MINIMUM_TENURE`). The `assert` statement in the `mutualFund` function ensures this condition is met.

### Withdrawal

Investors can initiate a withdrawal by calling the `withdraw` function, providing a tenure of at least 10 years. 
The manager can withdraw the entire fund balance.

### Balance Inquiry

Investors can check the balance of the contract using the `checkBalance` function, which returns the current balance in ethers.

## License

This smart contract is open-source and released under the MIT License.

## Author 

Mdmuzammil

mdmuzammil000007@gmail.com
