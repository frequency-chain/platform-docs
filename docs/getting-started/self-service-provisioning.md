Self-Service Provider Provisioning Guide
========================================

Introduction
------------

Welcome to the Frequency ecosystem's self-service provider provisioning guide. This comprehensive document will walk you through the steps required to become a Provider on Frequency, allowing you to build applications that leverage our decentralized social network protocol.

What is a Provider in the Frequency Ecosystem?
----------------------------------------------

A Provider is a pivotal entity in the Frequency ecosystem - typically an application or service that interfaces directly with the Frequency blockchain on behalf of users. Providers serve as the bridge between users and the blockchain, handling transactions, managing user delegations, and facilitating various operations that make the ecosystem function seamlessly.

### The Provider's Crucial Role:

-   **Delegated Authority**: Providers execute specific permissioned actions on behalf of users, ensuring security and transparency
-   **Content Management**: With user consent, Providers publish and update content such as posts, comments, and social interactions
-   **Social Graph Maintenance**: Providers help maintain users' social connections on Frequency based on user direction
-   **Content Storage Solutions**: Providers store user-generated content and write links to it on Frequency, with options including decentralized storage like IPFS
-   **Accessibility Enhancement**: By handling transaction complexities and fees, Providers make blockchain applications more accessible to non-technical users
-   **Seamless User Experience**: Providers offer intuitive interfaces that shield users from blockchain complexities

Self-Service Provisioning: Step-by-Step Guide
---------------------------------------------

### Step 1: Generate Your Frequency-Compatible Keys

Several wallet options can generate and secure your Frequency-compatible keys:

-   Polkadot Extension
-   Talisman
-   Other compatible wallets

This key generation process is essential for creating both your account and your Provider Account, which will be required for various transactions within the ecosystem.

### Step 2: Acquire Testnet Tokens

Using the account created in Step 1:

1.  Visit the Frequency Testnet Faucet
2.  Follow the simple prompts to receive Testnet tokens (XRQCY)
3.  These tokens will enable you to perform transactions on the testnet

### Step 3: Register as a Testnet Provider

Access the Provider Dashboard to establish your official Provider presence:

1.  Select "Testnet on Paseo" from the network dropdown
2.  Choose your Application Account from the available options
3.  Create an MSA (Message Source Account) and approve the transaction prompts
4.  Enter your Provider name - typically your company or application name

**Important**: Provider MSA IDs cannot be removed from the chain once registered, ensuring transaction verification integrity.

### Step 4: Acquire Capacity

"Capacity" enables you to perform certain transactions on Frequency without token cost. All user-behalf interactions can be conducted with Capacity.

To gain Capacity:

1.  Log into the Provider Dashboard
2.  Select "Stake to Provider"
3.  Stake approximately 100 XRQCY Tokens

### Step 5: Integrate Sign In With Frequency (SIWF)

To authenticate users through the Frequency ecosystem:

1.  Implement the SIWF integration following our developer portal documentation
2.  Test authentication flows using the Gateway support for SIWF
3.  Ensure your implementation handles user authentication and delegation properly

### Step 6: Gateway Integration

For content publication and social graph management:

1.  Review the Gateway documentation
2.  Implement the necessary API calls to interact with the Frequency Gateway
3.  Test content publication and retrieval in your testnet environment

Moving to Production
--------------------

When you're ready to transition from testnet to mainnet:

1.  Repeat steps 1-4 using the Mainnet selection in the Provider Dashboard
2.  Secure sufficient FRQCY tokens for production operations
3.  Implement Provider Boosting to enhance your application's performance and capabilities
4.  Consider integration with Community Rewards to incentivize user participation

Troubleshooting Common Onboarding Issues
----------------------------------------

### Wallet Connection Problems

-   **Issue**: Unable to connect wallet to the Provider Dashboard
-   **Solution**: Ensure your browser extension (Polkadot/Talisman) is properly installed and unlocked. Try refreshing the page or using an incognito window if connection issues persist.

### Transaction Failures

-   **Issue**: Transactions failing during MSA creation or Provider registration
-   **Solution**: Verify you have sufficient testnet tokens (at least 5 XRQCY for transaction fees). Check your network connection and ensure you're connected to the correct network (Testnet on Paseo).

### Capacity Not Reflecting

-   **Issue**: Staked tokens not converting to Provider Capacity
-   **Solution**: There may be a short delay in capacity reflection. Wait 5-10 minutes and refresh the dashboard. If the issue persists, try staking a small additional amount to trigger an update.

### Authentication Errors with Sign In With Frequency

-   **Issue**: Problems implementing SIWF for your users
-   **Solution**: Review the SIWF integration documentation thoroughly. The Frequency Developer Portal provides specific guides for SIWF phase 1 implementation.

### Gateway Integration Challenges

-   **Issue**: Difficulty connecting your application to the Frequency Gateway
-   **Solution**: Check the Gateway support documentation, which includes dedicated support for Sign In With Frequency functionality.

### Provider Dashboard Access Issues

-   **Issue**: Unable to access or use the Provider Dashboard features
-   **Solution**: Ensure you're using a compatible browser (Chrome or Firefox recommended). Clear cache/cookies if experiencing persistent UI issues. For technical support, reference the documentation available on frequency.xyz.

Technical Support and Resources
-------------------------------

Our ecosystem is expanding rapidly, with partners like MeWe already onboarding. The Frequency Developer Portal provides comprehensive documentation including quick start guides to help you integrate seamlessly with our ecosystem.

For developers looking to contribute more deeply to the ecosystem, join our "Builders" community category where you can access specialized resources and connect with fellow developers.

The Provider Provisioning Tools, including the Faucet, Testnet, and Provider Dashboard, are specifically designed to create a self-service experience for builders looking to launch on Frequency.

For technical assistance or questions about the provider onboarding process, check out frequency.xyz for the latest documentation, updated narrative, and provider dashboard access.

Coming Soon to the Frequency Ecosystem
--------------------------------------

-   Enhanced Gateway features with support for additional providers
-   Community Rewards integration possibilities
-   Threshold Cryptography for advanced privacy features

