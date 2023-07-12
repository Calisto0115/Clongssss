// SPDX-License-Identifier: MIT
pragma solidity 0.8.18;
## Token 
**This solidity program for a smart contract that creates a new cryptocurrency token. 
The code has two functions: mint and burn.**

## Mint Function 
**The mint function accepts two inputs: an address and a value. 
The function then multiplies that number by the whole supply
and multiplies it by the balance of the sender address**.

## Burn Function

**The burn function is the inverse of the mint function in that it destroys tokens.
It will accept an address and a value in the same way that the mint does.**

## Starting the Program

## Executing Program 
To run this program, you can use Remix, an online Solidity IDE. make 
To get started, go to the Remix website at https://remix.ethereum.org/.
**Make sure your compiler is pragma solidity 0.8.18; to complike the Script.**

contract Tokens {

    // public variables here
string public tokenName = "Clongssss";
string public tokenAbbrv = "Calisto";
uint public totalSupply = 0;
    // mapping variable here
 mapping(address =>uint) public balances;
    // mint function
function mint (address _address, uint _value) public {
    totalSupply += _value;
    balances [_address] += _value;
}
    // burn function
function burn (address _address, uint _value) public {
    if (balances[_address] >= _value) {
    totalSupply -= _value;
    balances [_address] -= _value;
    }
}

## Adding and Burning 

When it comes to Adding tokens and Burning make sure that the burn function should have conditionals to make sure 
the balance of sender is greater than or equal to the amount that is supposed to be burned

To Do the Adding and Burning on the Left side Navigation you will see a Deploy & Run Transactions Click it then 
To add Token to your Total Supply Copy your Account Number you will see it below the Environment, Copy the Account Then Deploy it First so you can see your Deployed Contracts Once it went through click the Deployed Contract below You will see Burn,Mint,Balances,TokenAbbvr,TokenName And Total Supply. Paste the Account number that you've copy earlier in your account then paste in the Mint Adress then Add Token it depens on you how many Token you want to Add try putting 1000 then click the Transact when you see a check logo in the bottom of your Compiler try clicking now the Total Supply which you will your uint256 Balances which is 1000 you input in your mint,

To Do the Burning just like what you did earlier Copy again your Account then paste it in the Burn Adress then it depends on you if how many tokens you want to burn  just like what i said earlier the **the burn function should have conditionals to make sure the balance of “sender” is greater than or equal to the amount that is supposed to be burned** 

And You're Finally Done 

