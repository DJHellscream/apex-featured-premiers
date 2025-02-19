# 🚰 Staking

## Burst Staking

**Stake Your Tokens to Earn LP Rewards**\
On the Burst page, users can stake their tokens to earn LP rewards generated from liquidity added after the bonding curve phase.

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption><p>This is for example purposes only</p></figcaption></figure>

***

### After Launch

Once a token successfully completes the bonding curve phase, all remaining tokens are added to liquidity pools and the selected reward LP tokens are sent to the Apex Burst Distributor for staking rewards.

### Reward Distribution

Stakers in Burst earn LP rewards at a rate of 0.25% per epoch (\~1% per day) based on their staked amount.

An LP yield farm also becomes available on the [Apex DeFi Earn](https://apexdefi.xyz/earn) page. Here you can earn the $APEX token.

### Flexible Reward Token Selection

Apex Burst allows the token creator to choose a reward token, offering a more flexible setup tailored to each project’s ecosystem.

***

#### Deposits & Withdrawals

**Depositing**\
Users can deposit any amount of tokens into Burst staking, and any unclaimed rewards are automatically claimed upon deposit.

**Withdrawing**\
An 8-epoch waiting period (starting from the last claim) is required before users can withdraw their staked tokens. Unclaimed rewards are automatically claimed during withdrawal.

**Emergency Withdrawals**\
Emergency withdrawals are available anytime, but they do not claim rewards automatically. This allows users to access staked tokens instantly, though without the added rewards from the last claim.

***

#### Calculating Rewards

Rewards are distributed to stakers based on their share of the total staked tokens. The contract distributes LP tokens at a rate of 0.25% per epoch to all stakers. For example:

* If Fred owns 1% of the total supply of a token in the Distributor and claims after 4 epochs, he can claim `4 * 0.25% * 1%` of the total LP balance in the Nursery.
* Assuming there are 10,000 LP tokens in the contract, Fred would receive 1 LP.

These rewards continue until the LP balance in the Nursery is depleted. This will occur after \~100 days.
