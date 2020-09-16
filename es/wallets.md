#### ¿Qué es una Billetera? {docsify-ignore}

Una billetera es un programa de software que crea, almacena y maneja el accesso a las llaves públicas y privadas que controlan los fondos en la blockchain. Puedes usar diferentes billeteras, pero mientras sigas usando la misma llave privada, podr'as accesar a los mismos fondos en la cadena. Las billeteras en el ecosistema de Cardano son `Determinista Jerárquicas ('HD' por sus siglas en inglés)` y basadas en el modelo `UTXO` - y por buenas razones. Antes de platicar sobre estos términos, repasemos los conceptos básicos sobre las llaves.

#### Conceptos Básicos sobre Llaves Privadas {docsify-ignore}

Una llave privada es una cadena de carateres generados de manera aleatoria y estos pueden generar una llave pública, la cual pasa por el proceso de hashing para crear una dirección. La introducción de las cirptomonedas comenzó con usuarios en completo control sin necesidad de terceros (ser tu propio banco). Esto automáticamente significa que el usuario es responsable pro sus propios fondos, y es la responsabilidad del individuo mantener las llaves privadas seguras. Si pierdes tus llaves privadas, básicamente pierdes acceso a tus fondos digitales en la blockchain, y **nadie** (ni siquiera los desarrolladores) pueden brindarte acceso a esos fondos.

La mejor forma de asegurar tus llaves privadas depende del uso de tu dispositivo. No hay una regla de oro que aplique para todos. En estos tiempos, tener tus llaves en línea las hace susceptibles a ser comprometidas - ya sea por la seguridad de tu dispositivo en línea, o por el acceso a tu servidor. Por lo tanto, una práctica común es mantener tus llaves privadas fuera del alcance de una conexión a internet. No querás tener alguna formato no encriptado o que sea hackeado fácilmente en tu dispositvo en línea.

#### Billeteras Deteminista Jerárquicas (HD) {docsify-ignore}

Las billeteras deterministas jerárquicas (HD) permiten a los usuarios derivar sus llaves (públicas y privadas) de una clave en común (construida usando mnemotécnicos BIP39) lo que facilita el respaldo y permite mejores características de la billetera y privacidad del historial. Esto significa eu recibirás una combinación de palabras (12, 15, 24, 25 o 27 - dependiendo del tipo de billetera software que elijas) y el hash de estas palabras resultará ser tu llave privada única, volviéndolo más fácil acceder y mejorando la seguridad. Una de las características de una billetera HD es que una sola billetera puede contener hasta 2147483647 cuentas diferentes con 2147483647 direcciones, todas asociadas a una sola billetera - y cada una con su historial de transacciones único.

Puedes visitar [esta wiki](https://github.com/input-output-hk/cardano-wallet/wiki/About-Address-Derivation) para información detallada sobre las billeteras HD y cómo funciona la derivación de direcciones entre:
- Billeteras HD Aleatorias (Billeteras Daedalus de Legacy Byron - donde las direcciones comienzan con `Ddz..`
- Billeteras Secuenciales HD Estilo Icarus de Legacy Byron - donde las direcciones comienzan con `Ae2..`
- Billeteras Shelley (siempre basadas en HD Secuenciales, pero usando bech32 - dirección típica comenzando con `addr...`).

Como puedes ver, hay una hay gran variedad para las distintas combinaciones usadas para los mnemotécnicos de las diferentes billeteras. Solo para darte un resumen de cuántas claves son soportadas por x número de billeteras:

|Billetera         |Era      |Tipe             |Número de Palabras             |
|------------------|---------|-----------------|-------------------------------|
|Daedalus          |Byron    |Caliente/En línea|12                             |
|Daedalus          |Byron    |Papel            |27 (18 en papel + 9 digital)   |
|Daedalus Rewards  |ITN      |Caliente/En línea|15                             |
|Yoroi             |Byron/ITN|Caliente/En línea|15                             |
|Yoroi             |Byron/ITN|Papel            |21 en papel + contraseña       |
|Daedalus          |Shelley  |Caliente/En línea|24                             |
|Yoroi             |Shelley  |Caliente/En línea|24                             |

#### Fondos en una billeteras versus dirección {docsify-ignore}

Una de las confusiones más comunes que los usuarios encuentran es comprender el saldo de una billetera HD, y el conflicto entre los fondos en una dirección versus los fondos en una billetera. Esto se debe a la forma en la cual los UTXO (Unspent Transaction Output "Salida de Transacción no Gastada") de las billeteras HD operan. Cada nueva transacción dentre de la billetera selecciona de manera automática un set de direcciones las cuales forman un saldo mínimo para efectuar la transferencia, y luego agrega una *nueva* dirección de salida (referida como UTXO antes mencionada) - la cual es un "dirección de cambio".
El concepto se comprende mejor utilizando una analogía con notas de moneda - asi como es usado en el sistema financiero actual.

Digamos que Alice tiene 3 notas de 10 dólares en su cartera, y ella quiere comprar 50 manzanas que Bob vende a un costo de 18 dólares.
Alice le paga a Bob usando ambas notas de 10 dólares, y recibe 2 dólares de cambio (los cuales ella no tenía antes) como una nueva salida de transacción no gastada.
Por lo tanto, Alice, ahora tiene una nota de 10 dólares y un cambio de 2 dólares  - añadidos a su cartera. Revisar su cartera por notas anteriores resultará en una nota de 10 dólares - pero el total de fondos en su cartera incluirán los 2 dólares de cambio.

De manera similar, cuando efectúas una transacción desde tu billetera - las entradas seleccionadas normalmente excederán las salidas y un cambio deberá de ser creado.
Cuando consultes tus fondos, si estás viendo el valor de una dirección - pueda que no veas todos sus detalles, porque la billetera contiene varias direcciones, y los usuarios pueda que no sepan cu''antos fondos contiene cada dirección luege de efectuar transacciones.
Por lo tanto, la mejor manera de consultar tus fondos es utilizando tu billetera software, la cual tuvo acceso a tus llaves. Revisar si tus fondos fueron recibidos en la dirección X, el explorador es bastante conveniente.

Para más detalles, puedes leer el gran [blog de Emurgo](https://emurgo.io/en/blog/blockchain-primer-cardanos-utxo-model-simply-explained) el cual entre en más detalles sobre el modelo UTXO.
