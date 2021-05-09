Puede reclamar/tranferir fondos desde una billetera de Byron/ITN a una billetera de Shelley en Yoroi.

!> Las siguientes instrucciones asumen que ya ha [instalado Yoroi](es/Wallets/Yoroi/install.md) *Y* ya ha [creado una billetera de Shelley](es/Wallets/Yoroi/create.md) **O** [restaurado una billetera de Shelley](es/Wallets/Yoroi/restore.md).

Note que la billetera versus la era versus mnemotécnico, las métricas pueden ser encontradas [aquí](es/wallets.md#heirarchical-deterministic-hd-wallets)

Haga click en el ícono `Claim / Transfer` (Reclamar/Transferir) en la barra lateral, y seleccione la era de la billetera que intenta reclamar:

![Claim / Transfer page](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/img-es/yoroi-claim-1.jpg ':size=40%')

Asegúrese que tenga:

#### Billetera de la Era Byron

<!-- tabs:start -->

##### **Billetera Daedalus Legacy**

Esta sección es para los usuarios de Byron Daedalus (Billetera caliente + billetera de papel + acceso a la llave maestra (master key). Seleccione el tipo de billetera que intenta restaurar como se indica a continuación:

![Claim / Transfer Byron Daedalus Wallets](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/img-es/yoroi-claim-2.jpg ':size=25%')

##### **Billetera Icarus/Yoroi**

Esta sección es para los usuarios de la extensión de Yoroi/ADALite + usuarios móviles de Byron. Seleccione el tipo de billetera que intenta restaurar:

![Claim / Transfer Byron Icarus/Yoroi Wallets](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/img-es/yoroi-claim-3.jpg ':size=25%')

*Usuarios de Byron Ledger: Nota que a partir de la versión 3.2.2 de la extensión de Yoroi, la integración Ledger todavía no es compatible, e introducir las llaves de restauración de Ledger ***no es recomendado***. Puede conectar su Ledger a <https://adalite.io> (completamente compatible con las billeteras de Yoroi), si no desea esperar a que esté presente esta característica.*

<!-- tabs:end -->

#### Billetera de la Era Shelley (Recompensas de Shelley Incentivised Testnet ITN)

Esta opción es para reclamar las recompensas de las billeteras de Yoroi (por los momentos) usando su frase de restauración de 15 palabras o la llave maestra. Esto igual le permite reclamar las recompensas de la ITN si participó y tiene recompensas por reclamar. Para ledger/trezor y billeteras con claves de 24 palabras, puede reclamar sus recompensas desde la pestaña `Dashboard` (Tablero de Control) dentro de la respectiva billetera.

Para continuar con la frase de restauración, primeramente asegúrese de que la parte superior de su billetera activa diga `Shelley-standard wallet` (Billetera Estándar de Shelley) como se muestra a continuación:

![Claim Shelley Rewards](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/img-es/yoroi-claim-shelley-reward.jpg ':size=30%')

Es recomendado que tenga `10 ADA` en la billetera a la cual enviará las recompensas (aún cuando el costo actual requerido probablemente sea menor a 1 ADA). Haz click en `Shelley-Era Wallet` (Billetera de la era Shelley) y luego seleccione la opción adecuada:


##### Obteniendo acceso desde la extensión chromium a su llave privada encriptada

Si no tiene acceso a sus mnemotécnicos, puede obtener la llave privada de su billetera Yoroi. Para ello, abra la extensión de Yoroi en su explorador y diríjase a `Developer Tools` (Herramientas del desarrollador). Para Chrome, puede navegar como se muestra a continuación:

![Yoroi Chrome Dev Tools](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/img-es/chrome-dev-tools.jpg ':size=30%')

Debería de ver un nuevo pánel. Ve a la pestaña `Application` (Aplicación) y navegue a `Storage > IndexedDB > yoroi-schema > Key` (Almacenamiento > BD Indexada > Esquema de Yoroi > Llave ). Verá las IDs de sus billeteras. Si expande las opciones, debería de ver su hash encriptado, el cual puede copiar (y luego pegar cuando se le pida al reclamar las recompensas de Shelley como mencionamos anteriormente):

![Yoroi get encrypted private key](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/img-es/yoroi-get-priv-key.jpg ':size=30%')

Note que las llaves pueden ser encriptadas usando la contraseña que utilizó anteriormente, y utilizar el hash también le pedirá introducir su contraseña.

!> Sus billeteras de Shelley testnet (ITN) **solamente** contienen sus recompensas, no los fondos de la mainnet. Sus fondos de la mainnet se mantendrán, independientemente de lo que sucedió en la Shelley Incentivized Testnet ITN- si no realizó ninguna acción con sus fondos de mainnet desde el 29 de noviembre del 2019, puede acceder a ellos utilizando la sección anteriormente descrita para [reclamar su billetera de la era Byron](#byron-era-wallet).
