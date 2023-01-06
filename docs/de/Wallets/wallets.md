#### Was ist eine Wallet?

Eine Wallet ist eine Software, die den Zugriff auf die privaten und öffentlichen Schlüsselpaare erstellt, speichert und verwaltet, die die Gelder auf einer Blockchain kontrollieren.  Du kannst verschiedene Wallets verwenden, aber solange du denselben privaten Schlüssel verwendest, hast du Zugang zu denselben Geldern auf der Blockchain.  Die Wallets im Cardano-Ökosystem sind `Hierarchical Deterministic (HD)` und basieren auf dem `UTXO`-Modell - und das aus guten Gründen. Bevor wir in diese Begriffe eintauchen, lasse uns die Grundlagen bezüglich der Schlüssel besprechen.

#### Grundlegendes zu privaten Schlüsseln

Ein privater Schlüssel ist eine zufällig generierte Zeichenfolge, die einen öffentlichen Schlüssel erzeugen kann, der durch Hashing Adressen bilden kann. Die Einführung von Kryptowährungen begann damit, dass die Nutzer die vollständige Kontrolle haben wollten, ohne sich auf eine externe Instanz (Bank) zu verlassen. Dies bedeutet automatisch, dass der Nutzer für seine eigenen Gelder verantwortlich ist, und es liegt in der Verantwortung des Einzelnen, diese privaten Schlüssel sicher aufzubewahren und zu schützen. Wenn du deine privaten Schlüssel verlierst, verlierst du deinen Zugang zu deinen digitalen Geldern auf der Blockchain, und niemand (nicht einmal die Entwickler) kann deinen Zugang wiederherstellen.

Die besten Praktiken für die Sicherung deines privaten Schlüssels hängen von der Nutzung des Geräts durch den Einzelnen ab. Es gibt nicht die eine goldene Regel, die für alle gilt. Im heutigen Zeitalter ist die Online-Verwahrung von Schlüsseln oft anfällig für Schwachstellen - sei es die Sicherheit des eigenen Online-Geräts oder der Zugriff auf physische Server. Daher ist es eine gute Vorgehensweise, deine privaten Schlüssel offline auf einem digitalen Medium aufzubewahren. Du willst keine unverschlüsselten oder leicht zu entschlüsselnden Formate von privaten Schlüsseln auf deinem Online-Gerät haben.

#### Hierarchische Deterministische (HD) Wallets

Hierarchische Deterministische (HD) Wallets erlauben es Nutzern, Schlüssel (private und öffentliche) von einem gemeinsamen Seed abzuleiten ( unter Verwendung von BIP39 Mnemonics), die einfacher zu sichern sind und bessere Wallet-Funktionen und Privatsphäre der Historie ermöglichen. Das bedeutet, dass man eine Kombination von Wörtern erhält (12, 15, 24, 25 oder 27 - abhängig von der Art der Wallet-Software, die man wählt) und der Hash dieser Wörter tatsächlich den einzigartigen privaten Schlüssel ergibt, was den Zugriff und die Sicherheit erleichtert. Eines der Merkmale einer HD-Wallet ist, dass eine einzelne Wallet bis zu 2147483647 Konten mit 2147483647 Adressen enthalten kann, die alle mit einer einzigen Wallet verbunden sind - und jede mit ihrer eigenen einzigartigen Historie von Transaktionsdaten.

Du kannst [dieses Wiki](https://input-output-hk.github.io/cardano-wallet/concepts/address-derivation) besuchen, um detaillierte Informationen über HD Wallets zu erhalten und wie die Adressableitung funktioniert:
- HD Random (Legacy Byron Daedalus-Wallets - bei denen die Adressen mit `Ddz..` beginnen
- Legacy Byron Icarus-style HD Sequntial wallets - bei denen die Adressen mit `Ae2..` beginnen
- Shelley-Wallets (immer noch basierend auf HD Sequential, aber mit bech32 - typische Adresse beginnt mit `addr...`).

Du wirst sehen, dass es eine Reihe von verschiedenen Kombinationen der Anzahl von Wörtern für Mnemonics gibt, die in verschiedenen Wallets unterstützt werden. Nur um eine kurze Zusammenfassung zu geben, welcher Wallet-Typ wie viele Seeds unterstützt:

|Wallet            |Era      |Type      |Number of words                |
|------------------|---------|----------|-------------------------------|
|Daedalus          |Byron    |Hot/Online|12                             |
|Daedalus          |Byron    |Paper     |27 (18 on paper + 9 digital)   |
|Daedalus Rewards  |ITN      |Hot/Online|15                             |
|Yoroi             |Byron/ITN|Hot/Online|15                             |
|Yoroi             |Byron/ITN|Paper     |21 on paper + Spending password|
|Daedalus          |Shelley  |Hot/Online|24                             |
|Yoroi             |Shelley  |Hot/Online|15 / 24                        |

#### Guthaben in einer Wallet versus Adresse

Eine der häufigsten Verwirrungen, auf die Nutzer stoßen, ist das Ablesen des Guthabens einer HD-Wallet und der Konflikt zwischen Guthaben in einer Adresse und Guthaben in einer Wallet. Dies liegt an der Art und Weise, wie UTXO (Unspent Transaction Output) HD Wallets funktionieren. Jede neue Transaktion innerhalb einer Wallet wählt automatisch eine Reihe von Adressen aus, die ein Mindestguthaben bilden, um die Überweisung durchzuführen, und fügt dann eine *neue* Ausgabeadresse hinzu (oben als UTXO bezeichnet) - die eine "Wechseladresse" ist.
Das Konzept lässt sich am besten mit einer Analogie zu Geldscheinen erklären - wie sie im aktuellen Finanzsystem verwendet werden.

Nehmen wir an, Alice hat 3 Geldscheine zu je 10 Dollar in ihrem Portemonnaie und möchte von Bob 50 Äpfel zu einem Preis von 18 Dollar kaufen.
Alice bezahlt mit den beiden 10-Dollar-Scheinen an Bob und erhält ein Wechselgeld von 2 Dollar (das sie vorher nicht hatte) als neue, unverbrauchte Ausgabe dieser Transaktion.
Somit hat Alice nun einen 10-Dollar-Schein und 2 Dollar Wechselgeld in ihrem Geldbeutel. Wenn sie in ihrer Geldbörse nach alten Scheinen sucht, findet sie einen 10-Dollar-Schein - aber der Gesamtbestand in ihrer Geldbörse enthält auch das zusätzliche Wechselgeld von 2 Dollar.

Ähnlich verhält es sich, wenn du eine Transaktion von einer Wallet aus durchführst - die gewählten Eingaben werden oft die Ausgaben übersteigen und es muss eine Änderung erstellt werden.
Wenn der Wert einer Adresse abgefragt wird, kann es sein, dass man kein Gesamtbild sieht, weil die Wallet aus vielen Adressen besteht und die Nutzer nicht wissen, welche Adresse wie viel Geld hat, nachdem die Transaktionen durchgeführt wurde. Daher ist der beste Weg, das Guthaben abzufragen, die Verwendung der Wallet-Software, die Zugriff auf die Schlüssel hat. Um zu sehen, ob das Guthaben an Adresse B angekommen ist, ist der Explorer sehr hilfreich.

Für weitere Details kannst du den hervorragenden [Blog von Emurgo](https://emurgo.io/en/blog/blockchain-primer-cardanos-utxo-model-simply-explained) lesen, der auf das UTXO-Modell näher eingeht.
