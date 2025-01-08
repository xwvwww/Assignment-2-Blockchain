# AI Model Marketplace dApp
**Done by Almen Alnur SE-2315**

## Overview
The **AI Model Marketplace** is a decentralized application (dApp) developed for Assignment 2 of the Blockchain Technologies course. This dApp enables users to list, purchase, and rate AI models on a blockchain-powered marketplace.

### Features
- **List Models**: Users can add AI models with details such as name, description, and price.
- **Purchase Models**: Users can purchase listed AI models, transferring funds to the model creator.
- **Rate Models**: Users can rate purchased AI models, contributing to their overall rating.
- **Withdraw Funds**: Model creators can withdraw accumulated earnings from model sales.
- **View Model Details**: Users can retrieve detailed information about a specific AI model.

## Smart Contract Details
The project includes a smart contract written in Solidity:

### Contract Functions
1. `listModel(string memory name, string memory description, uint256 price)`
   - Allows users to list a new AI model.
2. `purchaseModel(uint256 modelId)`
   - Enables users to purchase an AI model by ID.
3. `rateModel(uint256 modelId, uint8 rating)`
   - Lets users rate a purchased AI model (1-5 stars).
4. `withdrawFunds()`
   - Allows the contract owner to withdraw accumulated funds.
5. `getModelDetails(uint256 modelId)`
   - Retrieves the details of a specific AI model.

## Frontend Integration
The frontend is built using JavaScript and interacts with the smart contract via **Web3.js**. It provides:

- A form to list AI models.
- A list of available models with purchase options.
- A form to rate purchased models.
- A button to withdraw funds for model creators.
- A detailed view for each AI model.

## Setup and Usage

### Prerequisites
- **Node.js**
- **Ganache**
- **MetaMask**
- **Remix IDE**
- **Visual Studio Code**

### Installation

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd <repository-name>
   ```

2. **Install dependencies**:
   Install Node.js packages and Truffle (globally if not already installed):
   ```bash
   npm install
   npm install -g truffle
   ```

3. **Install Web3.js**:
   Install the `web3` library:
   ```bash
   npm install web3
   ```

4. **Compile and migrate contracts** (if applicable):
   ```bash
   truffle compile
   truffle migrate
   ```

5. **Start the project** (if it includes a frontend):
   ```bash
   npm start
   ```

## Repository Structure
```plaintext
AIModelMarketplace/
├── contracts/
│   └── AIModelMarketplace.sol
├── frontend/
│   ├── app.js
│   └── index.html
├── README.md
└── LICENSE
```

## Demo Screenshots

**All Demo Screenshot is here ![Demo](AIModelMarketPlace/Usage)**

## Example Usage
1. **List a Model**:
   Fill out the form and click "List Model" to add an AI model.
2. **Purchase a Model**:
   Click the "Purchase" button for a specific model.
3. **Rate a Model**:
   Select a purchased model, rate it, and submit.
4. **Withdraw Funds**:
   Click "Withdraw Funds" to retrieve earnings.

## License
This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

## References
1. [Web3.js Documentation](https://docs.web3js.org/)
2. [Smart Contracts Guide](https://docs.web3js.org/guides/smart_contracts/smart_contracts_guide)
3. [Ganache Blockchain](https://trufflesuite.com/ganache/)
4. [Remix with Ganache and MetaMask](https://medium.com/@kacharlabhargav21/using-ganache-with-remix-and-metamask-446fe5748ccf)


