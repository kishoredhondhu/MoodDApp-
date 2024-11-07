# MoodDApp

A simple decentralized application (dApp) on Ethereum that allows users to set and retrieve their "mood" on the blockchain. This project serves as an introductory example of building a dApp, utilizing Solidity for the smart contract and a web interface for user interaction.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [License](#license)

## Introduction

**MoodDApp** is a decentralized application built on Ethereum's Sepolia test network. It allows users to store a mood on the blockchain through a simple web interface. Users interact with the dApp via MetaMask, which ensures secure transactions and data storage on the blockchain.

This project demonstrates how to develop and deploy a smart contract, connect it to a front-end web interface, and interact with the Ethereum blockchain using JavaScript and MetaMask.

## Features

- **Set Mood**: Store a mood on the blockchain.
- **Get Mood**: Retrieve the stored mood from the blockchain.
- **Decentralized Storage**: All mood data is stored on Ethereum’s Sepolia test network.

## Technologies Used

- **Solidity**: For writing the smart contract.
- **Remix IDE**: For compiling and deploying the smart contract on the Sepolia test network.
- **JavaScript & HTML**: For building the front-end interface.
- **Viem**: A library for interacting with Ethereum and smart contracts.
- **MetaMask**: A browser extension for managing Ethereum accounts and interacting with dApps.

## Getting Started

### Prerequisites

- **Node.js** and **npm**: Install from [Node.js](https://nodejs.org/).
- **MetaMask**: Install the [MetaMask extension](https://metamask.io/) for your browser.

### Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/MoodDApp.git
   cd MoodDApp
   ```

2. Install `lite-server` globally if you haven't already:

   ```bash
   npm install -g lite-server
   ```

3. Start the local server:

   ```bash
   lite-server
   ```

   This will serve the `index.html` file on `http://localhost:3000`.

## Project Structure

```
MoodDApp/
├── index.html            # Main HTML file with the web interface and JavaScript code
├── mood.sol              # Solidity smart contract for storing and retrieving mood
├── README.md             # Project documentation
└── package.json          # Node.js package file (if applicable)
```

### Description of Files
- **index.html**: Contains the front-end code, including HTML for the user interface and JavaScript for interacting with the smart contract using `viem` and MetaMask.
- **mood.sol**: The Solidity contract that defines two functions, `setMood` and `getMood`, to store and retrieve mood data on the blockchain.
- **README.md**: Documentation file that explains the project, setup, and usage.
- **package.json**: (Optional) This file lists any dependencies and scripts for your project if you're using Node.js.

## Usage

1. **Deploy the Smart Contract**:
   - Open [Remix IDE](https://remix.ethereum.org/).
   - Copy the code from `mood.sol` and paste it into Remix.
   - Compile and deploy the contract on the Sepolia test network.
   - Note the contract address, as it will be used in the web interface.

2. **Configure the Front-End**:
   - Open `index.html` in a text editor.
   - Replace `MoodContractAddress` in the JavaScript section with your deployed contract's address.

3. **Run the dApp**:
   - Open `http://localhost:3000` in a browser.
   - Connect MetaMask to Sepolia network and authorize the dApp.
   - Enter a mood and click **Set Mood**. Confirm the transaction in MetaMask.
   - Click **Get Mood** to retrieve and display the stored mood.

## License

This project is open-source and available under the [MIT License](LICENSE).
