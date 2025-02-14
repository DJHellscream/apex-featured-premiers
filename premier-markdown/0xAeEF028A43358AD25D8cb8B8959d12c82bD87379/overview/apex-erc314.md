# APEX ERC314

The original ERC314 contract and its predecessors offered many additional features over the standard ERC20 contract. However, many of those features were not fully fleshed out and had some flaws.

## Original ERC314

* **Simple MEV protection**: MEV Bots can work around the protection by using two separate wallets or contracts to perform sandwich attacks.
* **Single Liquidity Provider**: Only the owner of the ERC314 was able to add liquidity to the contract. This meant community members and other users could not contribute to the liquidity. This meant the liquidity was very thin and couldn't support large transactions.
* **Trading Fees**: The locked liquidity did not earn any fees. The industry standard is that some small percentage of each swap remains in the liquidity pool. This means the liquidity did not grow naturally from market volume as with traditional Liquidity Pools.
* **Proportional Swaps**: The calculations to perform swaps and add liquidity were based on proportional swaps instead of the constant product formula as commonly found on Uniswap and its clones.

## APEX ERC314 Improvements

The APEX version of ERC314 addresses these flaws and adds new features.

* **Enhanced MEV (bot) Protection**: By introduction slippage instead of simply relying on anti-MEV RPCs, APEX improves upon the MEV protection saving users from unnecessary losses.
* **Decentralized Liquidity**: Anyone can add liquidity to the pool thereby bolstering the number of tokens available for trading.&#x20;
* **Liquidity Tokens**: APEX's ERC314 also issues LP tokens as seen by traditional DEXes. This enables the Liquidity Provider to potentially use those tokens in other ways, e.g. staking, locking.
* **Liquidity Fees**: Liquidity providers also earn fees (0.2%) from all trades that occur. This is standard industry wide. This also means that the provided liquidity will grow over time.
* **Trading Fees**: Developers can set and modify a trading fee to grow their own treasury funds.
* **Flash swaps**: APEX also introduces an integral feature of Uniswap to ERC314 by enabling the ability for _**developers**_ to perform flash swaps.

APEX is the first ERC314 token to combine the tried-and-true features of a traditional DEX (Decentralized Liquidity, Fee earning, Constant product formula, and Flash swaps) into a single contract.
