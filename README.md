# Solidity-Lottery-Contract
The Solidity Lottery Contract is a smart contract where people can enter the lottery by sending 0.1 ETH to the contract. 
When the owner of the contract decides, they can call the function pickWinner which will select a random player and award them with all of the ETH from the lottery.

Technical Spec for Lottery contract:

Anyone’s able to send a fixed amount of Ether to the contract’s address
The address of a sender will be stored in a dynamic array called players. The same user can send more than one transaction to have more chances of winning. The same principle as in a classical lottery where you can buy as many tickets as you want at a fixed price per ticket
The contract has an owner with special permission
After there are at least 3 players, the owner can call a function that makes the contract pick a random player from the list which will be the winner
The contract transfers the entire balance to the winner’s address, the players array is reset and the lottery is now ready to play again
