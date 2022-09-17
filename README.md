# Multisender Smart Contract

Download the repository.
Run: 

npm install

Create .env file to the root folder and put the private keys in this format or create variable of your own and update them in hardhat.config.js

MAINNET_PRIVATE_KEY = YOUR MAINNET PRIVATE KEY (AVAOID PUTIING HERE UNTIL YOU ARE DEPLOYING ON MAINNET AND TESTED ON TEST NETWORKS)
TESTNET_PRIVATE_KEY = YOUR TESTNET PRIVATE KEY (KEEP MAINNET AND TESTNET PRIVATE KEYS SPERATE)
BSC_API_KEY = YOUR CONTRACT VERIFICATION API KEYS. I OBTAINED FROM BSCSCAN.COM. CHECK ON DIFFERENT NETWORKS

# Deployment

# To deploy non upgradable version of Multisender smart contract.

Run: 

npx hardhat compile
npx hardhat run scripts/deploy_Multisender.jsx (will deploy on your default network configured in hardhat.config.js )

(--network bsctestnet for bsc testnet or bsc for mainnet or choose your own network)

Run to Verify smart contract:

npx hardhat verify "ADDRESS OF DEPLOYED SMART CONTRACT"

(--network bsctestnet for bsc testnet or bsc for mainnet or choose your own network)


# To deploy upgradable version of Multisender smart contract.

Run: 

npx hardhat compile
npx hardhat run scripts/deploy_MultisenderUpgradable.jsx (will deploy on your default network configured in hardhat.config.js )

(--network bsctestnet for bsc testnet or bsc for mainnet or choose your own network)

Run to Verify smart contract proxy and implementation both:

npx hardhat verify "ADDRESS OF DEPLOYED SMART CONTRACT PROXY"

(--network bsctestnet for bsc testnet or bsc for mainnet or choose your own network)



You are free to contribute in this smart contract, just pull the repository.
