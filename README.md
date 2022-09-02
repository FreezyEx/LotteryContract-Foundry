# <h1 align="center"> Lottery Contract </h1>

![Github Actions](https://github.com/freezyex/LotteryContract-Foundry/workflows/test/badge.svg)

## DISCLAIMER
This is my first time I use Foundry, so it is very likely that many things can be improved.  
Feel free to contribute to the repo!

## How does it work?
The contract uses a PRNG function to pick a winner from an array of players, as VRF wasn't necessary for the purpose of this project.  
To gurantee a 100% fairness, the admin must compute the hash of a random string off-chain and set it at the creation of each lottery. 
Once the hash for that lottery is set, it can't be changed. To provide more randomness, the admin can call the ``pickWinner()`` whenever he wants.
 

## Getting Started

```sh
forge init
forge build
forge test
```

## Development

This project uses [Foundry](https://getfoundry.sh). See the [book](https://book.getfoundry.sh/getting-started/installation.html) for instructions on how to install and use Foundry.
