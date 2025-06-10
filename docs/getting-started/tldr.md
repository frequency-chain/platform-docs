```
# tl;dr with Frequency: Web3 Developer Portal

Welcome to the Frequency Developer Portal! This guide will help you quickly get up and running building decentralized applications on the Frequency blockchain. Whether you're a seasoned developer or new to decentralized technologies, Frequency's tools and APIs make it easy to create, interact with, and manage data in a decentralized way.

---

## What is Frequency?

Frequency is a purpose-built blockchain for decentralized applications. It provides robust primitives for decentralized identity, social graph management, content publishing, and more. Frequency is designed to empower developers to build the next generation of open, user-centric social platforms .

---

## Key Features

- **Decentralized Identity:** Manage users and authentication in a privacy-preserving, censorship-resistant way.
- **Social Graph:** Create and interact with open, composable user relationship graphs.
- **Content Management:** Publish, update, and interact with social content on-chain.
- **Web2 API Simplicity:** Developer Gateway offers familiar RESTful interfaces for easy integration.
- **OpenAPI/Swagger Support:** Rapidly prototype and document your integrations.
- **Optimized Docker Images:** Deploy services quickly and securely .

---

## Prerequisites

Before you begin, ensure you have:

- Basic familiarity with REST APIs and/or Web3 concepts
- [Docker](https://www.docker.com/get-started) installed (for running local services)
- [Node.js](https://nodejs.org/) (optional, for certain SDKs or tooling)

---

## Quick Start: Frequency Developer Gateway

The Frequency Developer Gateway is the fastest way to get started building on Frequency, providing microservices for account management, social graph operations, and content publishing with easy-to-use APIs .

### 1. Clone the Developer Gateway Repository

```bash
git clone https://github.com/projectlibertylabs/gateway.git
cd gateway

```

### 2\. Start the Gateway via Docker

```
docker compose up

```

This will spin up the key microservices:

-   **Account Service:** Manage users, authentication, and delegation.
-   **Graph Service:** Manage social connection data (follows, friendships).
-   **Content Publishing Service:** Create, update, and delete social posts/content.
-   **Content Watcher Service:** Receive webhooks for new/updated content .

* * * * *

Core API Workflows
------------------

### Account Service

-   **Create/Authenticate Accounts** (with SIWF)
-   **Manage Delegations**
-   **Create/Fetch User Handles**
-   **Key Management**

### Graph Service

-   **Fetch User Graphs**
-   **Update Connections (follow, friend)**
-   **Watch for Graph Updates**

### Content Publishing

-   **Create Posts, Replies, Reactions**
-   **Update/Delete Content**
-   **Attach Media (IPFS integration)**

### Content Watcher

-   **Register for Webhooks**
-   **Receive Content Notifications**

* * * * *

Example: Creating a Social Post
-------------------------------

```
curl -X POST http://localhost:<content-service-port>/posts\
  -H 'Authorization: Bearer <user-token>'\
  -d '{
    "content": "Hello, Frequency World!",
    "media": []
  }'

```

Replace `<content-service-port>` and `<user-token>` with your running service details and token.

* * * * *

Learn More
----------

-   [Frequency Official Documentation](https://docs.frequency.xyz/) - Deep dive into core concepts, architecture, and advanced topics .
-   [Developer Gateway API Reference](https://projectlibertylabs.github.io/gateway/index.html) - Full OpenAPI/Swagger docs and tutorials .
-   [Frequency Whitepaper](https://docs.frequency.xyz/) - Understand the vision and technology.

* * * * *

Community & Support
-------------------

-   **GitHub Issues:** Report bugs or request features.
-   **Security:** Found a vulnerability? [Report it securely](https://github.com/frequency-chain/frequency/security/advisories/new) 

* * * * *

Next Steps
----------

-   Explore code examples in the [Gateway repository](https://github.com/projectlibertylabs/gateway).
-   Build, test, and deploy your own decentralized social app.
-   Dive deeper into [Frequency Documentation](https://docs.frequency.xyz/) for advanced features and best practices .

* * * * *

Happy Building on Frequency! 🚀

```

**References:**
- : Overview - Frequency Documentation (https://docs.frequency.xyz/)
- : Introduction - Frequency Developer Gateway (https://projectlibertylabs.github.io/gateway/index.html)
- [[4]](https://poe.com/citation?message_id=401364267257&citation=4): Security Policy (Frequency GitHub)

```
