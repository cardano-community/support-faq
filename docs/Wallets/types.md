## Types of Wallets

- [Hardware Wallets](#hardware-wallets)
- [Software Wallets](#software-wallets)
  - [Full-Node Wallets](#full-node-wallet)
  - [Light Wallets](#light-wallet)

To summarise from end user's point of view, there are primarily two types of wallet:

### Hardware Wallets:

> TODO

### Software Wallets:

> TODO

#### Full node wallet:

A full node wallet runs a complete independent blockchain node and provides capability to operate your wallet by querying the node. An example of such a wallet is Daedalus. There are a few advantages of running such a node:
 - The entire blockchain history is available locally to your node, to be able to query as per your needs.
 - Your node will validate all blocks as they're created and synchronised to your device, thereby - reducing the trust required to operate on wallet.
 - Running a full node - also enhances availability of the blockchain in your geograpical region, providing better latency for block making nodes.
 - If there is a feature supported by node, but not yet by a wallet UI - you can directly connect to the node and access the feature.

Alongwith those advantages, running a node automatically means a few responsibilities - which may be seen as a discomfor from end user's perspective - especially if your only usage is making transactions:
 - Synching entire blockchain on your device needs time when setting up initially, which could be hours depending on network and disk throughput of the device.
 - There are storage, memory and network commitments required to run a wallet connected to full node.
 - Full node wallets may not be considered ideal for portable/handheld devices.
 
#### Light wallet:

A light wallet is a light-weight interface that connects to a remote node for operations.

For official links about the comparison, kindly visit [this support article](https://iohk.zendesk.com/hc/en-us/articles/360026058573-Daedalus-wallet-compared-to-Yoroi-wallet) from IOHK.
