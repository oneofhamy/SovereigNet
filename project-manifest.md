/SovereigNet/
│
├── /docs/                          # Whitepapers, specifications, and design docs
│   ├── README.md                   # Intro to the documentation
│   ├── whitepaper.md              # Full updated project whitepaper
│   ├── roadmap.md                 # Full development roadmap (phased)
│   ├── project-manifest.md        # Full project manifest
│   ├── project-board.md           # Full project board
│   ├── architecture.md            # System design overview
│   ├── governance.md              # Voting and proposal system design
│   └── proof-of-humanity.md       # ZK + PoH integration design
│
├── /contracts/                    # Smart contracts (Solidity / Rust etc.)
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
│
├── /frontend/                     # Web interface and dApp
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
│   │   ├── state/                 # Recoil / Redux / Context
│   │   └── utils/
│   │       ├── zkHelpers.ts
│   │       └── ipfsUtils.ts
│   └── /public/
│       └── icons, logos, favicon, etc.
│
├── /p2p-network/                  # Peer-to-peer node infrastructure
│   ├── README.md
│   ├── ipfs-node-setup.md
│   ├── node-identity.ts
│   ├── message-protocol.ts
│   ├── content-routing.ts
│   └── encryption-layer.ts
│
├── /proof-of-humanity/           # ZK Proof system
│   ├── circuits/
│   │   ├── poh.zok
│   │   └── hashCircuit.zok
│   ├── snarkjs/
│   │   ├── generateProof.ts
│   │   └── verifyProof.ts
│   └── test/
│       └── poh.test.ts
│
├── /governance/                  # DAO tools, voting engine
│   ├── quadratic-voting.ts
│   ├── bracket-elimination.ts
│   ├── rewards-distributor.ts
│   ├── audit-logger.ts
│   └── validator-utils.ts
│
├── /cli-tools/                   # Developer CLI, utilities
│   ├── sovereign-cli.ts
│   ├── proposal-submit.ts
│   ├── zk-register.ts
│   └── vote-analyze.ts
│
├── /defi-integration/            # Liquidity, staking, DeFi protocols
│   ├── liquidity-pools.md
│   ├── defi-hooks.ts
│   ├── staking-contract.ts
│   └── reward-metrics.ts
│
├── /tests/                       # Unit + integration tests
│   ├── frontend/
│   │   └── App.test.tsx
│   ├── contracts/
│   │   ├── Voting.test.ts
│   │   └── Treasury.test.ts
│   └── governance/
│       └── QuadraticVoting.test.ts
│
├── /scripts/                     # Deployment and migration scripts
│   ├── deployContracts.ts
│   ├── setupGenesis.ts
│   └── migration.md
│
├── /static/                      # Static media, docs, assets
│   ├── whitepaper.pdf
│   ├── logo.svg
│   └── diagrams/
│
├── .env                          # Environment variables
├── .gitignore
├── README.md
├── LICENSE
└── package.json
