
Starting with Yoroi (chromium extension) 3.10.0 release, Yoroi now supports Voting Center from your wallet.

To participate in a voting as an end user, remember there are 2 phases:
- Registering your wallet to receive voting power based on funds in a registered wallet at the time of snapshot (date is shared beforehand for each voting round)
- Actual voting which occurs after snapshot is taken and is done via mobile app.

For the current voting round (**fund-3**):
- Registration timeline is `17-Feb-2021 to 03-Mar-2021`
- Snapshot will be taken on `05-Mar-2021 23:23:00 GMT`.
- Minimum amount of ADA to register a wallet for voting is `2950 ADA`.
- Hardware Wallets cannot participate for voting in this round

#### Register for voting

In order to register a wallet for voting, kindly head to your wallet in Yoroi on chromium extension as below:

![Yoroi Voting tab](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/voting1.png ':size=50%')

You can install the Catalyst mobile app using the link shown on voting tab (links for [iOS](https://apps.apple.com/kg/app/catalyst-voting/id1517473397) and [Android](https://play.google.com/store/apps/details?id=io.iohk.vitvoting)).

![Android Catalyst install](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/mobilevoting1.png ':size=50%')

On the mobile, open the Catalyst voting App and follow through the introduction wizard, and select "Complete Registration" in mobile app as indicated below and go through the wizard.

![Mobile App - Complete Registration](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/mobilevoting2.png ':size=50%')
![Voting wizard](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/mobilevoting3.png ':size=18%')

Come back to the Yoroi Extension, and set up a pin code as below. Remember that you will be asked to use the same PIN on your mobile device. Keep this PIN safe with you.

![Set up PIN](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/voting2.png ':size=35%')

Enter your spending password as prompted (note that you will be prompted twice). You can leave the amount to 0. This will make your registration (it is a transaction on blockchain and will cost you typically ~ 0.17 ADA) on blockchain so that wallet is eligible to be captured as part of snapshot.

![Set up PIN](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/voting4.png ':size=35%')

You will now be presented a QR code on Yoroi extension. Scan this QR code using your catalyst app, as shown below:
!> Please ensure to backup this QR code as a screenshot, this is the *ONLY* way to restore your mobile access in case you lose your voting app.

![QR Code - extension](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/voting5.png ':size=35%')  

![Scan QR Code - Catalyst](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/mobilevoting4.png ':size=30%')

Enter the PIN on your catalyst app that was captured before to decode the QR code:

![Enter PIN](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/mobilevoting5.png ':size=30%')

This will land you back to home screen. Note that at this stage it is OK to have 0 against your voting power. The funds you would have on 5th March at the time of snapshot will decide your voting power.

![Completion](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/mobilevoting6.png ':size=30%')

The message above indicates that you have successfully completed your registration. The next step is to wait for the voting period to commence.

#### Frequently asked Questions :id=FAQ

##### I finished the voting. Where can I find list of voting proposals?

You will be able to vote from within your Catalyst app once the voting period begins. If you'd like to study other voting proposals meanwhile, you can 

##### The instructions here are for Yoroi, what if I use Daedalus?

Instructions for Daedalus integration is managed by IOG Zendesk support teams. The voting instructions can be found [here](https://iohk.zendesk.com/hc/en-us/articles/900004485866-Project-Catalyst-Fund3-voting-instructions) while their FAQ can be found [here](https://iohk.zendesk.com/hc/en-us/articles/900004448046-Catalyst-Fund3-FAQ).

##### Can I use Yoroi mobile for wallet registration?

No, voting is limited to Chromium/Firefox extensions for now.

##### Does participating to vote affect my staking rewards?

No, staking is not affected by whether you participate in voting process.

##### Can I use my hardware wallet?

Voting using Hardware wallet is actively under works, but unfortunately - atleast for this round, you cannot register a hardware wallet. Do checkout the query below

##### Can I move my funds from ledger/trezor to Yoroi wallet to register and move it back?

You can register an online wallet using minimal transaction fees, and then few minutes/hours before snapshot (`05-Mar-2021 23:23:00`) - transfer your funds from hardware device to this hot wallet. After a confirmation that snapshot is taken, you can move funds back to your hardware wallet. This will ensure that your staking process remains unaffected.

For any queries not answered by above, please check a more detailed FAQ [here](https://docs.google.com/document/d/1qYtV15WXeM_AQYvISzr0a0Qj2IzW3hDvhMBvZZ4w2jE) and make sure to join the [Catalyst chat](https://t.me/ProjectCatalystChat).
