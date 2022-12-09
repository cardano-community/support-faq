
The following is a list of well-known wallets to support Cardano.

Note that in case of issues, usually only queries relating to official wallets can be answered in Cardano groups across telegram/forum. You may need to consult with specific wallet support teams for third party wallets.

!!! Note ""

    - Its is important to know verify that you're in sole control of your wallet keys, and that the keys used can be restored in official wallets if a wallet provider is non-functional. Hence, put special attention to first two fields in table below.
    - The score column below is strictly a count of checks against each feature listed, the impact of specific feature (and thus, score) is up to reader's descretion.
    - The actual reliability (consistent uptime) of wallet is variable, and often dependent on network load. This metric is outside of scope for the table below (eg: recently, Yoroi has had trouble with consistency and bugs)
    - The table represents current state on mainnet network, any future roadmap activities are out-of-scope.
    - Non-Custodial (more specific for Cardano wallets) are wallets where payment as well as stake keys are not shared/reused by wallet provider, and funds can be transparently verified on explorer.

|Name         |[Type][1]|Score      |Non-Custodial          |Compatibility          |Stake Control          |Transparent Support    |Voting                 |Hardware Wallet        |Native Assets          |dApp Integration       |Mobile App             |Desktop (app,extension,web)                             |Open Source            |
|-------------|---------|-----------|-----------------------|-----------------------|-----------------------|-----------------------|-----------------------|-----------------------|-----------------------|-----------------------|-----------------------|--------------------------------------------------------|-----------------------|
|[Eternl]     |Light    |10         |:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|( :x:,:ballot_box_with_check:,:ballot_box_with_check: ) |:x:                    |
|[Yoroi]      |Light    |10         |:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:x:                    |:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|( :x:,:ballot_box_with_check:,:ballot_box_with_check: ) |[:ballot_box_with_check:](https://github.com/emurgo/yoroi-frontend)|
|[Flint]      |Light    |9          |:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:x:                    |:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:                    |( :x:,:ballot_box_with_check:,:ballot_box_with_check: ) |[Partial](https://github.com/dcSpark)                    |
|[Typhon]     |Light    |9          |:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:x:                    |( :x:,:ballot_box_with_check:,:ballot_box_with_check: ) |[Partial](https://github.com/StricaHQ)|
|[ADAlite]    |Light    |9          |:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:x:                    |:x:                    |( :x:,:x:,:ballot_box_with_check: )                     |[:ballot_box_with_check:](https://github.com/vacuumlabs/adalite)|
|[NuFi]       |Light    |8          |:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:x:                    |:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:x:                    |( :x:,:ballot_box_with_check:,:ballot_box_with_check: ) |:x:                    |
|[Daedalus]   |Full     |8          |:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:x:                    |:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:x:                    |:x:                    |( :ballot_box_with_check:,:x:,:x: )                     |[:ballot_box_with_check:](https://github.com/input-output-hk/daedalus)|
|[Nami]       |Light    |7          |:ballot_box_with_check:|:ballot_box_with_check:|:x:                    |:ballot_box_with_check:|:x:                    |:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:x:                    |( :x:,:ballot_box_with_check:,:x: )                     |[:ballot_box_with_check:](https://github.com/Berry-Pool/nami-wallet)|
|[Gero]       |Light    |7          |:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:x:                    |:ballot_box_with_check:|:ballot_box_with_check:|:x:                    |:x:                    |( :x:,:ballot_box_with_check:,:x: )                     |:x:                    |
|[LodeWallet] |Light    |6          |:ballot_box_with_check:|:ballot_box_with_check:|:x:                    |:x:                    |:x:                    |:x:                    |:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|( :x:,:ballot_box_with_check:,:x: )                     |:x:                    |
|[Coin Wallet]     |Light    |5          |:ballot_box_with_check:                    |:ballot_box_with_check:                    |:x:                    |:x:                    |:x:                    |:x:                    |:x:                    |:x:                    |:ballot_box_with_check:|( :ballot_box_with_check:,:x:,:ballot_box_with_check: )                     |[:ballot_box_with_check:](https://github.com/CoinSpace/CoinSpace)                    |
|[Medusav1]   |Light    |4          |:x:                    |:ballot_box_with_check:|:ballot_box_with_check:|:ballot_box_with_check:|:x:                    |:ballot_box_with_check:|:x:                    |:x:                    |:ballot_box_with_check:|( :x:,:x:,:ballot_box_with_check: )                     |:x:                    |
|[Atomic]     |Light    |4          |:ballot_box_with_check:|:ballot_box_with_check:|:x:                    |:ballot_box_with_check:|:x:                    |:x:                    |:x:                    |:x:                    |:ballot_box_with_check:|( :ballot_box_with_check:,:x:,:ballot_box_with_check: ) |:x:                    |
|[Exodus]     |Light    |2          |:x:                    |:x:                    |:x:                    |:x:                    |:x:                    |:x:                    |:x:                    |:x:                    |:ballot_box_with_check:|( :x:,:x:,:ballot_box_with_check: )                     |:x:                    |

[1]: types.md#software-wallets
[Daedalus]: https://daedaluswallet.io
[Yoroi]: https://yoroi-wallet.com
[ADAlite]: https://www.adalite.io
[NuFi]: https://nu.fi
[Typhon]: https://typhonwallet.io
[Eternl]: https://eternl.io
[Flint]: https://flint-wallet.com
[Medusav1]: https://adawallet.io/
[Nami]: https://namiwallet.io
[Atomic]: https://atomicwallet.io/
[Gero]: https://gerowallet.io
[Exodus]: https://www.exodus.io/
[LodeWallet]: https://lodewallet.io
[Coin Wallet]: https://coin.space
