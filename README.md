SovereigNet GitHub Repository - README.md

Welcome to the SovereigNet repository; a fully decentralized, peer-to-peer encrypted social media platform designed for secure communication, democratic governance, and user sovereignty.

---

Overview

SovereigNet empowers users to:

Post, comment, and share media without centralized servers.

Participate in governance through quadratic voting and proposal-based decision-making.

Maintain full privacy using encryption and zero-knowledge proof identity systems.

Earn rewards for contributions, engagement, and moderation.

---

Project Setup

1. Install Dependencies

yarn install   # or npm install

2. Compile Smart Contracts

cd contracts
npx hardhat compile

3. Launch Local Blockchain

npx hardhat node

4. Deploy Contracts

cd scripts
npx hardhat run deployContracts.ts --network localhost

5. Start IPFS Node (optional for dev)

jsipfs daemon

6. Start Frontend

cd frontend
yarn dev

---

Key Directories

Directory	Purpose

/contracts	Smart contracts for voting, treasury, tokens, PoH

/frontend	dApp interface (React + Tailwind)

/p2p-network	P2P node protocol, messaging, encryption

/proof-of-humanity	ZK proof circuits and verifiers

/governance	Voting engine, runoff logic, audit trail

/defi-integration	Token utility, yield, and LP rewards

/docs	Whitepaper, roadmap, governance design

/cli-tools	Command-line tools for users and validators

/tests	Contract and frontend tests

/scripts	Deployment and genesis configuration

---

License

This project is licensed under the MIT License.

---

Get Involved

Check /docs/whitepaper.md and /docs/roadmap.md for details on the project's structure and goals.

Use the Project Board to view and contribute to open tasks.

Join the SovereigNet movement — decentralized, censorship-resistant, user-owned communication.
