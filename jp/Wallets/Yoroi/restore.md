
!> The instructions below assume you've already [installed Yoroi](Wallets/Yoroi/install.md)

You can restore a Yoroi wallet or a Paper wallet in Yoroi using your recovery phrase. Note that the steps below apply *ONLY* to shelley wallets. Legacy (Byron/ITN) wallets can be claimed via instructions on [this page](Wallets/Yoroi/transfer.md)

Kindly check the screens below for the process:

> If you've already created/restored a Shelley wallet and would like to restore another shelley wallet, please follow instructions [here](Wallets/Yoroi/create.md#adding-or-switching-between-wallets) to click on `Add New Wallet` and reach the page below

Select Restore wallet on the home screen as shown below:

![Home Page](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-home.jpg ':size=50%')

Select currency as `Cardano`:

![Currency](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-select-currency.jpg ':size=30%')

You will now be asked to select the type of wallet to restore:

![Restore 1](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-restore-wallet-1.jpg ':size=30%')

Select the appropriate option based on wallet you're restoring, and use the tab below for corresponding screenshots:

<!-- tabs:start -->

#### ** Enter a 15-word recovery phrase **

Yoroi and ADALite wallets provide a 15-word recovery phrase as default when creating a new `Hot` wallet. Use this option if you're trying to restore such a shelley wallet. 
Currently, there are two types of Recovery phrase you can restore. For simplicity of usage, only stick to restoring `Shelley-era wallet` during restore. as noted at top of this document. The `Byron wallet` option is only present for transaction history (eg: taxation) purposes, should you need it.

![Restore 15-word Shelley Wallet](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-restore-wallet-15-type.jpg ':size=30%')

Provide a wallet name to identify your wallet, enter the 15-word recovery phrase, and select a new spending password that you will use for this wallet.

![Restore 15-word Shelley Wallet - details](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-restore-wallet-15-mnemonics.jpg ':size=30%')

#### ** Enter a 24-word recovery phrase **

Daedalus Mainnet by default provides you a 24-word recovery phrase when creating shelley wallets. Use this option if you're trying to restore such a wallet.

Provide a wallet name to identify your wallet, enter your 24-word recovery phrase, and select a new spending password that you will use for this wallet.

![Restore 24-word Shelley Wallet - details](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-restore-wallet-15-mnemonics.jpg ':size=30%')

#### ** Paper Wallet **

Yoroi allows you to create paper wallets that are shelley-compatible. Use this option if you're trying to restore such a shelley wallet.

Provide a wallet name to identify your wallet, enter the 21-word recovery phrase ***from your paper wallet*** and the ***paper wallet password*** that you were asked to remember (note that both are essential , you accepted warnings when creating paper wallets - saying you're responsible to have *both* when restoring), and select a new spending password that you will use for this wallet.

![Restore 24-word Shelley Wallet - details](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-restore-paper-wallet.jpg ':size=30%')

<!-- tabs:end -->

You will see account checksum (like a car number plate for identification) and addresses for your wallet from each era/type for verification, click `Confirm`:

![Verify wallet](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-restore-verify.jpg ':size=40%')

Congratulations! You've succesfully restored your Shelley wallet !!