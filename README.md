# Smart Contracts: Money on Mars
The aim of this project is to build a monetary system for the first human colony on Mars.

## About
Smart Contracts on the Ethereum network can be used to create cryptocurrencies following the ERC-20 standard. In this project an ERC-20 compliant fungible token called KaseiCoin will be created on the Ethereum network. This token will be used to conduct monetary transactions by the first Human colony on Mars. The goal is to launch a crowdsale for the KaseiCoin token so that those who are moving to Mars can convert their earth money to it.

## Getting Started
To run the application, you need to use an Ethereum IDE such as [Remix](https://remix.ethereum.org/).

To deploy the contracts on a local blockchain, you will also need a local Ethereum blockchain such as [Ganache](https://trufflesuite.com/ganache/) and a wallet such as [Metamask](https://metamask.io/).

## Usage

You can clone or download this GitHub project and open the `KaseiCoin.sol` and `KaseiCoinCrowdsale.sol` using any IDE of your choice, one being Remix.

Ensure that the compiler is using solidity version 0.5.5.

Deploy the `KaseiCoinCrowdsaleDeployer` contract using your wallet as the Injected Provider.

Call the contract addresses of the `KaseiCoin` and `KaseiCoinCrowdsale` in the deployed `KaseiCoinCrowdsaleDeployer` contract.

Select the corresponding contract in the "CONTRACT" drop box and use the "At Address" button to load the `KaseiCoin` and `KaseiCoinCrowdsale` contracts.

# Report
## KaseiCoin Contract

Create and compile the `KaseiCoin` token contract.

<center>
    <img src="Execution_Results/Step1.png">
</center>

## KaseiCoin Crowdsale Contract

Create and compile the `KaseiCoinCrowdsale` contract.

<center>
    <img src="Execution_Results/Step2.png">
</center>

## KaseiCoin Deployer Contract

Create and compile the `KaseiCoinCrowdsaleDeployer` contract.

<center>
    <img src="Execution_Results/Step3.png">
</center>

## Deploy and Test the Crowdsale on a Local Blockchain

### KaseiCoin Crowdsale Deployer

Deploy the `KaseiCoinCrowdsaleDeployer` contract.

<center>
    <img src="Execution_Results/Step4_Remix_Load_Contracts.png">
</center>

View the results on the local blockchain.

|<img src="Execution_Results/Step4_Ganache_Accounts_Deployer.png"> |
|:--:|
|*Contract owned and deployed by Account 1*|

|<img src="Execution_Results/Step4_Ganache_Blocks_Deployer.png"> |<img src="Execution_Results/Step4_Ganache_Blocks__Block1_Deployer.png"> |
|:--:|:--:|
|*Block 1 created*|*Details of Block 1*|

|<img src="Execution_Results/Step4_Ganache_Transactions_Deployer.png"> |<img src="Execution_Results/Step4_Ganache_Transactions_TX1_Deployer.png"> |
|:--:|:--:|
|*Contract Creation transaction created*|*Details of the Contract Creation transaction*|

### KaseiCoin and KaseiCoin Crowdsale

Load the `KaseiCoin` and `KaseiCoinCrowdsale` contracts.

<center>
    <img src="Execution_Results/Step4_Remix_Load_Contracts.png">
</center>

### Buying Tokens on Account 2

Purchase 10 ETH worth of KaseiCoin tokens using Account 2.

|<img src="Execution_Results/Step4_Remix_Acc2_Confirm_Purchase.png"> |
|:--:|
|*Sign and Confirm the transaction on Account 2 using Metamask*|

View the results on the local blockchain.

|<img src="Execution_Results/Step4_Ganache_Accounts_Acc2_Purchase.png"> |
|:--:|
|*Crowdsale contract called by Account 2*|

|<img src="Execution_Results/Step4_Ganache_Blocks_Acc2_Purchase.png"> |<img src="Execution_Results/Step4_Ganache_Blocks_Block2_Acc2_Purchase.png"> |
|:--:|:--:|
|*Block 2 created*|*Details of Block 2*|

|<img src="Execution_Results/Step4_Ganache_Transactions_Acc2_Purchase.png"> |<img src="Execution_Results/Step4_Ganache_Transactions_TX2_Acc2_Purchase.png"> |
|:--:|:--:|
|*Contract Call transaction created*|*Details of the Contract Call transaction*|

Check the balance of Account 2 using the KaseiCoin contract "balanceOf" call.

|<img src="Execution_Results/Step4_Remix_Acc2_Check_Balance.png"> |
|:--:|
|*KaseiCoin balance of Account 2*|

### Buying Tokens on Account 3

Purchase 123456789 Wei worth of KaseiCoin tokens using Account 3.

|<img src="Execution_Results/Step4_Remix_Acc3_Confirm_Purchase.png"> |
|:--:|
|*Sign and Confirm the transaction on Account 3 using Metamask*|

View the results on the local blockchain.

|<img src="Execution_Results/Step4_Ganache_Accounts_Acc3_Purchase.png"> |
|:--:|
|*Crowdsale contract called by Account 3*|

|<img src="Execution_Results/Step4_Ganache_Blocks_Acc3_Purchase.png"> |<img src="Execution_Results/Step4_Ganache_Blocks_Block3_Acc3_Purchase.png"> |
|:--:|:--:|
|*Block 3 created*|*Details of Block 3*|

|<img src="Execution_Results/Step4_Ganache_Transactions_Acc3_Purchase.png"> |<img src="Execution_Results/Step4_Ganache_Transactions_TX3_Acc3_Purchase.png"> |
|:--:|:--:|
|*Contract Call transaction created*|*Details of the Contract Call transaction*|

Check the balance of Account 3 using the KaseiCoin contract "balanceOf" call.

|<img src="Execution_Results/Step4_Remix_Acc3_Check_Balance.png"> |
|:--:|
|*KaseiCoin balance of Account 3*|

### Token Balances on Metamask

Check the KaseiCoin token balances of Account 2 and Account 3 on Metamask.

|<img src="Execution_Results/Step4_Metamask_Import_Token.png"> |
|:--:|
|*Import the KaseiCoin token using the token's address*|

|<img src="Execution_Results/Step4_Metamask_Acc2_Check_Balance.png"> |<img src="Execution_Results/Step4_Metamask_Acc3_Check_Balance.png"> |
|:--:|:--:|
|*Token balances of Account 2*|*Token balances of Account 3*|

### Total Minted Token Supply and Wei Raised by the Crowdsale

Review the total supply of the minted KaseiCoin tokens and the amount of wei the KaseiCoin crowdsale contract has raised by using the "weiRaised" and "totalSupply" calls on the `KaseiCoinCrowdsale` and `KaseiCoin` contracts respectively.

<center>
    <img src="Execution_Results/Step4_Remix_Total_Supply_Wei_Raised.png">
</center>

## Contributor
Andy Vu