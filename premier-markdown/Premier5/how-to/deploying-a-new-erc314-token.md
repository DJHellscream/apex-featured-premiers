# Deploying a New ERC314 Token

Deploying a new ERC314 token on the APEX platform is a straightforward process designed to accommodate both novice and seasoned developers. This guide will walk you through the steps required to successfully deploy your own ERC314 token, including setting up token parameters, understanding fees, and managing your token post-deployment.

### Step-by-Step Guide to Token Deployment

#### 1. Prepare Token Details

Before initiating the deployment, you will need to prepare the following details:

* **Token Logo**: Upload a token logo with dimensions of 150x150 pixels to represent your token visually.
* **Token Name**: Define a unique name for your token that will be recognized on the blockchain.
* **Token Symbol**: Choose an abbreviation that will be used to represent your token on trading platforms.
* **Total Supply**: Specify the total number of tokens that will be created.
* **Owner Address**: Provide the wallet address that will own the token and control its distribution.
* **Trading Fee**: Set a trading fee ranging from 0% to 5%. This fee will be applied to all transactions involving your token on the platform.
* **Max Wallet %**: Determine the maximum percentage of the total token supply that any single wallet can hold. This helps prevent market manipulation and ensures a wider distribution of your tokens.

**Considerations:**

* Max Wallet % applies to both EOA (Wallet addresses) and Contract addresses. If you intend to implement staking features or want to allow other contracts to accept your ERC314 Max Wallet % will need to be adjusted accordingly.

#### 2. Understand the Costs

Deploying a token involves certain costs:

* **Deployment Fee**: For a limited unspecified amount of time there will be ZERO deployment fees!
* **Swap Fees:** A fee of up to 0.1% on each swap of the deployed contract.
* **Gas Costs**: Like any operation on the blockchain, deploying a token incurs gas fees, which are payments made to compensate for the computing energy required to process and validate transactions on the blockchain. These costs can vary based on the network's congestion at the time of deployment.

#### 3. Deployment Process

Once you have gathered your token details and prepared for the associated costs, follow these steps to deploy your token:

1. **Access the Create Page**: Connect your wallet to the APEX platform and navigate to the 'Create' page.
2. **Enter Token Details**: Fill in the forms with your token's details, including the logo, name, symbol, total supply, owner address, trading fee, and max wallet percentage.
3. **Review and Confirm**: Double-check all the information for accuracy. Errors in the token details can be irreversible once the token is deployed. Some information can be updated later that is contained in the metadata URI on the IPFS protocol. (These include token logo currently with more to be supported in the future)
4. **Pay the Deployment Fee**: Submit the deployment fee (as seen on the 'Create' page) along with the required gas costs.
5. **Deploy**: Confirm the transaction and initiate the token deployment. The platform will handle the technical process, and you will receive a confirmation once your token is live on the blockchain.

#### 4. Post-Deployment

After deploying your token, consider the following to manage and promote your token effectively:

* **Add Liquidity:** Add liquidity via the 'Manage' page to initialize the contract. Trading cannot begin until liquidity has been added.
* **Lock Liquidity:** If you choose, you can lock your liquidity using the locker under the 'Secure' page.&#x20;
* **Enable Trading:** On the 'Manage' page you can enable trading to allow users to swap for your ERC314 token. _**Once trading has been enabled it cannot be disabled**_.
* **Claim Fees:** On the 'Manage' page claim accrued fees if you have a trading fee set and enabled.
* **Monitor Transactions**: Keep an eye on the trading activity of your token. Tools on the APEX platform can help you track transactions and understand how your token is being used.
* **Engage the Community**: Use social media, forums, and other platforms to engage with potential users and investors. Community support is crucial for the growth and success of any new token.

### Conclusion

Deploying a new ERC314 token on the APEX platform provides a streamlined approach to entering the cryptocurrency market. By following the detailed steps outlined above and preparing for the associated costs, you can ensure a successful launch of your token.
