StashWish is a Web3 wishlist and savings-goal application. Users can create wishlist goals, track how much ETH they have contributed toward each goal, and view their savings progress through a dashboard. The project combines a React frontend with a Solidity smart contract.
Status: Educational/prototype project. Review and test the smart contract thoroughly before using it with real funds.

✨ Features
- Savings dashboard — view total saved, wishlist item count, goals reached, and goal progress.
- Wishlist management — create wishlist entries with a name, flair, and target amount.
- ETH contributions — contribute ETH toward a selected wishlist item through a connected wallet.
- Wallet integration — connect using MetaMask and approve blockchain transactions.
- On-chain storage — wishlist items and contributed amounts are stored through the StashWish Solidity contract.
- Animated interface — React, Framer Motion, and a Silk background component provide visual effects.
🧰 Tech Stack
Frontend
- React 19
- Vite
- React Router
- Ethers.js
- Framer Motion
- React Icons
- Three.js / React Three Fiber
- CSS Modules
Smart contracts
- Solidity ^0.8.20
- Hardhat
- MetaMask / injected EIP-1193 wallet provider
📁 Project Structure
StashWish/
├── stash-frontend/
│   ├── src/
│   │   ├── components/       # Navbar, wishlist cards, background
│   │   ├── config/           # Contract ABI and address configuration
│   │   ├── context/          # Wishlist state and contract interactions
│   │   ├── hooks/            # Wishlist-related hooks
│   │   ├── pages/            # Dashboard, Wishlist, Stake
│   │   ├── App.jsx
│   │   └── main.jsx
│   └── package.json
└── stash-contracts/
    ├── contracts/
    │   └── StashWish.sol
    ├── scripts/
    ├── test/
    └── hardhat.config.js
