
Maintenant que vous vous êtes familiarisés avec la notion de portefeuille, nous allons explorer les types de portefeuilles que vous pouvez utiliser. Naviguez comme indiqué ci-dessous pour explorer un type de portefeuille spécifique.

En résumé, du point de vue de l'utilisateur final, il existe principalement deux types d'interfaces de portefeuille :

### "Software (Hot) Wallets"

Un portefeuille logiciel est une interface de portefeuille numérique où les clés cryptographiques (cryptées) seront stockées sur l'appareil que vous utilisez. Il existe principalement deux types de portefeuilles logiciels, comme indiqué ci-dessous.

<!-- tabs:start -->

#### ** "Full node wallet" ou Portefeuille à noeud complet **

Exemple: Daedalus

Un portefeuille nœud complet fait fonctionner un nœud de blockchain de manière indépendante et permet de faire fonctionner votre portefeuille en interrogeant le nœud. Un exemple de ce type de portefeuille est Daedalus. Il y a quelques avantages à faire fonctionner un tel nœud :
 - L'historique complet de la blockchain est disponible localement pour votre nœud, afin de pouvoir l'interroger selon vos besoins.
 - Votre nœud validera tous les blocs au fur et à mesure de leur création et de leur synchronisation avec votre appareil, ce qui réduira la confiance nécessaire pour opérer le portefeuille.
 - L'exécution d'un nœud complet améliore également la disponibilité de la blockchain dans votre région géographique, ce qui améliore la latence des nœuds de création de blocs.
 - Si une fonctionnalité est prise en charge par un nœud, mais pas encore par une interface utilisateur de portefeuille, vous pouvez vous connecter directement au nœud et accéder à la fonctionnalité.
 
Outre ces avantages, lancer un nœud implique automatiquement quelques responsabilités - ce qui peut être considéré comme un inconvénient du point de vue de l'utilisateur final - surtout si votre seul usage est d'effectuer des transactions :
 - La synchronisation de l'ensemble de la blockchain sur votre appareil nécessite du temps lors de la configuration initiale, ce qui peut prendre plusieurs heures selon le réseau et les capacités de votre ordinateur.
 - Il faudra du stockage, de la mémoire et un réseau nécessaires pour faire fonctionner un portefeuille connecté à un nœud complet.
 - Les portefeuilles à nœud complet peuvent ne pas être considérés comme idéaux pour les appareils portables.
 
#### ** "Light wallet" ou Portefeuille léger**

Exemple: Yoroi, ADALite

Un portefeuille léger utilise une interface qui se connecte à un nœud distant pour les opérations - vous libérant ainsi de la responsabilité de lancer vous-même un nœud complet de la blockchain. Ils peuvent être disponibles sous forme de plugins/extensions de navigateur, de sites web ou d'applications mobiles. Avantages de l'utilisation d'un portefeuille léger :
- Vous n'avez pas besoin d'attendre que toute la blockchain soit synchronisée sur votre appareil pour commencer à effectuer des opérations, car vous vous connectez à un nœud déjà à jour via votre portefeuille.
- Vous gardez le contrôle de vos clés. Une perception erronée courante avec les portefeuilles légers est qu'ils ne sont pas sûrs parce que vos clés sont envoyées sur le réseau. La plupart des portefeuilles légers professionnels garantissent que vos clés ne quitteront jamais votre appareil et qu'elles seront toujours cryptées, même sur votre appareil. Jusqu'à présent, cela ne devrait pas vraiment vous permettre de faire la différence entre un portefeuille complet et un portefeuille léger, ils sont tous deux aussi sûrs que votre appareil.
- Vous n'avez pas à vous soucier de la mise à niveau des nœuds de la blockchain, car cela peut être fait côté serveur.
- Les portefeuilles légers peuvent être intégrés facilement sur des appareils portables.
- Ils sont généralement très légers et n'ont pas d'exigences élevées en terme de stockage/mémoire ou de réseau.

Pour les liens officiels concernant la comparaison, veuillez consulter le site [suivant](https://iohk.zendesk.com/hc/en-us/articles/360026058573-Daedalus-wallet-compared-to-Yoroi-wallet) fait par I.O.G.

<!-- tabs:end -->

### "Paper (Cold) Wallets" ou Portefeuille papier

Les "portefeuilles papiers" sont essentiellement des portefeuilles créés par des interfaces logicielles, mais réalisés de telle manière que les clés de ces portefeuilles papiers n'ont jamais été mise en ligne. Ils sont généralement constitués de deux parties : une partie imprimée sur papier et une autre contenant des mots (dans le cas de Daedalus) ou un mot de passe (dans le cas de Yoroï) qui garantissent que même si quelqu'un a accès au papier, il ne pourra pas accéder à vos clés. Points à retenir :
- Le logiciel de création de portefeuille papier n'aura pas transféré de fonds vers un portefeuille généré, il doit s'agir d'une action manuelle.
- Si pour une raison quelconque vous décidez de restaurer votre portefeuille papier, celui-ci aura été restauré sur un appareil numérique qui est en ligne et ne sera plus un portefeuille "froid". Dans ce cas, il serait donc préférable de créer un nouveau portefeuille papier pour garantir à nouveau le même niveau de sécurité.

### "Hardware (Cold) Wallets" ou Portefeuilles matériels

Lisez [ce blog d'Emurgo](https://emurgo.io/en/blog/hardware-wallet-explanation-yoroi-keep-ada-safe) pour un bref résumé de la façon dont les Hardware Wallets fonctionnent avec Yoroi
