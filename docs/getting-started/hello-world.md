```
# HelloWorld 

This guide will show you how to publish your first piece of content to the Frequency decentralized social blockchain using the Frequency Developer Gateway.

---

## Prerequisites

- Docker installed (for running the Developer Gateway locally)
- Basic familiarity with REST APIs
- A (working) internet connection or localhost set up if running locally 

---

## Step 1: Start the Frequency Developer Gateway

The Developer Gateway provides easy-to-use REST APIs for interacting with Frequency's social layers: identity, graph, and content.
You can run it locally using Docker:

```bash
docker compose up

```

This will start several microservices, including:

-   **Account Service**: Manage users, authentication, and delegation
-   **Graph Service**: Manage social connections
-   **Content Publishing Service**: Create and manage social content
-   **Content Watcher Service**: Subscribe to content updates via webhooks

* * * * *

Step 2: Publish a "Hello World" Post
------------------------------------

Once the Content Publishing Service is running, you can create a post via a simple HTTP request.\
Replace `<content-service-port>` with your actual service port (default may be 8080), and `<user-token>` with a valid authentication token.

```
curl -X POST http://localhost:<content-service-port>/posts\
  -H 'Authorization: Bearer <user-token>'\
  -H 'Content-Type: application/json'\
  -d '{
    "content": "Hello, Frequency World!",
    "media": []
  }'

```

This command will publish "Hello, Frequency World!" as a new post on the Frequency blockchain .

* * * * *

What's Now?
------------

-   Explore user authentication and account creation (link to..)
-   Try making connections with the Graph Service (link to.. )
-   Subscribe to Content Watcher Service (link to.. )

For more in-depth tutorials and API details, check out:

-   [Frequency Developer Documentation](https://docs.frequency.xyz/)
-   [Developer Gateway Quick Start](https://projectlibertylabs.github.io/gateway/index.html)

* * * * *

Happy building on Frequency! 🚀

```
: Introduction - Frequency Developer Gateway
: Overview - Frequency Documentation

```
