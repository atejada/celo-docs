---
title: Run Secure Celo Nodes and Services
description: Recommendations for running secure Celo nodes and services.
---

# Run Secure Nodes and Services

Recommendations for running secure Celo nodes and services.

:::warning
As of block height 31,056,500 (March 26, 2025, 3:00 AM UTC), Celo is no longer a standalone Layer 1 blockchain—it is now an Ethereum Layer 2!
Some documentation may be outdated as updates are in progress. If you encounter issues, please [file a bug report](https://github.com/celo-org/docs/issues/new/choose).

For the most up-to-date information, refer to our [Celo L2 documentation](https://docs.celo.org/cel2).
:::

---

:::warning

Running Celo nodes and services securely, especially as part of running a validator, is of utmost importance. Failure to do so can lead to severe consequences including, but not limited to loss of funds, slashing due to double signing, etc.

:::

### RPC Endpoints

Celo nodes can be interacted with through an RPC interface for common interactions such as querying the blockchain, inspecting network connectivity and much more. The RPC interface is exposed via HTTP, WebSockets or a local IPC socket. There are two considerations:

1. There is no authentication in the RPC interface. Anyone with access to the interface will be able to execute any actions that are enabled with the command-line options. This includes sensitive RPC modules like `personal` which interacts with the private keys stored on the node (`admin` is another one). It is not recommended to enable RPC modules unless you explicitly need them. Other RPC modules might be less sensitive but could create unnecessary load on your machine (like the `debug` module) to execute a DoS attack.

2. If you do need access to the RPC modules (for example to use `celocli` or the attestation service), use a firewall and similar mechanisms to restrict access to the RPC interface. You almost never want the interface to be accessible from outside the machine itself.

### Public Endpoints

Beyond the RPC interface, Celo nodes and services have other interfaces that actually need to be exposed to the public internet. While varying degrees of protection exist within the software, such as validating attestation requests against the blockchain or monitoring connections in the discovery protocol, additional measures are recommended to reduce the impact of malicious traffic. Examples include, but are not limited to:

- **DDoS protection:** Protected public endpoints from a DDoS attack is highly recommended to allow valid requests to be served
- **Whitelist endpoints:** The attestation service exposes a [limited number of paths](https://github.com/celo-org/celo-monorepo/blob/master/packages/attestation-service/src/index.ts#L34) to function correctly. You could use a reverse proxy to reject paths that don't match them.
