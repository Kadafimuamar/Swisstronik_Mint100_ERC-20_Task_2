# Swisstronik-erc-20

This repository contains a setup for deploying and interacting with an ERC-20 token on the Swisstronik testnet using Hardhat. The setup includes scripts for deploying the contract, minting tokens, and transferring tokens, utilizing encrypted transactions with Swisstronik.

## Prerequisites

Ensure you have the following installed:

- Node.js (version 14.x or later)
- npm (version 6.x or later)

## Faucet

https://faucet.testnet.swisstronik.com/

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/Kadafimuamar/Swisstronik_Mint100_ERC-20_Task_2.git
    cd Swisstronik_Mint100_ERC-20_Task_2
    ```

2. Run

    ```bash
    npm install --save-dev @nomicfoundation/hardhat-toolbox
    npm install dotenv
    npm install @swisstronik/utils
    npm install @openzeppelin/contracts
    ```

## Create File .env for Private Key (Keep Safe for this)

1. 

    ```bash
    PRIVATE_KEY=YOUR-PRIVATE-KEY
    ```



## Running

1. Compile

 ```bash
    npx hardhat compile
```

2. Deploy Erc-20

 ```bash
    npx hardhat run scripts/deploy.js --network swisstronik
```

2. Minting Erc-20

 ```bash
    npx hardhat run scripts/mint.js --network swisstronik
```

2. Minting Erc-20

 ```bash
    npx hardhat run scripts/transfer.js --network swisstronik
```

## Notes

- The `transfer.js` script is set to transfer tokens to the address `0x16af037878a6cAce2Ea29d39A3757aC2F6F7aac1` with an amount of `1 * 10 ** 18` tokens.
