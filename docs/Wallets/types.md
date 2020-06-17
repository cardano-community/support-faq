## Types of Wallets

Now that you have familiarised with what wallet is technically, lets explore the types of wallets you can use. Please navigate as per below to explore specific type of wallet.

- [Software Wallets](#software-wallets)
  - [Full-Node Wallets](#full-node-wallet)
  - [Light Wallets](#light-wallet)
- [Hardware Wallets](#hardware-wallets)

To summarise from end user's point of view, there are primarily two types of wallet:

### Software Wallets:

A software wallet is a digital wallet interface where the cryptographic keys (encrypted) will be stored on the device you're using. Within software wallets, there are mainly two types of wallets as noted below.

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

A light wallet is a light-weight interface that connects to a remote node for operations - thus, relieving you of the responsibility to operate a full blockchain node. An example of such a wallet is Yoroi. Advantages of using light wallet:
- You do not need to wait for entire blockchain to be synched on your device to start performing operations, as you connect to an already running up-to-date node via your wallet.
- You remain in control of your keys. A common misperception with light wallets is that it is unsafe because your keys are sent over network. Most professional light wallets will ensure that your keys never leave your device, and are always in encrypted state even on your device. To this point, this shouldnt really be a differentiator for you to select between a full node wallet v/s light wallet, they're _both as safe as your device._
- You do not need to worry about performing blockchain node upgrades, as this can be done on the server end.
- Light wallets can be integrated easily on portable/handle devices.
- They're typically very lightweight, and do not have high storage/memory or stable network requirements.

For official links about the comparison, kindly visit [this support article](https://iohk.zendesk.com/hc/en-us/articles/360026058573-Daedalus-wallet-compared-to-Yoroi-wallet) from IOHK.

### Hardware Wallets:

> TODO

