## Wallets

- [What is a Wallet?](#what-is-a-wallet)
- [Private keys](#basics-about-private-keys)
- [Heirarchical Deterministic (HD) Wallets](#heirarchical-deterministic-hd-wallets)
- [Funds in a Wallet v/s Address](#funds-in-a-wallet-versus-address)

### What is a Wallet?

A wallet is essentially a software that grants users access to the funds on blockchain using their private keys. You can use different wallets, but as long as you're using same private key - you would have access to the same funds on blockchain. Wallets in cardano ecosystem are of *Hierarchical Deterministic (HD)* and based on *UTXO* - and for good reasons. Before diving into these terms, lets ensure the basics about Private keys and its security is clarified.

### Basics about Private keys

A private key is essentially a string of digital characters that can generate a public key, which can go through hashing to form addresses. The introduction of Cryptocurrency initiated with users being in complete control without relying on an external entity (being your bank). This automatically means user is responsible for his own funds, and it is an individual's responsibility to keep this private key(s) safe and secure. If you lose your private keys, you essentially lose your access to digital funds on blockchain, and no one (not even developers) can get your access back.

The best practices for securing your private key depend on individual's usage of his device. There isnt a golden rule that applies to all. In the current age, having keys online is often susceptible to vulnerabilities - be it security of your online device, or access to physical servers. Thus, a common good practice is having your private keys offline from a digitial media. You dont want any form of unencrypted or easily brute forcable format of private key on your online device.

### Heirarchical Deterministic (HD) Wallets

Hierarchical Deterministic (HD) wallets allow users to derive keys (private and public) from a common seed (mnemonics) that are easier to backup and allow better wallet features and privacy of history. This means you may receive a combination of words (12, 15, 24, 25 or 27 - dependening on type of wallet software you elect) and the hash of these words actually result in your unique private key, making it easier for access and security. One of the features of a HD wallet is that a single wallet can hold up to 2147483647 accounts with 2147483647 addresses, all associated to a single wallet - and each with its own unique history of transaction records.

You can visit [this wiki](https://github.com/input-output-hk/cardano-wallet/wiki/About-Address-Derivation) for detailed information about HD Wallets and how address derivation works between HD Random (Legacy Byron Daedalus wallets - where addresses start with Ddz..) and HD Sequential (Yoroi Wallets - where Addresses start with Ae2..) on current mainnet.

### Funds in a wallet versus address

One of the common confusions users encounter is reading balance of a HD Wallet, and conflicting funds in an address versus funds in a wallet. This is because of the way UTXO (Unspent Transaction Output) HD Wallets operate. Every new transaction within a wallet automatically selects a set of addresses that form a minimum balance to make the transfer, and then adds a *new* output address (referred to as UTXO above) - which is a "change address".
The concept is best explained by using an analogy with currency notes - as used in current financial system.

Let us consider Alice has 3 notes of 10 dollars each in her purse, and wants to buy 50 apples from Bob at a cost of 18 dollars.
Alice pays using both 10 dollar notes to Bob , and receives a change of 2 dollars (which she did not have before) as a new unspent output of this transaction.
Thus, Alice, now ends up with a 10 dollar note and a 2 dollar change - added to her purse. Checking her purse for old notes, will result in a 10 dollar note - but overall funds in her purse will also include that additional 2 dollar change.

Similarly, when you make a transaction from a wallet - the inputs selected will often exceed the output and a change will have to be created.
When querying funds, if you're looking at value of an address - you may not see the complete picture, because wallet is made up of many addresses, and users may not know which address has how much funds after making transactions.
Thus, best way to query your funds is using your wallet software , which had access to your keys. While to look at whether funds have reached to address B, explorer comes in handy.

For further details, you can read the excellent [blog from Emurgo](https://emurgo.io/en/blog/blockchain-primer-cardanos-utxo-model-simply-explained) which goes into moredetails about UTXO model.

