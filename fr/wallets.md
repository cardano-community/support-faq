#### Qu'est-ce qu'un Wallet ?

Un portefeuille ou "wallet" est essentiellement un logiciel qui permet à l'utilisateur d'accéder à ses fonds sur la blockchain en utilisant ses clés privées. Vous pouvez utiliser différents portefeuilles, mais tant que vous utilisez la même clé privée, vous aurez accès aux mêmes fonds sur la blockchain. Dans l'écosystème Cardano, les portefeuilles sont de type `hiérarchique déterministe (HD)` et basés sur les "UTXO" - et ce pour de bonnes raisons. Avant de plonger dans ces termes, assurons-nous de clarifier les bases concernant les clés privées et leur sécurité.

#### Quelques bases à propos des clés privées

Une clé privée est essentiellement une chaîne de caractères numériques pouvant générer une clé publique, qui elle-même peut être "hashée" pour former des adresses. L'introduction des cryptomonnaies a été initiée par des utilisateurs souhaitant avoir un contrôle total, sans dépendre d'une entité externe (être sa propre banque). Cela signifie automatiquement que l'utilisateur est responsable de ses propres fonds, et qu'il lui incombe de conserver cette ou ces clés privées en toute sécurité. Si vous perdez vos clés privées, vous perdez essentiellement votre accès aux fonds numériques sur la blockchain, et personne (pas même les développeurs) ne pourra en récupérer l'accès.

Les meilleures pratiques pour sécuriser une clé privée dépendent de l'utilisation que chacun fait de son appareil. Il n'y a pas de règle d'or qui s'applique à tous. À l'heure actuelle, le fait d'avoir des clés en ligne est souvent source de vulnérabilités, qu'il s'agisse de la sécurité de votre appareil en ligne ou de l'accès à des serveurs physiques. Ainsi, une bonne pratique courante consiste à avoir vos clés privées hors ligne sur un support numérique. Vous ne voulez pas de clé privée non chiffrée ou sous un format facilement accessible sur votre appareil en ligne.

#### Portefeuilles Hiérarchiques Déterministes (HD)

Les portefeuilles  hiérarchiques déterministes (HD) permettent aux utilisateurs de dériver des clés (privées et publiques) à partir d'une information commune : la phrase mnémonique (Standard BIP39). Ces mots sont plus faciles à conserver et donnent de meilleures caractéristiques au portefeuille et à la confidentialité de l'historique. Cela signifie que vous pouvez recevoir une combinaison de mots (12, 15, 24, 25 ou 27 - selon le type de logiciel de portefeuille que vous choisissez) et le hachage de ces mots donne votre clé privée unique, ce qui en facilite l'accès et la sécurité. L'une des caractéristiques d'un portefeuille HD est qu'un seul ce des portefeuilles peut contenir jusqu'à 2147483647 comptes avec chacun 2147483647 adresses, le tout associé à un seul portefeuille - et chacun avec son propre historique unique de relevés de transactions.

Vous pouvez visiter [ce wiki](https://github.com/input-output-hk/cardano-wallet/wiki/About-Address-Derivation) pour plus d'informations sur les portefeuilles HD et comment la dérivation d'adresses fonctionne entre :

- HD Random / Byron Daedalus - les adresses commencent par `Ddz..`
- Byron / Icarus-style portfeuilles HD séquentiels - les adresses commencent par `Ae2..`
- Shelley wallets - toujours basé sur portfeuilles HD séquentiels, mais utilisant bech32 - les adresses commencent classiquement par `addr...`.

Vous constaterez peut-être qu'il existe différentes combinaisons de nombre de mots pour les mnémoniques prises en charge dans différents portefeuilles. Juste pour donner un bref résumé de quel type de portefeuille supporte combien de mots :

|Wallet            |Era      |Type      |Nombre de mots                 |
|------------------|---------|----------|-------------------------------|
|Daedalus          |Byron    |Hot/Online|12                             |
|Daedalus          |Byron    |Paper     |27 (18 sur papier + 9 digitaux)|
|Daedalus Rewards  |ITN      |Hot/Online|15                             |
|Yoroi             |Byron/ITN|Hot/Online|15                             |
|Yoroi             |Byron/ITN|Paper     |21 sur papier + Mot de passe   |
|Daedalus          |Shelley  |Hot/Online|24                             |
|Yoroi             |Shelley  |Hot/Online|24                             |

#### Fonds dans un portefeuille et fonds dans une adresse

L'une des confusions les plus courantes que les utilisateurs rencontrent est la lecture du solde d'un portefeuille HD, et les soldes contradictoires entre une adresse et un un portefeuille. Ceci est dû à la façon dont les porte-monnaie HD UTXO (Unspent Transaction Output) fonctionnent. Chaque nouvelle transaction dans un portefeuille sélectionne automatiquement un ensemble d'adresses qui forment un solde minimum pour effectuer le transfert, puis ajoute une *nouvelle* adresse de sortie (appelée UTXO) - qui elle, est une "adresse de change".
Le concept s'explique mieux en utilisant une analogie avec les billets de banque - tels qu'ils sont utilisés dans le système financier actuel.

Considérons qu'Alice a 3 billets de 10 euros chacun dans son sac à main, et qu'elle veut acheter 50 pommes à Bob au prix de 18 euros.
Alice paie Bob avec les deux billets de 10 euros, et reçoit une monnaie de 2 euros (qu'elle n'avait pas auparavant) comme nouveau produit non dépensé de cette transaction.
Alice se retrouve donc avec un billet de 10 euros et une monnaie de 2 euros - ajoutés à son sac à main. En vérifiant si son sac à main contient d'anciens billets, on obtient un billet de 10 euros - mais les fonds totaux de son sac à main comprennent également cette monnaie supplémentaire de 2 euros.

De même, lorsque vous effectuez une transaction à partir d'un portefeuille - les entrées sélectionnées seront souvent supérieures à la sortie et il faudra créer une monnaie.
Lorsque vous effectuez une recherche de fonds, si vous regardez la valeur d'une adresse, vous ne verrez peut-être pas le tableau complet, car le portefeuille est composé de nombreuses adresses, et les utilisateurs peuvent ne pas savoir quelle adresse contient combien de fonds après avoir effectué des transactions.
La meilleure façon d'interroger vos fonds est donc d'utiliser le logiciel de votre portefeuille, qui a accès à vos clés. Pour vérifier si des fonds sont arrivés à l'adresse B, l'explorateur est utile.
Pour plus de tétaisl, vous pouvez lire l'excellent [blog d'Emurgo](https://emurgo.io/en/blog/blockchain-primer-cardanos-utxo-model-simply-explained) qui rentre dans plus de détails sur les UTXOs.
