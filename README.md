# CPmm DEX

## Overview

The CPmm DEX (Constant Product Market Maker Decentralized Exchange) is a decentralized exchange implemented using Solidity for the Ethereum blockchain and JavaScript for the front-end interface. This DEX allows users to trade ERC-20 tokens directly from their wallets without the need for intermediaries. It leverages the constant product formula to maintain liquidity in the market.

## Features

- **Decentralized Trading**: Users can trade tokens directly without relying on a centralized exchange.
- **Liquidity Pools**: Users can add liquidity to pools and earn a portion of the trading fees.
- **Automated Market Making**: Uses the constant product formula (x * y = k) to ensure liquidity.
- **Secure and Transparent**: All transactions are executed through smart contracts on the Ethereum blockchain.

## Technologies Used

- **Solidity**: Smart contracts for the Ethereum blockchain.
- **JavaScript**: Front-end interface to interact with the smart contracts.
- **Web3.js**: Library to interact with the Ethereum blockchain.
- **Hardhat**: Development environment for Ethereum.
- **React.js**: User interface library.

## Getting Started

### Prerequisites

- **Node.js**: Ensure you have Node.js installed. You can download it from [here](https://nodejs.org/).
- **Hardhat**: Install Hardhat using npm:
  ```sh
  npm install --save-dev hardhat
  ```
- **Ganache**: A personal blockchain for Ethereum development. Install it from [here](https://www.trufflesuite.com/ganache).

### Installation

1. **Clone the Repository**:
   ```sh
   git clone https://github.com/SabaliDev/cpmm-dex.git
   cd cpmm-dex
   ```

2. **Install Dependencies**:
   ```sh
   npm install
   ```

3. **Compile Smart Contracts**:
   ```sh
   npx hardhat compile
   ```

4. **Deploy Smart Contracts**:
   ```sh
   npx hardhat run scripts/deploy.js --network localhost
   ```

5. **Run the Front-end**:
   ```sh
   npm start
   ```

## Smart Contract Overview

### CPmm.sol

This is the main smart contract that handles the core functionality of the DEX.

#### Functions:

- **addLiquidity**: Allows users to add liquidity to the pool.
- **removeLiquidity**: Allows users to remove liquidity from the pool.
- **swap**: Executes token swaps using the constant product formula.
- **getReserves**: Returns the current reserves of the token pair.

### Token.sol

An example ERC-20 token implementation for testing the DEX.

## Front-end Overview

The front-end is built using React.js and Web3.js to interact with the smart contracts deployed on the Ethereum blockchain.

### Key Components:

- **App.js**: Main component that initializes Web3 and interacts with the smart contracts.
- **Liquidity.js**: Component for adding and removing liquidity.
- **Swap.js**: Component for executing token swaps.

## Usage

1. **Add Liquidity**: Navigate to the "Liquidity" section and provide the amounts of tokens you want to add to the pool.
2. **Swap Tokens**: Navigate to the "Swap" section, select the tokens you want to trade, and execute the swap.
3. **Remove Liquidity**: Navigate to the "Liquidity" section, select the amount of liquidity you want to remove, and execute the transaction.

## Contributing

We welcome contributions from the community. To contribute:

1. Fork the repository.
2. Create a new branch.
3. Make your changes.
4. Submit a pull request.

## License

This project is licensed under the MIT License.

## Contact

For any inquiries or support, please reach out to mthunzisabali@gmail.com or create an issue on GitHub.

---

Thank you for using CPmm DEX! Happy trading!

---

This README provides a comprehensive overview of the CPmm DEX, including installation steps, smart contract details, and usage instructions. Make sure to update the placeholder details like the GitHub repository URL and contact email with actual information.
