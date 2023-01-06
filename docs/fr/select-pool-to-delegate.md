Il n'y a pas un pool "bon pour tout le monde" sur lequel vous pouvez déléguer, sinon - chacun déléguerait dans le même pool et il n'y aurait pas de décentralisation :). Si de nombreux utilisateurs sont attirés par les pools dont les marges tarifaires sont les plus faibles, c'est généralement le facteur le moins important pour faire la distinction entre les Stake Pools. Vous trouverez ci-dessous quelques facteurs importants à prendre en considération.

> N'oubliez pas que vous - un délégataire - êtes indirectement l'un des éléments essentiels du protocole et que vos actions peuvent déterminer la décentralisation ainsi que l'adoption de la plate-forme. Que ce soit pour votre bénéfice ou celui du réseau, il est important que vous choisissiez avec soin les personnes à qui vous déléguerez.

!> Il y a de gros contributeurs à l'écosystème qui ne font peut-être pas de publicité et n'obtiennent pas assez de délégations, vous pouvez en savoir plus sur eux [ici](community-contrib.md) si vous souhaitez les soutenir.

Dans cette section, nous aborderons les différents aspects que les utilisateurs doivent prendre en considération lorsqu'ils choisissent les personnes qu'ils souhaitent soutenir. Si vous n'êtes pas sûrs de l'un des paramètres lors de la simple utilisation du portefeuille, veuillez tirer parti des plateformes communautaires construites pour vous aider dans la prise de décision. Ces plateformes sont :
- [Pooltool](https://pooltool.io)
- [ADAPools](https://adapools.org)
- [ADAStat](https://adastat.net)
- [CardanoScan](http://cardanoscan.io)
- [PoolPeek](https://poolpeek.com/)

La plupart de ces sites vous permettront de filtrer en utilisant divers paramètres et vous aideront à prendre votre décision. En outre, notez les points ci-dessous :

#### Point de saturation
  Afin de ne pas centraliser tous les enjeux dans un seul pool, après avoir atteint un certain enjeu en délégation (calculé par l'`offre totale en circulation/nOpt`) où nOpt est actuellement de 500, un pool ne sera plus récompensé pour une délégation plus importante. Ainsi, la part de récompense de chaque délégataire commencera à diminuer à mesure qu'une plus grande part sera déléguée à un tel pool.
    
#### Montant de l'enjeu dans un pool
  Un protocole de preuve d'enjeu attribue plus de blocs aux pools qui ont un enjeu plus élevé, jusqu'à ce qu'ils atteignent le `point de saturation`. Ainsi, si vous déléguez à un groupe n'ayant presque pas d'enjeu - à moins que vous ne déléguiez quelques millions, les chances que ce groupe fasse des blocs seront moindres - et vous ne gagnerez peut-être pas beaucoup de récompenses. Dans le même temps, notez que plus l'enjeu du pool est élevée, plus le rapport entre votre mise et la mise totale déléguée dans le pool sera faible, tout comme les récompenses que vous gagnerez. Idéalement, vous devriez vous situer entre 3 % et 60 % du point de saturation afin d'être situé dans un pool qui produit des blocs de manière constante et de ne pas perdre en termes de ratio de récompenses.

#### L'opérateur de pool  
  Lorsque vous déléguez dans un pool, la première chose que vous devriez connaître est l'opérateur du pool et sa présence dans la communauté. Lorsque les choses tournent mal, vous devriez pouvoir entrer en contact avec les propriétaires/opérateurs du pool. Pour la plupart des pools, des liens sociaux sont disponibles soit via le site web associé au pool, soit via des informations contenues dans les métadonnées. Bien que nous ne puissions pas juger ceux qui souhaitent rester anonymes, vous pouvez être certain que ceux qui ne le sont pas (anonymes) et qui existent depuis un certain temps ne mettront pas leur réputation en danger.  

#### Nombre de pools opérés par un opérateur
  Il existe quelques opérateurs qui gèrent plusieurs pools avec un marketing attrayant de frais peu élevés et de très faibles engagements. Bien qu'ils soient tout à fait dans leur droit de le faire - comme le permet le protocole - c'est quelque chose de controversé et cela est discutable. Ce que font ces groupes (peut-être involontairement) est un début d'[attaque Sibyl](https://en.wikipedia.org/wiki/Sybil_attack#:~:text=In%20a%20Sybil%20attack%2C%20the,diagnosed%20with%20dissociative%20identity%20disorder) sur le protocole. Le protocole est conçu pour avoir des incitations contre ce comportement, mais il ne fonctionne que sur si *un délégataire est rationnel*, en prenant soin de ne pas rendre ces pools trop puissants.

#### Moyens de communications
  Le plus souvent, les opérateurs de pool ajouteront des moyens d'abonnement à leurs chaînes (qu'il s'agisse de groupes de Telegram, de flux twitter ou de site web). Il est important de s'abonner à ces canaux pour des raisons telles que la modification du montant de l'engagement ou des frais. Ne pas le faire peut donner l'impression d'être pris au dépourvu lorsque l'on constate un changement des paramètres du pool. Si vous ne trouvez pas le moyen de joindre l'opérateur, vous pouvez remettre en question votre décision.

#### Classement des pools
  Le classement des pools dans Daedalus ne tient *PAS* compte de quelques facteurs (la chance associée à l'attribution des blocks, même si elle est proportionnelle à l'enjeu, le facteur de décentralisation ayant un impact un peu aléatoire), ainsi que du montant de l'enjeu que l'utilisateur voudrait déléguer. Il ne faut pas suivre cette procédure à l'aveugle, mais ce serait un bon point de référence pour les délégataires afin de voir dans quelle mesure le pool est désirable selon les spécifications originales des portefeuilles.  

#### Frais

  S'il n'est pas vraiment difficile de constituer un pool de base, la gestion avec une bonne sécurité, disponibilité, maintenance et visibilité demande du temps et des dépenses financières. Le protocole permet donc au pool de spécifier ses frais et de le faire sur la base d'un certain nombre de paramètres. En tant que délégataire, vous trouverez ci-dessous un aperçu des éléments à connaître lorsque vous examinez les frais de pool :

##### Engagement propre (pledge)
  L'engagement est essentiellement la promesse des propriétaires d'un pool de conserver leur avoirs dans leurs adresses de propriétaires du pool (donc, leur propre intérêt). Un montant plus élevé de cet engagement est récompensé par un montant plus élevé de récompenses pour tous les délégataires du pool. Cependant, il faut noter qu'avec les paramètres actuels du protocole, la différence globale de récompense n'est pas très importante. Si un pool engage l'équivalent de 100 000 $ ou de 1 million (par exemple, pour les hypothèses de base), alors déléguer 100 000 $ vers un pool de 100 000 $ pourrait vous rapporter 5159 alors qu'un pool indiquant 1 million d'engagement pourrait vous rapporter 5161 ADA par an. Cependant, déléguer sur un pool avec 10 millions d'engagements - en suivant les mêmes hypothèses - pourrait vous rapporter 5223 ADA pour un même scénario sur une année. Vous pouvez jouer avec les paramètres des engagements et leurs effets en utilisant le calculateur de mise en jeu de l'IOHK [ici](https://cardano.org/calculator).

##### Frais fixes
  C'est le minimum de récompenses qu'un pool gagnera avant que les récompenses obtenues pour les blocs signés soient distribuées à ses délégataires par le protocole. Les paramètres actuels du protocole imposent un minimum de 340 ADA comme coût minimum fixe. Cette redevance est appliquée afin d'éviter une course vers 0, ce qui n'est pas vraiment viable pour le protocole à l'avenir. Il est à noter que ce coût fixe est prélevé une seule fois sur la totalité du pot de récompense, et non pas pour chaque délégataire.

##### Marge variable (%)
  Il s'agit du pourcentage de récompenses qu'un pool pourra obtenir à partir du pot de récompenses total. Par rapport au pot de récompenses qu'un pool génère (par exemple : 10000 ADA), la récompenses d'un délégataire (par exemple : 2,5 % des récompenses totales du pool) n'est pas très affectée par la marge du pool : 1 % (soit 230,9 ADA) contre 4 % (224,9 ADA) n'affecte pas vraiment les récompenses du délégataire par une très grande marge, à moins que ce délégataire ne constitue une mise substantielle pour ce pool. Les récompenses sont surtout affectées par la loterie de l'attribution des slots (blocs à faire) et la performance du pool, beaucoup plus que par les différences de marge.

##### Performance  
  Il s'agit d'une estimation de la performance *supposée* d'un pool basée sur le montant d'enjeu et le nombre de blocs attendus par le calcul (la loterie rend cela en réalité un peu plus variable). Chaque bloc est récompensé par le protocole (jusqu'au point de saturation), ainsi un délégataire voudra dans l'idéal s'en tenir à un pool qui a plus de 80-85% de performance. Notez que nous ne pouvons pas dire de manière concluante que nous sommes à 100% ici, car les blocs réels effectués par les pools dépendront également du nombre de blocs qui ont été effectivement attribués à un pool. Il y a un peu de hasard dans l'attribution des blocs, comme une roulette réservant un nombre plus élevé de slots en fonction de l'enjeu total du pool.

Nous espérons que ce qui précède vous aidera à choisir un pool qui vous convienne. Si vous souhaitez voir des ajouts à cette liste, veuillez soulever un ticket en utilisant l'icône en haut à droite de la page.
