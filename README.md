# NFTEarth Staking Rewards Program

## How is NFTE distributed?

The NFTE token distributions are controlled by the TokenDistributor contract that handles the issuance of new additions of NFTE tokens to two contracts:

Distributor contract (TokenDistributor) — It allows staking NFTE to earn NFTE tokens.

Splitter contract (TokenSplitter) — It receives NFTE tokens that are distributed in an asynchronous way ("splitted" based on predefined weights) to:

Trading rewards distributor contract (TradingRewardsDistributor).
 


# Two of the ways the NFTE token is distributed to users in the NFTEarth protocol to:

Stakers (FeeSharingSystem) — NFTE token holders can deposit LOOKS that are auto-compounded at each user interaction. This smart contract is an additional layer on top of the TokenDistributor contract, which also unlocks WETH rewards, stemming from the NFTEarth marketplace's protocol fee collected at every trade.

Traders (TradingRewardsDistributor) - Traders can collect rewards using a rolling Merkle-tree based system that distributes daily NFTE trading rewards based on volume activities (excluding private sale strategies). Computation of the trading rewards is done off-chain.


# ERC-1155 staking and ERC-721 staking to be added
