
!> Die folgenden Schritte setzen voraus, dass du Yoroi bereits [installiert](Wallets/Yoroi/yoroi.md#install) hast 

Du kannst eine Yoroi Wallet oder eine Papier-Wallet mit der Wiederherstellungs-Phrase in Yoroi wiederherstellen. Beachte, dass die folgenden Schritte *NUR* für Shelley Wallets gelten. Legacy (Byron/ITN) Wallets können über die Anweisungen auf [dieser Seite](Wallets/Yoroi/transfer.md) beansprucht werden.

Beachte bitte die unten aufgeführten Abbildungen für den Vorgang:

> Wenn du bereits eine Shelley Wallet erstellt/wiederhergestellt hast und eine andere Shelley Wallet wiederherstellen möchtest, folge bitte den Anweisungen [hier](Wallets/Yoroi/create.md#adding-or-switching-between-wallets) unter `Neue Wallet hinzufügen`

Wähle auf dem Startbildschirm die Option Wallet wiederherstellen, wie unten dargestellt:

![Home Page](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-home.jpg ':size=50%')

Als Währung `Cardano` auswählen:

![Currency](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-select-currency.jpg ':size=30%')

Du wirst nun aufgefordert, den Typ der wiederherzustellenden Wallet auszuwählen:

![Restore 1](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-restore-wallet-1.jpg ':size=30%')

Wähle die entsprechende Option basierend auf deiner Wallet, die du wiederherstellst:

<!-- tabs:start -->

#### ** Eingabe einer Wiederherstellungs-Phrase mit 15 Wörtern **

Yoroi und ADALite Wallets bieten eine 15-Wörter-Wiederherstellungs-Phrase als Standard, wenn eine neue `Hot` Wallet erstellt wird. Verwende diese Option, wenn du eine solche Wallet wiederherstellen möchten. 
Derzeit gibt es zwei Arten von Wiederherstellungs-Phrasen, die du wiederherstellen kannst. Der Einfachheit halber solltest du bei der Wiederherstellung nur die `Shelley-era wallet` wiederherstellen. Wie oben in diesem Dokument angegeben. Die Option `Byron Wallet` ist nur für Zwecke der Transaktionshistorie (z.B.: Besteuerung) vorgesehen, falls du sie benötigst.

![Restore 15-word Shelley Wallet](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-restore-wallet-15-type.jpg ':size=30%')

Gebe einen Wallet-Namen an, um deine Wallet zu kennzeichnen, gib die 15-Wörter-Wiederherstellungs-Phrase ein und wähle ein neues Auszahlungs-Passwort, das du für diese Wallet verwenden wirst.

![Restore 15-word Shelley Wallet - details](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-restore-wallet-15-mnemonics.jpg ':size=30%')

#### ** Eingabe einer Wiederherstellungs-Phrase mit 24 Wörtern **

Daedalus Mainnet bietet standardmäßig eine 24-Wörter-Wiederherstellungs-Phrase, wenn du Shelley-Wallets erstellst. Verwende diese Option, wenn du versuchst, eine solche Wallet wiederherzustellen.

Gebe einen Wallet-Namen an, um deine Wallet zu kennzeichnen, gib deine 24-Wörter-Wiederherstellungs-Phrase ein und wähle ein neues Ausgabe-Passwort, das du für diese Wallet verwenden wirst.

![Restore 24-word Shelley Wallet - details](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-restore-wallet-15-mnemonics.jpg ':size=30%')

#### ** Papier-Wallet **

Mit Yoroi kannst du Papier-Wallets erstellen, die Shelley-kompatibel sind. Verwendee diese Option, wenn du versuchst, eine solche Shelley Wallet wiederherzustellen.

Gebe eine Wallet Bezeichnung an, um deine Wallet zu kennzeichnen, gebe die 21-Wörter-Wiederherstellungs-Phrase ***von deiner Papier-Wallet*** und das ***Papier-Wallet-Passwort*** ein, das du aufgefordert wurdest, dir zu merken (beachte, dass beide essentiell sind, du hast Warnhinweise beim Erstellen der Papier-Wallet akzeptiert - die besagen, dass du dafür verantwortlich bist, *beide* zu haben, wenn du wiederherstellen willst), und wähle ein neues Ausgabe-Passwort, das du für diese Wallet verwenden wirst.

![Restore 24-word Shelley Wallet - details](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-restore-paper-wallet.jpg ':size=30%')

<!-- tabs:end -->

Du siehst die Kontoprüfsumme (wie ein Autokennzeichen zur Identifizierung) und die Adressen für deine Wallet aus jeder Ära/jedem Typ zur Überprüfung, klicke auf `Bestätigen`:

![Verify wallet](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-restore-verify.jpg ':size=40%')

Herzlichen Glückwunsch! Du hast deine Shelley Wallet erfolgreich wiederhergestellt !!
