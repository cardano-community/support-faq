Vous trouverez ci-dessous une liste de questions fréquemment posées au sein des canaux communautaires de Cardano sur les médias sociaux. Si vous ne trouvez pas de réponse à votre question, veuillez soulever un problème/PR en utilisant l'icône en haut à droite :smile:

#### J'ai délégué à un pool à l'époque `n`, quand vais-je recevoir des récompenses ? :id=reward-schedule
Pour tout changement de délégation, les récompenses sont perçues après 3 transitions d'époque (donc, après `15 à 20 jours`). Pour en savoir plus, consultez les détails ci-dessous :
- Une époque chez Cardano dure 5 jours. Tout changement de délégation est pris en compte lors d'un instantané à la fin de l'époque (à la 1ère transition d'époque).
- L'instantané capturé est considéré comme *vivant* à la prochaine (2ème) transition d'époque. Cela signifie que le pool auquel vous avez délégué reflète votre délégation dans les époques `n+2`, pour avoir la possibilité de faire des blocs proportionnels à sa participation (qui inclut maintenant votre délégation).
- Les blocs réalisés par le pool sont éligibles pour les récompenses, qui sont calculées à la transition de l'époque suivante (le calcul se fait donc à `n+3`).
- Enfin, les récompenses sont ensuite payées à la fin de l'époque `n+3`.
Ainsi, si vous avez délégué dans l'époque "n", vos récompenses seront avec vous au début de l'époque "n+4" (techniquement parlant, ce sera à la toute fin de l'époque `n+3`).
La représentation visuelle de l'explication ci-dessus est la suivante (en utilisant `n=213` dans l'exemple) :

  ![Rewards Schedule](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/rewards-schedule.jpg)

#### Rate-t-on des récompenses lorsque l'on change notre délégation pour un autre pool ? :id=change-delegation
Non.
Si vous changez de pool plusieurs fois au cours d'une même époque, seul le dernier changement sera enregistré lors de l'instantané de l'époque.
Si vous changez la délégation du pool `P1` vers le pool `P2`, vous continuez à recevoir des récompenses du groupe `P1` jusqu'à ce que le [calendrier des récompenses] (#reward-schedule) pour le pool `P2` commence.

#### Comment puis-je contrôler mes récompenses ? YoroI ou Daedalus ne montrent pas la distribution des récompenses par époque :id=monitor-rewards
Les portefeuilles ne peuvent actuellement pas afficher l'historique des récompenses en raison d'une API manquante qui devrait être disponible prochainement. En attendant, il existe plusieurs façons de surveiller vos récompenses, vous pouvez utiliser n'importe quelle adresse de votre portefeuille (peu importe laquelle, choisissez une adresse aléatoire dans votre portefeuille > onglet Recevoir) et suivre l'historique des récompenses en utilisant l'une des options ci-dessous :
- via un navigateur dans [pooltool](https://pooltool.io) ou [cardanoscan](https://cardanoscan.io).
- recevoir des notifications via [Pegasus Mobile App](https://pegasuspool.info/) sur votre téléphone portable
- obtenir des notifications Telegram via [ADAstat](https://t.me/AdaStatBot)

#### Je n'ai pas reçu mes récompenses bien qu'ayant suivi le calendrier. Que dois-je faire? :id=missing-rewards
Le premier point de contact est idéalement l'opérateur de votre pool. La plupart des opérateurs vous fournissent un moyen de les contacter. Voici quelques conseils pour en vérifier vous-même la cause :
- Si vous attendez des récompenses à l'époque x, vérifiez si des blocs ont été produits par le pool à l'époque x-2 (voir le calendrier [ci-dessus](#reward-schedule) pour plus de détails).  Vous pouvez utiliser n'importe quel [explorateurs de pools](explorers.md#list) et vérifier dans l'historique du pool les blocs effectués pour l'époque concernée.
- Si le pool a fait des blocs, mais que vous n'avez pas reçu de récompenses, vérifiez les paramètres du pool - si les frais fixes (le minimum par défaut est de 340 ADA) du pool sont supérieurs aux récompenses obtenues, un délégataire peut ne pas recevoir de récompenses.
- Si l'opérateur lui-même n'a pas reçu de récompenses, cela peut indiquer un problème dans la configuration de son pool, il vaut mieux le notifier le plus tôt possible.

#### Dois-je retirer mes récompenses et les déléguer à nouveau ? :id=withdraw-rewards
Les récompenses que vous gagnez sont automatiquement mise en jeu dans le cadre de votre délégation. Cela s'applique également à tout nouveau fonds reçu ou épuisé du portefeuille. Actuellement, votre portefeuille lui-même est délégué à un pool, tout changement survenu à l'époque `n` sera donc automatiquement pris en compte dans l'instantané et entraînera une mise à jour des récompenses à l'époque `n+4`. **Le seul moment où vous pouvez avoir besoin de retirer vos récompenses est lorsque vous déplacez tous vos fonds vers un autre portefeuille/plateforme d'échange.**

[pooltool]: https://pooltool.io
[cardanoscan]: https://cardanoscan.io
[adapools]: https://adapools.org
