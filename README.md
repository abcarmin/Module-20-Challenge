# Module-20-Challenge

For this project, I am utilizing Solidity and Remix IDE to create a Solidity smart contract that controls a joint savings account. The smart contract uses ether management functions to deposit and withdraw funds from the joint savings account.

---

## Technologies

This project uses Solidity, Remix IDE, Git Bash, Visual Studio, Github.

---

## Installation Guide

The web version of Remix IDE was used and this is the Solidity version that was used:

    pragma solidity ^0.5.0

---

## Usage

* Step 1: Create a Joint Savings Account Contract in Solidity

I defined a new contract named JointSavings with the following variables:

    contract JointSavings {

        address payable accountOne; 

        address payable accountTwo; 

        address public lastToWithdraw;

        uint public lastWithdrawAmount;

        uint public contractBalance;


Within the contract, I defined withdraw, deposit, and setAccounts functions. I ended the contract with a fallback function.


* Step 2: Compile and Deploy Your Contract in the JavaScript VM

I successfully compiled my contract and deployed it under the JavaScript VM(Now called Remix VM)

![Compile and Deploy](https://github.com/abcarmin/Module-20-Challenge/blob/main/Screenshot%20(16).png)



* Step 3: Interact with Your Deployed Smart Contract

I used the setAccounts function to define the addresses that are able to withdraw funds:

![setAccounts Function](https://github.com/abcarmin/Module-20-Challenge/blob/main/Screenshot%20(10).png)


I deposited 1 ether into the account and tested the contractBalance function:

![Deposit Function](https://github.com/abcarmin/Module-20-Challenge/blob/main/Screenshot%20(11).png)


I deposited 10 more ether into the account and tested the contractBalance function:

![Deposit Function](https://github.com/abcarmin/Module-20-Challenge/blob/main/Screenshot%20(12).png)


I deposited 5 more ether into the account and tested the contractBalance function:

![Deposit Function](https://github.com/abcarmin/Module-20-Challenge/blob/main/Screenshot%20(13).png)


I withdrew 5 ether into accountOne then tested the contractBalance, lastToWithdraw, and lastWithdrawAmount functions:

![Withdraw Function](https://github.com/abcarmin/Module-20-Challenge/blob/main/Screenshot%20(14).png)


I withdrew 10 ether into accountTwo then tested the contractBalance, lastToWithdraw, and lastWithdrawAmount functions:

![Withdraw Function](https://github.com/abcarmin/Module-20-Challenge/blob/main/Screenshot%20(15).png)




---

## Contributors

Allyssa Carmin

---

## License

SMU Fintech Course