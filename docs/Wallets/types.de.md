
Nun, da du dich damit vertraut gemacht hast, was eine Wallet ist, lass uns die Arten von Wallets erkunden, die du benutzen kannst. Bitte navigiere wie unten beschrieben, um einen bestimmten Wallet-Typ zu erkunden.

Aus Sicht des Endnutzers gibt es hauptsächlich zwei Arten von Wallet-Schnittstellen:

### Software (Hot) Wallets

Nun, da du dich damit vertraut gemacht hast, was eine Wallet ist, lass uns die Arten von Wallets erkunden, die du benutzen kannst. Bitte navigiere wie unten beschrieben, um einen bestimmten Wallet-Typ zu erkunden.

Aus Sicht des Endnutzers gibt es hauptsächlich zwei Arten von Wallet-Schnittstellen:

<!-- tabs:start -->

#### ** Full Node Wallet **

Beispiel: Daedalus

Eine Full-Node-Wallet betreibt einen komplett unabhängigen Blockchain-Knoten und bietet die Möglichkeit, die Wallet durch Abfragen des Knotens zu betreiben. Ein Beispiel für eine solche Wallet ist Daedalus. Es gibt einige Vorteile, einen solchen Knoten zu betreiben:
 - Die gesamte Blockchain-Historie ist lokal auf Ihrem Knoten verfügbar, um sie nach Ihren Bedürfnissen abfragen zu können.
 - Ihr Knoten wird alle Blöcke validieren, wenn sie erstellt und auf Ihr Gerät synchronisiert werden, wodurch - das für den Betrieb der Wallet erforderliche Vertrauen reduziert wird.
 - Das Betreiben eines vollständigen Knotens - verbessert auch die Verfügbarkeit der Blockchain in Ihrer geografischen Region und bietet eine bessere Latenz für die Blockerstellungs-Knoten.
 - Wenn es eine Funktion gibt, die vom Knoten unterstützt wird, aber noch nicht von einer Wallet-Benutzeroberfläche kannst du dich direkt mit dem Knoten verbinden und auf die Funktion zugreifen.

Neben diesen Vorteilen bringt der automatische Betrieb eines Knotens auch einige Pflichten mit sich, die aus Sicht des Endnutzers als unangenehm empfunden werden können - vor allem, wenn man nur Transaktionen durchführt:
 - Die Synchronisierung der gesamten Blockchain auf dem Gerät benötigt Zeit bei der Ersteinrichtung, die je nach Netzwerk- und Festplattendurchsatz des Geräts Stunden betragen kann.
 - Es gibt Speicher-, Arbeitsspeicher- und Netzwerkverpflichtungen, die erforderlich sind, um eine mit einem Full Node verbundene Wallet zu betreiben.
 - Full-Node-Wallets sind möglicherweise nicht ideal für mobile Geräte.
 
#### ** Light Wallet **

Beispiel: Yoroi, ADALite

Eine Light-Wallet verwendet eine Schnittstelle, die eine Verbindung zu einem entfernten Knoten für den Betrieb herstellt - und Sie somit von der Verantwortung entbindet, einen vollständigen Blockchain-Knoten zu betreiben. Diese können als Browser-Plugins/Erweiterungen, Websites oder mobile Apps verfügbar sein. Vorteile der Verwendung von Light-Wallets:
- Es ist nicht nötig, darauf zu warten, dass die gesamte Blockchain auf dem Gerät synchronisiert wird, um Transaktionen durchführen zu können, da man sich über die Wallet mit einem bereits laufenden, aktuellen Knoten verbindet.- Du behälst die Kontrolle über deine Schlüssel. Eine häufige Fehlwahrnehmung bei Light Wallets ist, dass sie unsicher sind, weil Ihre Schlüssel über das Netzwerk gesendet werden. Die meisten professionellen Light Wallets stellen sicher, dass die Schlüssel das Gerät nie verlassen und sich auch auf Ihrem Gerät immer in verschlüsseltem Zustand befinden. Bis zu diesem Punkt sollte dies nicht wirklich ein Unterscheidungsmerkmal für dich sein, um zwischen einer Full Node Wallet und Light Wallet zu unterscheiden, sie sind_beide so sicher wie dein Gerät._
- Du musst dich nicht um die Durchführung von Blockchain-Knoten-Upgrades kümmern, da dies auf der Server-Seite erfolgen kann.
- Light Wallets können leicht auf mobilen Geräten integriert werden.
- Sie sind in der Regel sehr schlank und haben keine hohen Anforderungen an Speicher oder ein stabiles Netzwerk.

Für offizielle Links zum Vergleich schaue dir bitte [diesen Support-Artikel](https://iohk.zendesk.com/hc/en-us/articles/360026058573-Daedalus-wallet-compared-to-Yoroi-wallet) von IOHK an.

<!-- tabs:end -->

### Papier (Cold) Wallets

Papier-Wallets sind im wesentlichen Wallets, die durch Software-Schnittstellen erstellt werden, aber so erstellt werden, dass die Schlüssel für diese Papier-Wallets nie online waren. Diese bieten in der Regel Seeds in zwei Teilen - ein Teil auf Papier gedruckt, und der andere Teil mit Worten (im Falle von Daedalus) oder einem Passwort (im Falle von Yoroi), das garantiert, dass selbst wenn jemand Zugang zu dem Papier hat, er nicht in der Lage sein wird, auf die Schlüssel zugreifen. Punkte, die zu beachten sind:
- Die Software, die das Papier-Wallet erstellt, wird keine ADA auf die erzeugte Wallet übertragen, es muss eine manuelle Transaktion ausgeführt werden.
- Wenn du dich, aus welchem Grund auch immer, dazu entscheidest, deine Papier-Wallet wiederherzustellen, wird deine Wallet auf einem digitalen Gerät, das online ist, wiederhergestellt und wäre damit keine "kalte" Wallet mehr. Daher wäre es in diesem Fall aus Sicherheitsgründen am besten, eine neue Papier-Wallet zu erstellen.

### Hardware (Cold) Wallets

Einen kurzen Überblick über die Funktionsweise von Hardware Wallets mit Yoroi findest du in [diesem](https://emurgo.io/en/blog/hardware-wallet-explanation-yoroi-keep-ada-safe) Blog von Emurgo.

