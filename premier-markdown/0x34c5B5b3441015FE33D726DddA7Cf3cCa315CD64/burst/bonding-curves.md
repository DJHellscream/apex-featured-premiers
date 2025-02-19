# 📊 Bonding Curves

#### How Apex Burst Bonding Curves Work

Similar to the **Liquidity Book** feature on Trader Joe, Apex Burst’s bonding curves use **bins** to hold token amounts and determine prices. When AVAX is exchanged for a token, tokens are distributed from a bin until it’s empty, then the process moves to the next available bin. Token prices increase by **20% per bin**, using a step-wise approach for a structured and incremental bonding curve.

This design allows **Apex Burst** to support multiple pricing strategies, offering flexibility for various token launches.

#### Curve Types Available on Apex Burst

On the **Create** page, Apex Burst provides several curve options:\


<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

1. **Linear Pricing**: Price increases linearly with supply. This curve offers predictable pricing where each additional token incrementally increases in cost.
2. **Carrying Capacity Curve (Logarithmic-like)**: Price rises quickly initially but levels off as supply increases. Early buyers face higher price increases, but later growth stabilizes, reducing further price jumps.
3. **Exponential Curve**: Price increases exponentially with supply. This curve rewards early participants, but prices escalate rapidly.
4. **Cubic Curve (Bell)**: Price increases rapidly at the start, consolidates in the middle, and rises again towards the end. This curve offers both early and late buyers opportunities, with a mid-point where prices stabilize.

#### Mathematical Formulas for Bonding Curves

**Price Calculation for Each Bin**

To calculate the price in each bin, the formula is:

$$
price = basePrice \times \left(1 + \frac{i \times x}{100}\right)
$$

Where `i` is the bin index (starting from 0), `basePrice` is the initial token price and `x` is the increment factor per bin.

**Calculating the Last Non-Zero Bin Price**

The price for the final bin with non-zero tokens is:

$$
{lastNonZeroPrice} = \text{basePrice} \times \left(1 + \frac{(n - 1) \times 20}{100}\right)
$$

Where `n` is the total number of bins and `x` is the increment factor. This helps determine the final bin price at the end of the distribution.

**Market Cap Calculation**

The market cap, representing the token’s final value on a DEX like Trader Joe, is calculated as:

$$
{requiredMarketCap} = \text{totalDistribution} \times \text{lastNonZeroPrice}
$$

**Fraction Validation**

To validate the fraction of total supply in the bins, use:

$$
{cumulativeValue} = \sum_{i=0}^{n-1} \text{lists}[i] \times \text{price}_i
$$

Then, the fraction is calculated as:

$$
{fraction} = \frac{10,000 \times \text{requiredMarketCap}}{\text{cumulativeValue} + \text{requiredMarketCap}}
$$

This formula ensures the allocation aligns with the desired distribution on the bonding curve and the total selected amount required for bonding.
