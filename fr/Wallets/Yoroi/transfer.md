Vous pouvez réclamer/transférer des fonds d'un wallet Byron ou ITN vers un wallet Shelley dans Yoroi.

!> Les étapes décrites ci-dessous partent du principe que vous avez déjà [installé Yoroi](Wallets/Yoroi/install.md) *ET* que vous avez soit  [créé un wallet shelley](Wallets/Yoroi/create.md) ou [restoré un wallet shelley](Wallets/Yoroi/restore.md) already.

Notez que les nombres de mots d'un wallet pour un ère donnée peuvent être trouvés [ici](wallets.md#heirarchical-deterministic-hd-wallets)

Cliquez sur l'icône `Claim / Transfer`sur la barre latérale, et sélectionnez le type de wallet (ère) que vous essayez de récupérer, comme indiqué ci-dessous :

![Claim / Transfer page](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-1.jpg ':size=40%')

Assurez-vous que vous avez 

#### Byron-era wallet

<!-- tabs:start -->

##### **Wallet Daedalus Ancien**

Ceci est pour les utilisateurs de Dédale (Wallet Hot + wallet papier + ou ceux qui ont accès à leur clé maître) Byron. Sélectionnez le type de portefeuille que vous essayez de restaurer comme indiqué ci-dessous :

![Claim / Transfer Byron Daedalus Wallets](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-2.jpg ':size=25%')

##### **Wallet Icarus/Yoroi**

Ceci est pour les utilisateurs de l'extension Yoroi/ADALite + mobile de l'ère Byron. Sélectionnez le type de wallet que vous essayez de restaurer :

![Claim / Transfer Byron Icarus/Yoroi Wallets](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-3.jpg ':size=25%')

*Utilisateurs de Ledger Byron : Notez qu'avec la version 3.2.2 de l'extension Yoroi, l'intégration de Ledger n'est pas encore prise en charge, et la saisie des clés de récupération du ledger est **non recommandés**. Vous pouvez  connecter votre Ledger à https://adalite.io (entièrement compatible avec les portefeuilles Yoroi), si vous ne pouvez pas attendre que cette fonctionnalité soit disponible.*

<!-- tabs:end -->

#### Wallet de l'ère Shelley (Récompenses du testnet Shelley ITN)

Cette option vous permet de récupérer les récompenses des wallets Yoroi (pour l'instant) en utilisant une phrase de récupération de 15 mots ou une clé-maître. Cela vous permet également de récupérer des récompenses ITN si vous y avez participé et que vous avez des récompenses à récupérer. Pour les utilisateurs de hardware wallet Ledger/Trezor et les wallets à phrase de récupération de 24 mots, vous pouvez retirer vos récompenses directement depuis l'onglet `Dashboard` dans le même wallet.

Pour procéder à la récupération, assurez-vous d'abord que votre wallet actif porte la mention `Shelley-standard wallet` dans la partie supérieure, comme indiqué ci-dessous :

![Claim Shelley Rewards](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-shelley-reward.jpg ':size=30%')

Il est recommandé d'avoir 10 ADA dans le wallet sur lequel vous réclamez les récompenses (même si les frais réels exigés seront probablement inférieurs à 1 ADA). Cliquez sur Wallet Shelley-Era et sélectionnez ensuite le choix approprié :

![Select type of reward to withdraw](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-shelley-reward-type.jpg ':size=25%')

##### Obtenir l'accès à une clé privée cryptée à partir d'extensions sur chromium

Si vous n'avez pas accès à vos mnémoniques, vous pouvez également saisir la clé privée de votre portefeuille Yoroi. Afin d'accéder à votre clé privée, ouvrez l'extension Yoroi dans votre navigateur et allez dans `Developer Tools`. Pour Chrome, vous pouvez naviguer comme indiqué ci-dessous :

![Yoroi Chrome Dev Tools](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/chrome-dev-tools.jpg ':size=30%')

Vous devriez voir un nouveau volet s'ouvrir. Allez dans l'onglet Application et naviguez jusqu'à "Storage > IndexedDB > yoroi-schema > Key". Vous devriez voir les identifiants de vos wallet. Lors de l'ouverture, vous devriez voir votre hash crypté que vous pouvez copier (et ensuite coller lorsque vous y êtes invité pour réclamer des récompenses Shelley comme ci-dessus) :

![Yoroi get encrypted private key](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-get-priv-key.jpg ':size=30%')

Notez que les clés sont cryptées à l'aide du mot de passe de dépense que vous utilisiez auparavant, et que vous devrez également saisir votre mot de passe de dépense même si vous utilisez le hash.

!> Vos wallets Shelley testnet (ITN) contenaient **seulement** vos récompenses, pas les fonds du réseau principal. Vos fonds Mainnet sont restés indépendants de ce qui s'est passé sur Shelley ITN - et si vous n'avez pris aucune mesure concernant vos fonds Mainnet depuis le 29 novembre 2019, vous pouvez toujours accéder à vos fonds Mainnet en utilisant la section [récupérer les fonds de l'ère Byron](#byron-era-wallet) ci-dessus.