
!> Les étapes décrites ci-dessous partent du principe que vous avez déjà [installé Yoroi](Wallets/Yoroi/install.md)

Vous pouvez restaurer un wallet Yoroi ou un wallet papier Yoroi en utilisant votre phrase de récupération (mots secrets). Notez que les étapes ci-dessous s'appliquent *UNIQUEMENT* aux wallet Shelley. Les wallet Byron ou ITN peuvent être récupérés via les instructions figurant sur [cette page](Wallets/Yoroi/transfer.md)

Veuillez consulter les écrans ci-dessous pour connaître la procédure à suivre :

> Si vous avez déjà créé/restauré un wallet Shelley et que vous souhaitez en restaurer un autre, veuillez suivre les instructions [ici](Wallets/Yoroi/create.md#adding-or-switching-between-wallets), cliquez sur `Add New Wallet` et atterissez sur la page ci-dessous

Sélectionnez Restaurer un wallet sur l'écran d'accueil comme indiqué ci-dessous :

![Home Page](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-home.jpg ':size=50%')

Sélectionnez la devise `Cardano` :

![Currency](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-select-currency.jpg ':size=30%')

Il vous sera alors demandé de sélectionner le type de wallet à restaurer :

![Restore 1](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-restore-wallet-1.jpg ':size=30%')

Sélectionnez l'option appropriée en fonction du wallet que vous restaurez, et utilisez l'onglet ci-dessous pour les captures d'écran correspondantes :

<!-- tabs:start -->

#### ** Entrez une phrase de récupération de 15-mots **

Les wallets Yoroi et ADALite fournissent une phrase de récupération de 15 mots par défaut lors de la création d'un nouveau wallet `Hot`. Utilisez cette option si vous essayez de restaurer ce type de wallet Shelley. 
Actuellement, il existe deux types de phrase de récupération que vous pouvez restaurer. Pour simplifier l'utilisation, ne vous en tenez qu'à la restauration d'un portefeuille de `l'ère Shelley` pendant la restauration, comme indiqué en haut de ce document. L'option `Wallet Byron` n'est présente que pour l'historique des transactions (par exemple : la fiscalité), au cas ou vous en auriez besoin.

![Restore 15-word Shelley Wallet](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-restore-wallet-15-type.jpg ':size=30%')

Fournissez un nom de wallet pour l'identifier, entrez la phrase de récupération de 15 mots et sélectionnez un nouveau mot de passe de dépense que vous utiliserez pour ce wallet.

![Restore 15-word Shelley Wallet - details](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-restore-wallet-15-mnemonics.jpg ':size=30%')

#### ** Entrez une phrase de récupération de 24-mots **

Par défaut, Daedalus Mainnet vous fournit une phrase de récupération de 24 mots lorsque vous créez des wallet Shelley. Utilisez cette option si vous essayez de restaurer ce type de wallet.

Fournissez un nom de wallet pour l'identifier, entrez votre phrase de récupération de 24 mots, et sélectionnez un nouveau mot de passe de dépense que vous utiliserez pour ce portefeuille.

![Restore 24-word Shelley Wallet - details](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-restore-wallet-15-mnemonics.jpg ':size=30%')

#### ** Wallet Papier**

Yoroi vous permet de créer des wallets papier qui sont compatibles avec Shelley. Utilisez cette option si vous essayez de restaurer ce type wallet papier.

Fournissez un nom de portefeuille pour l'identifier, entrez la phrase de récupération de 21 mots ***de votre portefeuille en papier*** et le ***mot de passe du portefeuille en papier*** dont on vous a demandé de vous souvenir (notez que les deux sont essentiels, vous avez accepté les avertissements lors de la création de ce wallet papier - disant que vous devez présenter *ces deux informations* lors de la restauration), et sélectionnez un nouveau mot de passe de dépense que vous utiliserez pour ce portefeuille.

![Restore 24-word Shelley Wallet - details](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-restore-paper-wallet.jpg ':size=30%')

<!-- tabs:end -->

Vous verrez la somme de contrôle (checksum) de votre compte (comme une plaque d'immatriculation de voiture pour l'identification) et les adresses pour votre portefeuille de chaque ère/type pour vérification, cliquez sur `Confirm` :

![Verify wallet](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-restore-verify.jpg ':size=40%')

Félicitations ! Vous avez restauré votre wallet Shelley !