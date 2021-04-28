#### ¿Qué es una Billetera? {docsify-ignore}

Una billetera es un programa de software que crea, almacena y maneja el acceso a las llaves públicas y privadas que controlan los fondos en la blockchain. Puede usar diferentes billeteras, pero mientras siga empleando la misma llave privada, podrá acceder a los mismos fondos en la cadena. Las billeteras en el ecosistema de Cardano son `Determinista Jerárquica ('HD' por sus siglas en inglés)` basadas en el modelo `UTXO`, por buenas razones. Antes de platicar sobre estos términos, repasemos los conceptos básicos sobre las llaves.

#### Conceptos Básicos sobre Llaves Privadas {docsify-ignore}

Una llave privada es una cadena de caracteres generados de manera aleatoria y estos pueden generar una llave pública, la cual pasa por el proceso de hashing para crear una dirección. La introducción de las criptomonedas comenzó, teniendo los usuarios el completo control sin necesidad de terceros (ser su propio banco). Esto automáticamente significa que el usuario es responsable por sus propios fondos, y es responsabilidad del individuo mantener las llaves privadas seguras. Si pierde sus llaves privadas, básicamente pierde acceso a sus fondos digitales en la blockchain, y **nadie** (ni siquiera los desarrolladores) pueden brindarle acceso a esos fondos.

La mejor forma de asegurar sus llaves privadas depende del uso de su dispositivo. No hay una regla de oro que aplique para todos. En estos tiempos, tener sus llaves en línea las hace susceptibles a ser comprometidas - ya sea por la seguridad de su dispositivo en línea, o por el acceso a su servidor. Por lo tanto, una práctica común es mantener sus llaves privadas fuera del alcance de una conexión a internet. No querrá tenerla en algún formato no encriptado o que sea hackeado fácilmente en su dispositivo en línea.

#### Billeteras Deterministas Jerárquicas (HD) {docsify-ignore}

Estas permiten a los usuarios derivar sus llaves (públicas y privadas) de una clave en común (construida usando mnemotécnicos BIP39) lo que facilita el respaldo y permite mejores características de la billetera y privacidad del historial. Esto significa que recibirá una combinación de palabras (12, 15, 24, 25 o 27 - dependiendo del tipo de billetera software que elija) y el hash de estas palabras resultará ser tu llave privada única, volviéndo el acceso más fácil y mejorando la seguridad. Una de las características de una billetera HD es que puede contener hasta 2147483647 cuentas diferentes con 2147483647 direcciones, todas asociadas a una sola billetera - y cada una con su historial de transacciones único.

Puede visitar [esta wiki](https://github.com/input-output-hk/cardano-wallet/wiki/About-Address-Derivation) para obtener información detallada sobre las billeteras HD y cómo funciona la derivación de direcciones entre:

- Billeteras HD Aleatorias (Billeteras Daedalus de Legacy Byron - donde las direcciones comienzan con `Ddz..`
- Billeteras Secuenciales HD Estilo Icarus de Legacy Byron - donde las direcciones comienzan con `Ae2..`
- Billeteras Shelley (siempre basadas en HD Secuenciales, pero usando bech32 - dirección típica comenzando con `addr...`).

Como puede ver, hay gran variedad para las distintas combinaciones usadas en los mnemotécnicos de las diferentes billeteras. Solo para darle un resumen de cuántas claves son soportadas por x número de billeteras:

|Billetera         |Era      |Tipo             |Número de Palabras             |
|------------------|---------|-----------------|-------------------------------|
|Daedalus          |Byron    |Caliente/En línea|12                             |
|Daedalus          |Byron    |Papel            |27 (18 en papel + 9 digital)   |
|Daedalus Rewards  |ITN      |Caliente/En línea|15                             |
|Yoroi             |Byron/ITN|Caliente/En línea|15                             |
|Yoroi             |Byron/ITN|Papel            |21 en papel + contraseña       |
|Daedalus          |Shelley  |Caliente/En línea|24                             |
|Yoroi             |Shelley  |Caliente/En línea|15 / 24                        |

#### Fondos en una billetera versus dirección {docsify-ignore}

Una de las confusiones más comunes que los usuarios encuentran es comprender el saldo de una billetera HD y el conflicto entre los fondos en una dirección versus los fondos en una billetera. Esto se debe a la forma en la cual los UTXO (Unspent Transaction Output "Salida de Transacción no Gastada") de las billeteras HD operan. Cada nueva transacción dentro de la billetera selecciona de manera automática un set de direcciones que forman un saldo mínimo para efectuar la transferencia y luego agrega una *nueva* dirección de salida (referida como UTXO antes mencionada) - la cual es una "dirección de cambio".
El concepto se comprende mejor utilizando una analogía con billetes de moneda como en el sistema financiero actual.

Digamos que Alice tiene 3 billetes de 10 dólares en su cartera, y ella quiere comprar 50 manzanas que Bob vende a un costo de 18 dólares.
Alice le paga a Bob usando dos billetes de 10 dólares, y recibe 2 dólares de cambio (los cuales ella no tenía antes) como una nueva salida de transacción no gastada.
Por lo tanto, Alice, ahora tiene un billete de 10 dólares y un cambio de 2 dólares - añadidos a su cartera. Si ahora Alice revisa su cartera buscando billetes anteriores encontrará un billete de 10 dólares - pero el total de fondos en su cartera incluirán también los 2 dólares de cambio.

De manera similar, cuando efectúa una transacción desde su billetera - las entradas seleccionadas normalmente excederán las salidas y un cambio deberá de ser creado.
Cuando consultes sus fondos, si está viendo el valor de una dirección - puede que no vea todos sus detalles, porque la billetera contiene varias direcciones y los usuarios puede que no sepan cuántos fondos contiene cada dirección luego de efectuar transacciones.
Por lo tanto, la mejor manera de consultar sus fondos es utilizando su billetera software, la cual tuvo acceso a sus llaves. El uso de un explorador blockchain es bastante conveniente para revisar si sus fondos fueron recibidos en la dirección X.

Para más detalles, puede leer el excelente [blog de Emurgo](https://forum.cardano.org/t/manual-blockchain-el-modelo-utxo-de-cardano-explicacion-sencilla/28269) el cual provee más información sobre el modelo UTXO.
