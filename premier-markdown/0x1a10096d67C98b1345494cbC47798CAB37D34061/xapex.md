# 🦈 xAPEX

## A Yield-Bearing ERC4626 Token

xAPEX is an advanced ERC4626 token that offers users the ability to earn yield on their APEX tokens by staking them in a fully automated and efficient manner. Built on the ERC314 standard, xAPEX combines the benefits of ERC4626 with the foundational features of ERC314, ensuring compatibility and enhanced functionality. Below, we outline how xAPEX operates, its integrations, and its benefits to users and the Apex ecosystem.

### Key Features

* **Underlying Asset:** xAPEX represents staked APEX tokens, allowing users to deposit APEX and receive xAPEX in return.
* **Automated Yield Farming:** Deposited APEX is staked into the Single-sided APEX farm through the ChefStrategy contract.
* **Revenue Sharing:** Fees collected from the APEX DEX are converted to APEX and added to the xAPEX vault for enhanced yield.
* **Treasury Allocation:** A portion (10%) of AVAX gained from converting DEX fees is allocated to the Apex treasury to support ecosystem growth and sustainability.
* **Composability:** The ERC4626 standard allows xAPEX to integrate seamlessly into DeFi protocols, enabling holders to use their xAPEX tokens across the ecosystem while still earning APEX rewards.&#x20;

***

### How It Works

1. **Depositing APEX**
   * Users deposit APEX tokens into the xAPEX vault.
   * In return, they receive xAPEX tokens, which represent their share of the vault and automatically grow in value as yield is earned.
2. **Staking via ChefStrategy**
   * The APEX deposited is sent to the ChefStrategy contract.
   * ChefStrategy stakes these tokens into the Single-sided APEX farm, earning rewards for xAPEX holders.
3. **DEX Fee Integration**
   * Fees generated from trades on the Apex platform are routed to the ApexMaker contract.
   * ApexMaker converts these fees into APEX tokens.
   * Converted APEX is then deposited into the xAPEX vault, increasing the yield for all xAPEX holders.
4. **Treasury Contribution**
   * When tokens are sold to generate AVAX, 10% of the AVAX is allocated to the Apex treasury.
   * The remaining AVAX is converted to APEX and deposited back into the xAPEX vault to further enhance rewards.

***

### Benefits of Holding xAPEX

* **Compound Growth:** As rewards are reinvested and fees converted, the value of xAPEX relative to APEX grows over time.
* **Seamless Integration:** Users benefit from yield farming without the need for active management or multiple transactions.
* **Ecosystem Support:** Treasury contributions ensure that the Apex ecosystem remains robust and well-funded.
* **Transparency:** Built on the ERC4626 and ERC314 standards, xAPEX is fully compatible with DeFi protocols and composable with other yield strategies.

***

### Example Workflow

1. Alice deposits 1,000 APEX into the xAPEX vault.
2. ChefStrategy stakes her APEX into the Single-sided APEX farm. Assuming a staking reward rate of 10% annually, Alice’s 1,000 APEX earns 100 APEX over the course of a year.
3. DEX fees are collected and sent to ApexMaker. For example, if the DEX fees amount to 500 AVAX over a month, and 10% (50 AVAX) is allocated to the treasury, the remaining 450 AVAX is converted to APEX and deposited into the vault.
4. ApexMaker converts these fees into 450 APEX (assuming a 1:1 AVAX to APEX conversion rate) and deposits them back into the vault. Alice’s share of this yield increases the value of her xAPEX proportionally.
5. Over time, Alice’s xAPEX grows in value, reflecting the rewards earned from both staking (100 APEX) and DEX fees (her share of the 450 APEX deposited).
6. Alice can redeem her xAPEX for the underlying APEX at any time. For example, after one year, her xAPEX might represent a total of 1,550 APEX (staked rewards plus her share of the additional 450 APEX from DEX fees) depending on her share of the vault.

This detailed example clarifies how returns are calculated and distributed, demonstrating the combined impact of staking rewards and DEX fee integration on xAPEX holders.

***

### Technical Details

* **Standard:** ERC4626 (Yield-Bearing Vault Token)
* **Underlying Asset:** APEX
* **Contracts:**
  * **xAPEX Vault:** Manages deposits, withdrawals, and accounting for shares.
  * **ChefStrategy:** Handles staking in the Single-sided APEX farm.
  * **ApexMaker:** Converts DEX fees into APEX for reinvestment.
* **Treasury Allocation:** 10% of AVAX revenue is allocated to the Apex treasury before conversion.

***

#### Disclaimer

While the value of xAPEX relative to APEX can only increase over time due to the reinvestment of rewards and fees, there is no guarantee of return or profitability. Users should carefully consider the risks involved and only invest what they can afford to lose.

By utilizing xAPEX, users can maximize the utility and earning potential of their APEX tokens while contributing to the growth and sustainability of the Apex ecosystem.
