Du kannst in Yoroi Guthaben von einer Byron- oder ITN-Wallet zu einer Shelley-Wallet übertragen. 

!> Die folgende Anleitung setzt voraus, dass du bereits [Yoroi installiert](Wallets/Yoroi/install.md) *und* entweder [eine Shelley-Wallet erstellt](Wallets/Yoroi/create.md) oder [eine Shelley-Wallet wiederhergestellt](Wallets/Yoroi/restore.md) hast.

[Hier](wallets.md#heirarchical-deterministic-hd-wallets) findest du weitere Infos zu den mnemonische Metriken der verschiedenen Wallets. 

Klicke auf das Symbol `Einfordern / Übertragen` in der Seitenleiste und wähle, die Ära der Wallet, die du einfordern möchtest, wie unten gezeigt:

![Claim / Transfer page](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-1.jpg ':size=40%')



#### Byron-Ära Wallet

<!-- tabs:start -->

##### ** Legacy Daedalus Wallet **

Dies ist für Nutzer von Daedalus Byron-Wallets (Hot Wallet + Papier-Wallet). Wähle den Typ der Wallet, die du wiederherstellen willst, wie unten beschrieben:

![Claim / Transfer Byron Daedalus Wallets](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-2.jpg ':size=25%')

##### ** Icarus/Yoroi Wallet **

Dies ist für Nutzer der Yoroi/ADALite-Erweiterung + Mobile Byron. Wähle den Typ der Wallet, die du wiederherstellen möchtest:

![Claim / Transfer Byron Icarus/Yoroi Wallets](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-3.jpg ':size=25%')

*Byron Ledger Nutzer: Beachte, dass für die Yoroi-Erweiterungsversion 3.2.2 die Ledger-Integration noch nicht unterstützt wird und die Eingabe der Ledger-Wiederherstellungsschlüssel **nicht empfohlen** wird. Du kannst Ledger mit https://adalite.io (voll kompatibel mit Yoroi-Wallets) verbinden, wenn du nicht warten möchtest, bis diese Funktion zur Verfügung steht.*

<!-- tabs:end -->

#### Shelley-Ära Wallet (Belohnungen aus dem Shelley Incentivised Testnet)

Mit dieser Option kannst du (im Moment) Rewards aus Yoroi-Wallets abheben, indem du deine 15-Wort-Wiederherstellungs-Phrase oder einen Hauptschlüssel verwendest. Damit kannst du auch ITN-Rewards abheben, wenn du am ITN teilgenommen hast. Nutzer von Ledger/Trezor- und 24-Wörter-Seed-Wallets können ihre Rewards über die Registerkarte `Dashboard` in derselben Wallet abheben.

Um mit der Wiederherstellung fortzufahren, vergewissere dich zunächst, dass auf deiner aktiven Wallet oben `Shelley-Standard Wallet` steht, wie unten dargestellt:

![Claim Shelley Rewards](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-shelley-reward.jpg ':size=30%')

Es wird empfohlen, dass du `10 ADA` in der Wallet hast, für die du Rewards beanspruchst (auch wenn die tatsächlich benötigten Gebühren wahrscheinlich weniger als 1 ADA betragen werden). Klicke auf Shelley-Era Wallet und wähle dann die entsprechende Option:

![Select type of reward to withdraw](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-shelley-reward-type.jpg ':size=25%')

##### Zugriff auf verschlüsselten privaten Schlüssel von Chromium-Erweiterungen erhalten

Wenn du keinen Zugang zu deinen Wiederherstellungs-Phrasen hast, kannst du dir auch den privaten Schlüssel deiner Yoroi-Wallet holen. Um auf den privaten Schlüssel zuzugreifen, öffne die Yoroi-Erweiterung in deinem Browser und gehe zu `Entwicklerwerkzeuge`. Für Chrome, kannst du wie unten beschrieben vorgehen:

![Yoroi Chrome Dev Tools](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/chrome-dev-tools.jpg ':size=30%')

Es sollte sich ein neues Fenster öffnen. Gehe auf die Registerkarte Anwendung und navigiere zu Storage > IndexedDB > yoroi-schema > Key. Du solltest die ID für deine Wallets sehen. Beim Erweitern solltest du deinen verschlüsselten Hash sehen, den du kopieren kannst (und dann einfügen, wenn du aufgefordert wirst, ihn für die Beantragung von Shelley-Belohnungen wie oben beschrieben einzufügen):

![Yoroi get encrypted private key](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-get-priv-key.jpg ':size=30%')

Beachte, dass die Schlüssel mit dem Ausgabe-Passwort verschlüsselt werden, das du vorher festgelegt hast. Beachte dass du bei der Verwendung des Hashes auch dein Ausgaben-Passwort eingeben musst.

!> Deine Shelley Testnet (ITN) Wallets enthalten **nur** deine ITN-Rewards, keine Mainnet-ADA. Deine Mainnet-ADA blieben unabhängig von dem, was im Shelley Incentivised Testnet passierte - und wenn du seit dem 29. November 2019 keine Aktionen an deinen Mainnet-ADA vorgenommen hast, kannst du immer noch darauf zugreifen, indem du den obigen Abschnitt [claim byron-era wallet](#byron-era-wallet) anwendest.