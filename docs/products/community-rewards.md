Frequency Community Rewards Documentation
=========================================

Introduction
------------

Frequency Community Rewards is a strategic initiative designed to incentivize participation within the Frequency ecosystem. This documentation provides developers and providers with comprehensive information about implementing and leveraging the Community Rewards program within their applications.

Overview
--------

Community Rewards is a program that rewards both users and providers for specific actions that enhance the Frequency ecosystem, with a particular focus on interoperability between applications. The program is currently in development with planned launch and subsequent iterations.

Key Components
--------------

### Provider Rewards

Providers can earn rewards through several mechanisms:

-   When users create an MSA (Message Source Account), Universal Handle, and delegations through the provider 
-   When users who created their MSA through a provider subsequently delegate permissions to another provider within the Frequency ecosystem (interoperability rewards)
-   Rewards increase through a tiered system as activity increases 

### User Experience Points (XP)

While the primary focus is on provider rewards, a complementary XP system is being developed to:

-   Target end-users directly, distinct from the provider incentives
-   Reward ecosystem engagement rather than just technical integration 
-   Maintain flexibility in token allocation while building community momentum 

Implementation Guide
--------------------

### Provider Enrollment

To participate in the Community Rewards program as a provider:

1.  Sign up for the program at `rewards.frequency.xyz/providers`
2.  Complete the click-through agreement in the rewards provider dashboard 
3.  Ensure your application presents users with the option to interoperate with other providers in the ecosystem 

### Technical Integration

Implement the following to enable Community Rewards:

```
// Example code for tracking reward-eligible actions
function trackUserMSACreation(userId) {
  // Implementation details to track when a user creates an MSA
  // This would integrate with the Frequency rewards API
}

function trackUserInterop(userId, originatingProvider, newProvider) {
  // Implementation details to track when a user delegates to a new provider
  // This would integrate with the Frequency rewards API
}

```

### Payout Mechanism

Providers receive regular payouts based on user activity:

-   Rewards are distributed on a predefined schedule
-   The system tracks originating providers for user MSA creation
-   Interoperability actions are credited to the originating provider 

Community XP System
-------------------

The "Frequency Pulse" XP system complements the provider rewards by:

1.  Accelerating user acquisition and retention
2.  Driving meaningful ecosystem participation
3.  Creating positive token awareness and demand
4.  Establishing a foundation for long-term community growth
   
This system differentiates itself from existing incentives:

| Existing Incentives | Frequency Pulse XP System |
| --- | --- |
| Targets application developers | Targets end-users |
| Rewards concrete network utility | Rewards ecosystem engagement |
| Fixed, transparent token allocation | Deliberate ambiguity in token conversion |
| Focus on technical integration | Focus on community participation |
| Structured for predictable capacity | Structured for community growth |


Integration with Other Ecosystem Components
-------------------------------------------

### Sign In With Frequency (SIWF)

Community Rewards integrates with SIWF to track user authentication and delegation activities across providers.

[SIWF Documentation](https://github.com/frequency-chain/docs/tree/main/pages/authentication/sign-in-with-frequency)

### Provider Boosting

Community Rewards works alongside Provider Boosting, which is currently in development with both economics design and build phases planned.

[Provider Boosting Documentation](https://github.com/frequency-chain/docs/tree/main/pages/economics/provider-boosting)

### Token Support

The rewards system will initially be implemented with Frequency Access tokens, with plans to expand to the FRQCY token ecosystem.

[Token Integration Guide](https://github.com/frequency-chain/docs/tree/main/pages/economics/token-integration)

Community Engagement Features
-----------------------------

### Referral Program

A referral system enables users to earn rewards for inviting connections from projects within Frequency's ecosystem to explore other ecosystem applications.

### Ambassador Program

An ambassador program empowers highly engaged users to promote Frequency within their networks, creating grassroots advocacy.

### Co-marketing Campaigns

Shared initiatives across projects showcase the seamless interaction possible within Frequency's network, encouraging profile linking across platforms.

### "Find your Frequency" Challenges

UGC-styled contests where participants create content based on prompts, building community engagement.

Roadmap
-------

-   **Community Rewards Launch**: Scheduled in the development roadmap
-   **Community Rewards 2.0**: Planned for February 2025 
-   **Community Rewards Iterations**: Ongoing improvements following initial launch
  
API Reference
-------------

### Tracking User Actions

```
GET /api/rewards/track

```

Parameters:

-   `action_type`: The type of action being tracked (e.g., "msa_creation", "delegation")
-   `user_id`: The identifier for the user performing the action
-   `provider_id`: The identifier for the provider through which the action was performed
-   `secondary_provider_id` (optional): For interoperability actions, the identifier for the secondary provider

### Checking Provider Rewards

```
GET /api/rewards/provider/{provider_id}/summary

```

Response:

```
{
  "provider_id": "example_provider",
  "total_rewards": 1250,
  "tier": "Silver",
  "actions": {
    "msa_creations": 45,
    "interop_delegations": 23
  },
  "next_payout_date": "2025-03-15T00:00:00Z"
}

```

Testing and Development
-----------------------

For testing Community Rewards integration:

1.  [Set up a development environment](https://github.com/frequency-chain/docs/tree/main/pages/developers/getting-started/environment-setup)
2.  [Access the Testnet](https://github.com/frequency-chain/docs/tree/main/pages/developers/getting-started/testnet-access)
3.  Use test accounts to simulate user actions and verify reward tracking

Support and Resources
---------------------

-   [Developer Forum](https://github.com/frequency-chain/docs/tree/main/pages/community/forum)
-   [GitHub Repository](https://github.com/frequency-chain/docs)
-   [Discord Community](https://github.com/frequency-chain/docs/tree/main/pages/community/discord)
-   [Technical Support](https://github.com/frequency-chain/docs/tree/main/pages/support)

