
!> Las siguientes instrucciones asumen que ya ha [instalado Yoroi](es/Wallets/Yoroi/install.md)

Puede restaurar una billetera de Yoroi o una billetera de papel en Yoroi usando su frase de restauración. Note que los siguientes pasos *SOLAMENTE* aplican para las billeteras de Shelley. Las billeteras de Legacy (Byron/ITN) pueden ser reclamadas siguiendo las instrucciones en [esta página](es/Wallets/Yoroi/transfer.md).

Revise las siguientes pantallas para el proceso:

> Si ya ha creado/restaurado una billetera de Shelley y desea recuperar otra billetera de Shelley, siga [estas](es/Wallets/Yoroi/create.md#adding-or-switching-between-wallets) instrucciones para hacer click en `Add New Wallet` (Adicionar Billetera) y llegar a la siguiente página:

Seleccione `Restore wallet` (Restaurar billetera) en la página principal como se muestra a continuación:

![Home Page](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/img-es/yoroi-home.jpg ':size=50%')

Seleccione `Cardano` como currency (moneda):

![Currency](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/img-es/yoroi-select-currency.jpg ':size=30%')

Se le pedirá que seleccione el tipo de billetera que desea recuperar:

![Restore 1](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/img-es/yoroi-restore-wallet-1.jpg ':size=30%')

Seleccione la opción apropiada en base a la billetera que restaurará, y utilice el siguiente menú para ver las instrucciones respectivas:

<!-- tabs:start -->

#### **Frase de Restauración de 15 palabras**

Las billeteras de Yoroi y ADALite proporcionan frases de restauración de 15 palabras de manera predeterminada cuando crea una nueva billetera `Caliente`. Use esta opción si desea restaurar este tipo de billetera en Shelley. 
Actualmente, existen dos tipos de frases de restauración que puede restaurar. Para simplicidad, apéguese a restaurar solamente `Shelley-era wallet` (Billetera de la era Shelley), como es mencionado al inicio de este documento. La opción `Byron wallet` (Billetera Bryon) solamente está presente para fines de historial de transacción (ej: impuestos), en caso de que los necesite.

![Restore 15-word Shelley Wallet](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/img-es/yoroi-restore-wallet-15-type.jpg ':size=30%')

Dele un nombre a su billetera para ayudarle a identificarla, introduzca la frase de restauración de 15 palabras y seleccione una nueva contraseña que usará para esta billetera.

![Restore 15-word Shelley Wallet - details](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/img-es/yoroi-restore-wallet-15-mnemonics.jpg ':size=30%')

#### **Frase de Restauración de 24 palabras**

La Mainnet de Daedalus le provee de manera predeterminada con una frase de restauración de 24 palabras cuando crea billeteras de Shelley. Use esta opción si intenta restaurar este tipo de billeteras.

Dele un nombre a su billetera para ayudar a identificarla, introduzca la frase de restauración de 24 palabras y seleccione una nueva contraseña que usará para esta billetera.

![Restore 24-word Shelley Wallet - details](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/img-es/yoroi-restore-wallet-15-mnemonics.jpg ':size=30%')

#### **Billetera de Papel (Paper Wallet)**

Yoroi le permite crear billeteras de papel compatibles con Shelley. Use esta opción si intenta restaurar este tipo de billeteras en Shelley.

Dele un nombre a su billetera para ayudar a identificarla, introduzca la frase de restauración de 21 palabras **de su billetera de papel** y la **contraseña de la billetera de papel** que le pidieron que recordara (note que ambas son necesarias, aceptó las advertencias cuando creó la billetera de papel - diciendo que es responsable de tener *ambas* al momento de restaurar) y seleccione una nueva contraseña que usarás para esta billetera.

![Restore 24-word Shelley Wallet - details](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/img-es/yoroi-restore-paper-wallet.jpg ':size=30%')

<!-- tabs:end -->

Al final verá su account checksum (suma de comprobación de la cuenta) (como un número de la placa de un carro para identificación) y las direcciones de su billetera de cada era/tipo para verificación, haga click en `Confirm` (Confirmar):

![Verify wallet](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/img-es/yoroi-restore-verify.jpg ':size=40%')

¡Felicidades! ¡Ha restaurado su billetera de Shelley de manera correcta!