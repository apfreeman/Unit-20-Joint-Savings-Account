# Unit 20 - "Joint Savings Account"

![alt=“”](Images/20-5-challenge-image.png)

## Background

A fintech startup company has recently hired me. This company is disrupting the finance industry with its own cross-border, Ethereum-compatible blockchain that connects financial institutions. Currently, the team is building smart contracts to automate many of the institutions’ financial processes and features, such as hosting joint savings accounts.

To automate the creation of joint savings accounts, I have created a Solidity smart contract that accepts two user addresses. These addresses will be able to control a joint savings account. My smart contract will use ether management functions to implement a financial institution’s requirements for providing the features of the joint savings account. These features will consist of the ability to deposit and withdraw funds from the account.

## What I have Created

* A completed Solidity `JointSavings` smart contract.

* A folder named `Execution_Results` that contains all execution result images. These images confirm that the deposit and withdrawal transactions, which are designed to test the `JointSavings` functionality in the JavaScript VM, worked as expected.

### Compile and Deploy Your Contract in the JavaScript VM

1. I have successfully compiled the smart contract.

![](https://github.com/apfreeman/Unit-20-Joint-Savings-Account/blob/main/Execution_Results/1_compile.PNG?raw=true)

2. In the Remix IDE, I navigated to the “Deploy & Run Transactions” pane, and then made sure that “JavaScript VM” is selected as the environment.

3. I have deployed my smart contract, and then confirmed that it successfully deployed.

![](https://github.com/apfreeman/Unit-20-Joint-Savings-Account/blob/main/Execution_Results/2_deploy.PNG?raw=true)

### Interact with the Deployed Smart Contract

Now that the contract is deployed, it’s time to test its functionality! After each step, I have captured a screenshot of the execution, and then saved it in a folder named `Execution_Results`.

To interact with my deployed smart contract, I have completed the following steps:

1. Used the `setAccounts` function to define the authorized Ethereum addresses that will be able to withdraw funds from the contract.

![](https://github.com/apfreeman/Unit-20-Joint-Savings-Account/blob/main/Execution_Results/3_setAccounts.PNG?raw=true)

2. Tested the deposit functionality of the smart contract by sending the following amounts of ether. After each transaction, I have used the `contractBalance` function to verify that the funds were added to my contract:

    * Transaction 1 - Send **1 ether** as wei.
    ![](https://github.com/apfreeman/Unit-20-Joint-Savings-Account/blob/main/Execution_Results/4_contract_balance_1.PNG?raw=true)

    * Transaction 2 - Send **10 ether** as wei.
    ![](https://github.com/apfreeman/Unit-20-Joint-Savings-Account/blob/main/Execution_Results/5_contract_balance_2.PNG?raw=true)

    * Transaction 3 - Send **5 ether.**
    ![](https://github.com/apfreeman/Unit-20-Joint-Savings-Account/blob/main/Execution_Results/6_contract_balance_3.PNG?raw=true)

3. All funds have been successfully deposited into my contract. I have tested the contract’s withdrawal functionality by withdrawing 5 ether into `accountOne` and 10 ether into `accountTwo`. After each transaction, I have used the `contractBalance` function to verify that the funds were withdrawn from my contract. I have also, use the `lastToWithdraw` and `lastWithdrawAmount` functions to verify that the address and amount were correct.


    * Withdrawal 1 - **5 ether** into `accountOne`, withdrawal and Account balance logs. 
    ![](https://github.com/apfreeman/Unit-20-Joint-Savings-Account/blob/main/Execution_Results/7_contract_withdrawal_balance_1.PNG?raw=true)

    * Withdrawal 1 -  `lastToWithdraw` and `lastWithdrawAmount` logs.
    ![](https://github.com/apfreeman/Unit-20-Joint-Savings-Account/blob/main/Execution_Results/8_lastToWithdraw_lastWithdrawal_1.PNG?raw=true)

    * Withdrawal 2 -  **10 ether** into `accountTwo`, withdrawal and Account balance logs. 
    ![](https://github.com/apfreeman/Unit-20-Joint-Savings-Account/blob/main/Execution_Results/9_contract_withdrawal_balance_2.PNG?raw=true)

    * Withdrawal 2 - `lastToWithdraw` and `lastWithdrawAmount` logs.
    ![](https://github.com/apfreeman/Unit-20-Joint-Savings-Account/blob/main/Execution_Results/10_lastToWithdraw_lastWithdrawal_2.PNG?raw=true)