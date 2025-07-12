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

Directories


/SovereigNet/
│
├── /docs/                          # 📚 Whitepapers, specifications, and design docs
│   ├── README.md                   # Intro to the documentation
│   ├── whitepaper.md              # Full updated project whitepaper
│   ├── roadmap.md                 # Full development roadmap (phased)
│   ├── architecture.md            # System design overview
│   ├── governance.md              # Voting and proposal system design
│   └── proof-of-humanity.md       # ZK + PoH integration design

├── /contracts/                    # 📜 Smart contracts (Solidity / Rust etc.)
│   ├── README.md
│   ├── Voting/
│   │   ├── Nomination.sol
│   │   ├── QuadraticVoting.sol
│   │   ├── RunoffElection.sol
│   │   └── VoteRewardDistribution.sol
│   ├── Treasury/
│   │   ├── CommunityChest.sol
│   │   ├── MultiSigWallet.sol
│   │   ├── EmergencyFreeze.sol
│   │   └── EscrowMilestone.sol
│   ├── Tokens/
│   │   ├── RewardToken.sol
│   │   ├── UtilityToken.sol
│   │   └── GovernanceToken.sol
│   └── Identity/
│       ├── ZKProofVerifier.sol
│       └── PoHRegistry.sol

├── /frontend/                    # Web interface and dApp
│   ├── /src/
│   │   ├── index.html
│   │   ├── App.tsx
│   │   ├── routes/
│   │   │   ├── Feed.tsx
│   │   │   ├── Profile.tsx
│   │   │   ├── GovernancePortal.tsx
│   │   │   └── VotePage.tsx
│   │   ├── components/
│   │   │   ├── PostComposer.tsx
│   │   │   ├── CommentThread.tsx
│   │   │   ├── EncryptedChat.tsx
│   │   │   ├── ProposalCard.tsx
│   │   │   └── VotingInterface.tsx
│   │   ├── state/               # Recoil / Redux / Context
│   │   └── utils/
│   │       ├── zkHelpers.ts
│   │       └── ipfsUtils.ts
│   └── /public/
│       └── icons, logos, favicon, etc.

├── /p2p-network/                # Peer-to-peer node infrastructure
│   ├── README.md
│   ├── ipfs-node-setup.md
│   ├── node-identity.ts
│   ├── message-protocol.ts
│   ├── content-routing.ts
│   └── encryption-layer.ts

├── /proof-of-humanity/          # ZK Proof system
│   ├── circuits/
│   │   ├── poh.zok
│   │   └── hashCircuit.zok
│   ├── snarkjs/
│   │   ├── generateProof.ts
│   │   └── verifyProof.ts
│   └── test/
│       └── poh.test.ts

├── /governance/                 # DAO tools, voting engine
│   ├── quadratic-voting.ts
│   ├── bracket-elimination.ts
│   ├── rewards-distributor.ts
│   ├── audit-logger.ts
│   └── validator-utils.ts

├── /cli-tools/                  # Developer CLI, utilities
│   ├── sovereign-cli.ts
│   ├── proposal-submit.ts
│   ├── zk-register.ts
│   └── vote-analyze.ts

├── /defi-integration/           # Liquidity, staking, DeFi protocols
│   ├── liquidity-pools.md
│   ├── defi-hooks.ts
│   ├── staking-contract.ts
│   └── reward-metrics.ts

├── /tests/                       # Unit + integration tests
│   ├── frontend/
│   │   └── App.test.tsx
│   ├── contracts/
│   │   ├── Voting.test.ts
│   │   └── Treasury.test.ts
│   └── governance/
│       └── QuadraticVoting.test.ts
├── /scripts/                     # Deployment and migration scripts
│   ├── deployContracts.ts
│   ├── setupGenesis.ts
│   └── migration.md

├── /static/                      # Static media, docs, assets
│   ├── whitepaper.pdf
│   ├── logo.svg
│   └── diagrams/

├── .env                         Environment variables
├── .gitignore
├── README.md
├── LICENSE
└── package.json

---

License

This project is licensed under the MIT License.

---

Get Involved

Check /docs/whitepaper.md and /docs/roadmap.md for details on the project's structure and goals.

Use the Project Board to view and contribute to open tasks.

Join the SovereigNet movement — decentralized, censorship-resistant, user-owned communication.
