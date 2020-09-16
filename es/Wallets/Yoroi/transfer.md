Puedes reclamar/tranferir fondos desde una billetera de Byron/ITN a una billetera de Shelley en Yoroi.

!> Las siguientes instrucciones asumen que ya has [instalado Yoroi](es/Wallets/Yoroi/install.md) *Y* ya has [creado una billetera de Shelley](es/Wallets/Yoroi/create.md) **O** [restaurado una billetera de Shelley](es/Wallets/Yoroi/restore.md).

Nota que la billetara versus la era versus las métricas mnemotécnicas pueden ser encontradas [aquí](es/wallets.md#heirarchical-deterministic-hd-wallets)

Has click en el ícono `Claim / Transfer` en la barra lateral, y selecciona la era de la billetera que intentas reclamar:

![Claim / Transfer page](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-1.jpg ':size=40%')

Asegúrate que tengas:

#### Billetera de la Era Byron

<!-- tabs:start -->

##### ** Billetera Daedalus Legacy **

Esta sección es para los usuarios de Byron Daedalus (Billetera caliente + billetera de papel + acceso a la llave maestra (master key). Selecciona el tipo de billetera que intentas restaurar como se indica acontinuación:

![Claim / Transfer Byron Daedalus Wallets](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-2.jpg ':size=25%')

##### ** Billetera Icarus/Yoroi **

Esta sección es para los usuarios de la extensión de Yoroi/ADALite + usuarios móviles de Byron. Selecciona el tipo de billetera que intentas restaurar:

![Claim / Transfer Byron Icarus/Yoroi Wallets](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-3.jpg ':size=25%')

*Usuarios de Byron Ledger: Nota que apartir de la versión 3.2.2 de la extensión de Yoroi, la integración Ledger toadavía no es compatible, e introducir las llaves de restauración de Ledger ***no es recomendado***. Puedes conectar tu Ledger a https://adalite.io (completamente compatible con las billeteras de Yoroi), si no desea esperar a que esté presente esta característica.*

<!-- tabs:end -->

#### Billetera de la Era Shelley (Recompensas de Shelley Incentivised Testnet ITN)

Esta opción es para reclamar las recompensas de las billeteras de Yoroi (por los momentos) usando tu frase de restauración de 15 palabras o la llave maestra. Esto igual te permite reclamar las recompensas de la ITN si participaste y tiene recompensas por reclamar. Para ledger/trezor y billeteras con claves de 24 palabras, puede reclamar tus recompensas desde la pestaña `Dashboard` dentro de la billetera respectiva.

Para continuar can la frase de restauración, primeramente asegúrate que la parte superior de tu billetera activa diga `Shelley-standard wallet` como se muestra acontinuación:

![Claim Shelley Rewards](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-shelley-reward.jpg ':size=30%')

Es recomendado que tengas `10 ADA` en la billetera a la cual enviarás las recompensas (aún cuando el costo actual requerido probablemente sea menor a 1 ADA). Haz click en `Shelley-Era Wallet` y luego selecciona la opción adecuada:

![Select type of reward to withdraw](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-shelley-reward-type.jpg ':size=25%')

##### Obteniendo acceso desde la extensión chromium a tu llave privada encriptada

Si no tienes acceso a tus mnemotécnicos, puedes obtener la llave privada de tu billetera Yoroi. Para ello, abre la extensión de Yoroi en tu explorador y dirígete a `Developer Tools`. Para Chrome, puedes navegar como se muestra acontinuación:

![Yoroi Chrome Dev Tools](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/chrome-dev-tools.jpg ':size=30%')

Deberías de ver un nuevo pánel. Ve a la pestaña `Application` y navega a `Storage > IndexedDB > yoroi-schema > Key`. Verás las IDs de tus billeteras. Si expandes la opciones, deberías de ver tu hash encriptado, el cual puedes copiar (y luego pegar cuando se te pida al reclamar las recompensas de Shelley como mencionamos anteriormente):

![Yoroi get encrypted private key](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-get-priv-key.jpg ':size=30%')

Noata que las llaves puedes ser encriptadas usando la contraseña que utilizaste anteriormente, y utilizar el has también te pedirá introducir tu contraseña.

!> Tus billeteras de Shelley testnet (ITN) **solamente** contienen tus recompensas, no los fondos de la mainnet. Tu fondos de la mainnet permanecerán de manera independiente de lo que sucedió en la Shelley Incentivised Testnet ITN- si no tomaste acción alguna en tus fondos de mainnet desde el 29 de noviembre del 2019, puedes acceder a tus fondos de mainnet utilizando la sección anteriormente descrita para [reclamar tu billetera de la era Byron](#byron-era-wallet).
