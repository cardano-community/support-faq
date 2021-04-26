
Ahora que ya conoce más sobre lo que es una billetera, veamos los tipos de billeteras que puede usar. Revise las siguientes secciones para ver algún tipo específico de billetera.

Para resumir, hay dos tipos principales de interfaces de billeteras:

### Billeteras Software (Calientes)

Una billetera software es una interfaz de billetera digital donde las llaves criptográficas (encriptadas) serán almacenadas en el dispositivo que esté usando. Existen dos tipos de billeteras software:

<!-- tabs:start -->

#### **Billetera de Nodo Completo**

Ejemplo: Daedalus

Estas billeteras ejecutan por completo un nodo de la blockchain de manera independiente y proporciona la capacidad de operar su billetera consultando el nodo. Un ejemplo de tal billetera es Daedalus. Existen ciertas ventajas en ejecutar un nodo de este tipo:

- Todo el historial de la blockchain está disponible en su nodo de manera local, para que pueda consultarlo cuando lo necesite.
- Su nodo validará todos los bloques a medida que son creados y sincronizados con su dispositivo - reduciendo la confianza requerida de operar en una billetera.
- Ejecutar un nodo en su totalidad también aumenta la disponibilidad de la blockchain en su región geográfica, brindando mejor latencia para los nodos encargados de producir bloques.
- Si hay una configuración que es compatible con un nodo, pero no con una billetera con interfaz de usuario, usted puede conectarse directamente al nodo y acceder a la configuración.

Sumado a esas ventajas, ejecutar un nodo de manera automática significa más responsabilidades - las cuales pueden no ser placenteras para los usuarios - especialmente si su único uso es realizar transacciones:

- Sincronizar por completo la blockchain en su dispositivo requiere de tiempo la primera vez que el nodo es ejecutado, lo cual puede demorar horas dependiendo de la red y el disco del dispositivo.
- Se requiere de cierto espacio en el disco, memoria RAM y de la red para ejecutar una billetera conectada a un nodo completo.
- Las billeteras de nodo completo no son la mejor opción para un dispositivo móvil/portátil.

#### **Billeteras Ligeras**

Ejemplo: Yoroi, ADALite

Una billetera ligera utiliza una interfaz que se conecta a un nodo distante para operaciones - por lo tanto, no requiere de las responsabilidades de operar un nodo completo de la blockchain. Están disponibles como plugins/extensiones de exploradores, sitios web o aplicaciones móviles. Las ventajas de usarlas son:

- No necesita esperar a que toda la blockchain esté sincronizada a su dispositivo para poder realizar operaciones, ya que se conectas a un nodo ya actualizado vía su billetera.
- Permanece en control de sus llaves. Una mal interpretación común sobre las billeteras ligeras es que son inseguras porque sus llaves son enviadas por la red. La mayoría de las billeteras ligeras profesionales se asegurarán que sus llaves nunca dejen su dispositivo y que siempre estén encriptadas en él. Hasta ahora, esto no debería ser un factor determinante para usted al momento de seleccionar entre una billetera de nodo completo v/s una billetera ligera, *ambas son igual de seguras que su dispositivo*.
- No necesita preocuparse por actualizar el nodo de la blockchain, ya que esto es hecho del lado del servidor.
- Las billeteras ligeras pueden ser integradas fácilmente en dispositivos portátiles/móviles.
- Normalmente son bastante livianas y no requieren de un gran volumen de almacenamiento/memoria o una red estable.

Para enlaces oficiales sobre la comparación. visite [este artículo de soporte](https://forum.cardano.org/t/daedalus-versus-yoroi/27451?u=napoles) de IOG.

<!-- tabs:end -->

### Billeteras de Papel (Frías)

Las billeteras de papel son billeteras creadas por una interfaz de software, pero hechas de tal forma que las llaves de esas billeteras de papel nunca estuvieron en línea. Usualmente proporcionan su clave en dos partes - una parte impresa en papel, y la otra parte con palabras (en el caso de Daedalus) o contraseña (en el caso de Yoroi) lo que garantiza incluso que alguien que tiene acceso al papel, no pueda acceder a sus llaves. Puntos a recordar:

- El software encargado de crear la billetera de papel no transferirá los fondos a una billetera generada, esta debe de ser una operación manual.
- Si por cualquier razón decide restaurar su billetera de papel, esta será restaurada en un dispositivo digital cual está en línea y dejará de ser una billetera "fría". Por lo tanto, en ese caso es mejor crear una nueva billetera de papel si lo vemos de un punto de vista de seguridad.

### Billeteras Hardware (Frías)

Visite [este](https://forum.cardano.org/t/una-explicacion-sencilla-de-las-billeteras-de-hardware-como-funcionan-con-yoroi-y-por-que-son-importantes-para-mantener-segura-mi-ada/26131?u=napoles) blog de Emurgo para un breve resumen de cómo funcionan las Billeteras Hardware Wallets con Yoroi.
