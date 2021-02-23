You can claim/transfer funds from a Byron or ITN wallet to a shelley wallet in Yoroi.

!> The instructions below assume you've already [installed Yoroi](Wallets/Yoroi/install.md) *AND* you've either [created a shelley wallet](Wallets/Yoroi/create.md) or [restored a shelley wallet](Wallets/Yoroi/restore.md) already.

Note that wallet v/s era v/s mnemonics metrics can be found [here](wallets.md#heirarchical-deterministic-hd-wallets)

Click on the `Claim / Transfer` icon on the side bar, and select the era of wallet you're trying to claim as shown below:

![Claim / Transfer page](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-1.jpg ':size=40%')

Ensure that you've 

#### Byron-era wallet

<!-- tabs:start -->

##### ** Legacy Daedalus Wallet **

This is for Daedalus (Hot wallet + Paper wallet + those who have access to master key) Byron users. Select the type of wallet you're trying to restore as per below:

![Claim / Transfer Byron Daedalus Wallets](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-2.jpg ':size=25%')

##### ** Icarus/Yoroi Wallet **

This is for Yoroi/ADALite extension + mobile Byron users. Select the type of wallet you're trying to restore:

![Claim / Transfer Byron Icarus/Yoroi Wallets](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-3.jpg ':size=25%')

*Byron Ledger Users: Note that as of Yoroi extension version 3.2.2, Ledger integration is not supported yet, and entering the ledger recovery keys is **not recommended**. You can connect ledger to https://adalite.io (fully compatible with Yoroi wallets), if you cannot wait for this feature to be available.*

<!-- tabs:end -->

#### Shelley-era Wallet (Rewards from Shelley Incentivised Testnet)

This option is to withdraw rewards from Yoroi wallets (for now) using 15-word recovery phrase or master key. This also allows you to withdraw ITN rewards if you had participated and have some rewards to recover. For ledger/trezor and 24-word seed based wallet users, you can withdraw your rewards from `Dashboard` tab within same wallet.

To proceed with recovery, first ensure that your active wallet at the top says `Shelley-standard wallet` as per below:

![Claim Shelley Rewards](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-shelley-reward.jpg ':size=30%')

It is recommended that you have `10 ADA` in the wallet you're claiming rewards to (even though actual fees required is probably going to be less than 1 ADA). Click Shelley-Era Wallet and then select the appropriate choice:

![Select type of reward to withdraw](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-shelley-reward-type.jpg ':size=25%')

##### Getting access to encrypted Private key from chromium extensions

If you do not have access to your mnemonics, you can also grab the private key of your Yoroi wallet. In order to access your private key, open Yoroi extension in your browser and go to `Developer Tools`. For Chrome, you can navigate as per below:

![Yoroi Chrome Dev Tools](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/chrome-dev-tools.jpg ':size=30%')

You should see a new pane open up. Go to Application tab and navigate to Storage > IndexedDB > yoroi-schema > Key. You would see the ID for your wallets. Upon expanding, you should see your encrypted hash that you can copy (and then paste when prompted to paste for claiming Shelley rewards as per above):

![Yoroi get encrypted private key](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-get-priv-key.jpg ':size=30%')

Note that the keys be encrypted using spending password you used before, and using the hash will also need you to enter your spending password.

!> Your Shelley testnet (ITN) wallets **only** contained your rewards, not mainnet funds. Your mainnet funds remained independent of what happened on Shelley Incentivised Testnet - and if you did not take any actions to your Mainnet funds since 29th Nov 2019, you can still access your mainnet funds using [claim byron-era wallet](#byron-era-wallet) section above.