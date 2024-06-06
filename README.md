# Web3Domains

Web3Domains is a decentralized domain name service built on the Ethereum blockchain, providing a secure and censorship-resistant way to manage domains and online identities. With Web3Domains, users have true ownership and control over their domain names, represented as non-fungible tokens (NFTs) on the Ethereum network.

![Web3Domains Process Flowchart](public/Flowchart.png "Web3Domains Process Flow")

The flowchart above illustrates the end-to-end process of registering and resolving a domain name using the Web3Domains service.

## How does Web3Domains works ? 

- Users list their domains for sale by interacting with the smart contract through the user interface. The smart contract likely holds the domain name, owner information, and price.
    
- When another user wants to buy a domain, they interact with the smart contract again, likely sending the required amount of Ether (cryptocurrency) to the contract.
    
- The smart contract then transfers ownership of the domain to the buyer and updates its internal records. The seller can then withdraw the funds from the smart contract using a separate function.

## Tech Stack

- **Solidity**: Smart contracts for domain registration, ownership, and resolution logic.
- **JavaScript**: Frontend application built with React.js and Ethers.js for blockchain interaction.
- **Hardhat**: Ethereum development environment for compiling, testing, and deploying smart contracts.


### Requirements

- [Node.js](https://nodejs.org/en/) (version 12 or later)
- [NPM](https://www.npmjs.com/) (comes bundled with Node.js)

## Installation

1. Clone the repository:

```bash
git clone https://github.com/web3domains/web3domains.git
```

2. Install dependencies:

```bash
cd web3domains
npm install
```

## Running Locally

1. Start a local Ethereum node:

```bash
npx hardhat node
```

2. Deploy the smart contracts:

```bash
npx hardhat run scripts/deploy.js --network localhost
```

3. Start the React frontend:

```bash
npm start
```

The application should now be running at `http://localhost:3000`.

## Testing

Run automated tests with Hardhat:

```bash
npx hardhat test
```

## Demonstrating the Process with MetaMask

Using MetaMask, a popular Ethereum wallet and browser extension, simplifies the interaction with Web3Domains. Here’s a step-by-step demonstration of the process:

1. **Install MetaMask**: Ensure you have MetaMask installed and set up in your browser.

2. **Connect MetaMask to Web3Domains**:
   - Open the Web3Domains application.
   - Click on the "Connect Wallet" button and select MetaMask.
   - Approve the connection in the MetaMask popup.

3. **Register a Domain**:
   - Navigate to the domain registration section.
   - Enter the desired domain name and submit the registration request.
   - Confirm the transaction in MetaMask. Once the transaction is confirmed on the blockchain, the domain is minted as an NFT and assigned to your Ethereum address.