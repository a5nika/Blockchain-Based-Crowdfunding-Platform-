# Blockchain Based Crowdfunding Platform

## Description
This project is a simulation-based proof of concept that demonstrates how blockchain technology can improve transparency, accountability, and automation in crowdfunding systems. It replaces centralized intermediaries with smart contracts to enable trustless fund management and auditable transactions.

The system was developed and tested in a controlled local blockchain environment to validate core crowdfunding operations such as campaign creation, donations, fund withdrawal, and refunds.

## Methodology
The project follows an applied proof-of-concept approach rather than a purely theoretical or empirical study. A minimal blockchain-based crowdfunding prototype was designed to automate campaign workflows and financial transactions using smart contracts.

The system architecture consists of three main layers:
- **Frontend:** Built using HTML, CSS, and JavaScript to support campaign creation, donations, and real-time balance updates.
- **Blockchain Backend:** Implemented on Ethereum using Solidity smart contracts and deployed via Remix IDE.
- **Middleware API:** Developed using Node.js and Express to handle communication between the frontend and the blockchain network.

Ganache was used to simulate the Ethereum blockchain locally, enabling fast testing and debugging without gas costs.

## Smart Contract Design
The smart contract architecture is modular and includes two core components:
- **CampaignFactory:** Handles creation and indexing of crowdfunding campaigns. Each campaign is deployed as an independent contract instance.
- **Campaign:** Manages donations, funding goals, withdrawals, and refunds. Access control, validation checks, and event logging are used to ensure security and traceability.

The contracts implement basic security measures such as access restrictions and state updates to prevent common vulnerabilities.

## Simulation and Testing
The system was tested using Ganache with multiple pre-funded test accounts. Transactions were signed using MetaMask and executed through the deployed smart contracts.

Test cases covered:
- Campaign creation
- Donations before deadline
- Withdrawal after funding goal is reached
- Refunds for unsuccessful campaigns
- Rejection of unauthorized actions

All transactions were verified using transaction hashes, block numbers, and gas usage metrics.

## Results
The simulation demonstrated that:
- Valid donations were correctly recorded on the blockchain.
- Unauthorized or premature withdrawals were rejected.
- Funds were automatically released when campaign goals were met.
- Refunds were issued without manual intervention when goals were not achieved.
- All transactions were transparent and auditable through on-chain logs.

Transaction latency remained low in the local environment, and no successful security exploits were observed during testing.

## Technologies Used
- Ethereum
- Solidity
- Ganache
- Remix IDE
- MetaMask
- Node.js
- Express
- HTML
- CSS
- JavaScript

## Future Scope
- Integration with a production-ready frontend
- Deployment on public Ethereum test networks
- Multi-signature authorization and milestone-based fund release
- Compliance features such as KYC and decentralized identity support

## Keywords
Blockchain, Crowdfunding, Smart Contracts, Ethereum
