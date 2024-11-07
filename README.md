MoodDApp
A simple decentralized application (dApp) on Ethereum that allows users to set and retrieve their "mood" on the blockchain. This project serves as an introductory example of building a dApp, utilizing Solidity for the smart contract and a web interface for user interaction.

Table of Contents
Introduction
Features
Technologies Used
Getting Started
Project Structure
Usage
License
Introduction
MoodDApp is a decentralized application built on Ethereum's Sepolia test network. It allows users to store a mood on the blockchain through a simple web interface. Users interact with the dApp via MetaMask, which ensures secure transactions and data storage on the blockchain.

This project demonstrates how to develop and deploy a smart contract, connect it to a front-end web interface, and interact with the Ethereum blockchain using JavaScript and MetaMask.

Features
Set Mood: Store a mood on the blockchain.
Get Mood: Retrieve the stored mood from the blockchain.
Decentralized Storage: All mood data is stored on Ethereum’s Sepolia test network.
Technologies Used
Solidity: For writing the smart contract.
Remix IDE: For compiling and deploying the smart contract on the Sepolia test network.
JavaScript & HTML: For building the front-end interface.
Viem: A library for interacting with Ethereum and smart contracts.
MetaMask: A browser extension for managing Ethereum accounts and interacting with dApps.
Getting Started
Prerequisites
Node.js and npm: Install from Node.js.
MetaMask: Install the MetaMask extension for your browser.
Installation
Clone this repository:

bash
Copy code
git clone https://github.com/yourusername/MoodDApp.git
cd MoodDApp
Install lite-server globally if you haven't already:

bash
Copy code
npm install -g lite-server
Start the local server:

bash
Copy code
lite-server
This will serve the index.html file on http://localhost:3000.

Project Structure
bash
Copy code
MoodDApp/
├── index.html        # Main HTML file with the web interface
├── mood.sol          # Solidity smart contract for storing mood
└── README.md         # Project documentation
Usage
Deploy the Smart Contract:

Open Remix IDE.
Copy the code from mood.sol and paste it into Remix.
Compile and deploy the contract on the Sepolia test network.
Note the contract address, as it will be used in the web interface.
Configure the Front-End:

Open index.html in a text editor.
Replace MoodContractAddress in the JavaScript section with your deployed contract's address.
Run the dApp:

Open http://localhost:3000 in a browser.
Connect MetaMask to Sepolia network and authorize the dApp.
Enter a mood and click Set Mood. Confirm the transaction in MetaMask.
Click Get Mood to retrieve and display the stored mood.
License
This project is open-source and available under the MIT License.
