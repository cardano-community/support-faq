#### What is a Wallet?

A wallet is a software program that creates, stores and manages access to the private and public key pairs that control funds on a blockchain.  You can use different wallets but, as long as you're using same private key, you would have access to the same funds on chain.  Wallets in the Cardano ecosystem are `Hierarchical Deterministic (HD)` and based on the `UTXO` model - and for good reasons. Before diving into these terms, lets review the basics regarding keys.

#### Basics about Private keys

A private key is a randomly generated string of characters that uses a specified algorithm and can be derived into a public key, which can go through hashing to form addresses. The introduction of Cryptocurrency is for users to be in complete control of their own funds without relying on any external entity (being your own bank). This automatically means it is an individual's responsibility to keep this private key(s) safe and secure. If one lose/share their private key(s), they essentially sole lose access to digital funds on blockchain, and no one (not even developers) can get those access back.

The best practices for securing your private key depend on individual's usage of their device. There isnt a golden rule that applies to all. Having keys online is often susceptible to vulnerabilities - be it security of your online device, or access to physical servers. Thus, a common good practice is having your private keys offline from any digitial media.

#### Heirarchical Deterministic (HD) Wallets

Hierarchical Deterministic (HD) wallets allow users to derive keys (private and public) from a common seed (built using [BIP39 mnemonics](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki)) that are easier to backup and allow better wallet features and privacy of history. This means you may receive a combination of words (12, 15, 24, 25 or 27 - dependening on type of wallet you elect) and the hash of these words actually result in your unique private key. One of the features of a HD wallet is that a single wallet can hold up to 2147483647 accounts with 2147483647 addresses, all associated to a single wallet - each with its own unique history of transaction records.

You can visit [this page](https://input-output-hk.github.io/cardano-wallet/concepts/address-derivation) for detailed information about HD Wallets and how address derivation works between:

  * HD Random (Legacy Byron Daedalus wallets - where addresses start with `Ddz..`).
  * Legacy Byron (Icarus-style HD Sequntial wallets - where addresses start with `Ae2..`).
  * Shelley wallets (still based on HD Sequential , but using bech32 - typical address starting with `addr...`).

You might see that there are number of different combination of number of words for mnemonics supported in different wallets. Just to give a brief summary of which wallet type supports how many seeds:

|Wallet              |Era      |Type      |Number of words                |
|--------------------|---------|----------|-------------------------------|
|Daedalus            |Byron    |Hot/Online|12                             |
|Daedalus            |Byron    |Paper     |27 (18 on paper + 9 digital)   |
|Daedalus Rewards    |ITN      |Hot/Online|15                             |
|Yoroi               |Byron/ITN|Hot/Online|15                             |
|Yoroi               |Byron/ITN|Paper     |21 on paper + Spending password|
|Daedalus            |Shelley  |Hot/Online|24                             |
|Yoroi/Eternl/Typhon |Shelley  |Hot/Online|15 / 24                        |

#### Funds in a wallet versus address

One of the common confusions users encounter is reading balance of a HD Wallet, and conflicting funds in an address versus funds in a wallet. This is because of the way UTxO (Unspent Transaction Output) HD Wallets operate. Every new outgoing transaction made from a wallet would select a set of inputs (which are essentially previous transactions), and then adds a *new* output address (referred to as change address) , adds transaction fees to submit to the chain. This unspent output transaction is referred to as UTxO

The concept is best explained by using an analogy with currency notes - as used in current financial system.

Let us consider Alice has 3 notes of 10 dollars each in her purse, and wants to buy 50 apples from Bob at a cost of 18 dollars.
Alice pays using both 10 dollar notes to Bob , and receives a change of 2 dollars (which she did not have before) as a new unspent output of this transaction.
Thus, Alice, now ends up with a 10 dollar note and a 2 dollar change - added to her purse. Checking her purse for old notes, will result in a 10 dollar note - but overall funds in her purse will also include that additional 2 dollar change.

Similarly, when you make a transaction from a wallet - the inputs selected will often exceed the output and a change will have to be created.
When querying funds, if you're looking at value of an address - you may not see the complete picture, because wallet is made up of many addresses, and users may not know which address has how much funds after making transactions.
Thus, best way to query your funds is using your wallet software , which had access to your keys. While to look at whether funds have reached to address B, explorer comes in handy.

For further details, you can read the excellent [blog from Emurgo](https://emurgo.io/en/blog/blockchain-primer-cardanos-utxo-model-simply-explained) which goes into moredetails about UTXO model.
