
Ahora que ya conoces más sobre lo que es una billetera, veamos los tipos de billeteras que puedes usar. Navega las siguientes secciones para ver algún tipo específico de billetera.

Para resumir, hay dos tipos principales de interfaces de billeteras:

### Billeteras Software (Calientes)

Una billetera software es una interfaz de billetera digital donde las llaves criptográficas (encriptadas) serás almacenadas en el dispositivo que estés usando. Existen dos tipos de billeteras software:

<!-- tabs:start -->

#### ** Billetera de Nodo Completo **

Ejemplo: Daedalus

Una billetera de nodo completo ejecuta por completo un nodo de la blockchain de manera independiente y proporciona la capacidad de operar tu billetera consultando el nodo. Un ejemplo de tal billetera es Daedalus. Existen ciertas ventajas de ejecutar el nodo de manera completa:
 - Todo el historial de la blockchain está disponible en tu nodo de manera local, para que pueda consultarlo cuando lo necesites.
 - Tu nodo validará todos los bloques en lo que son creados y sincronizados con tu dispositivo, por lo tanto - reduciendo la confianza requerida de operar en una billetera.
 - Ejecutar un nodo en su totalidad también aumenta la disponibilidad de la blockchain en tu región geográfica, brindando mejor latencia para los nodos encargados de producir bloques.
 - Si hay una configuración que es compatible con un nodo, pero no con una billetera con interfaz de usuario, puedes conectarte directamente al nodo y acceder a la configuración.

Sumado a esas ventajas, ejecutar un nodo de manera automática significa más responsabilidades - las cuales pueden no ser placenteras para los usuarios - especialmente si tu uso principal es realizar transacciones:
 - Sincronizar por completo la blockchain en tu dispositivo requiere de tiempo la primera vez que es el nodo es ejecutado, lo cual puede demorar horas dependiendo de la red y el disco del dispositivo.
 - Se requiere de cierto espacio en el disco, memoria RAM y de la red para ejecutar una billetera conectada a un nodo completo.
 - Las billeteras de nodo completo no son la mejor opción para un dispositivo móvil/portátil.
 
#### ** Billeteras Ligeras **

Ejemplo: Yoroi, ADALite

Una billetera ligera utiliza una interfaz que se conecta a un nodo distante para operaciones - por lo tanto, no requiere de las responsabilidades de operar un nodo completo de la blockchain. Están disponibles como plugins/extensiones de exploradores, sitios web o aplicaciones móviles. Las ventajas de usar una billetera ligera son:
- No necesitas esperar a que toda la blockchain esté sincronizada a tu dispositivo para poder realizar operaciones, ya que te conectas a un nodo ya actualizado vía tu billetera.
- Permaneces en control de tus llaves. Una mal interpretación común sobre las billeteras ligeras es que son inseguras porque tus llaves son enviadas por la red. La mayoría de las billeteras ligeras profesionales se asegurará que tus llaves nunca dejen tu dispositivo, y que siempre estén encriptadas en tu dispositivo. Hasta ahora, esto no debería de ser un factor determinante para ti al momento de seleccionar entre una billetera de nodo completo v/s una billetera ligera, *ambas son igual de seguras que tu dispositivo*.
- No necesitas preocuparte por actualizar el nodo de la blockchain, ya que esto es hecho del lado del servidor.
- Las billeteras ligeras pueden ser integradas fácilmente en dispositivos portátiles/móviles.
- Normalmente son bastante livianas, y no requieren de un gran volumen de almacenamiento/memoria o una red estable.

Para enlaces oficiales sobre la comparación. visita [este artículo de soporte](https://iohk.zendesk.com/hc/en-us/articles/360026058573-Daedalus-wallet-compared-to-Yoroi-wallet) de IOG.

<!-- tabs:end -->

### Billeteras de Papel (Frías)

Las billeteras de papel son billeteras creadas por una interfaz de software, pero hechas de tal forma que las llaves de esas billeteras de papel nunca estuvieron en línea. Usualmente proporcionan su clave en dos partes - una parte impresa en papel, y la otra parte con palabras (en el caso de Daedalus) o contraseña (en el caso de Yoroi) que garantiza incluso alguien que tiene acceso al papel, no puede acceder a tus llaves. Puntos a recordar:
- El software encargado de crear la billetera de papel  no transferirá los fondos a una billetera generada, debe de ser una operación manual.
- Si por cualquier razón decides restaurar tu billetera de papel, tu billetera será restaurada en un dispositivo digital en cual está en línea y dejará de ser una billetera "fría". Por lo tanto, en ese caso es mejor crear una nueva billetera de papel si lo vemos de un punto de vista de seguridad.

### Billeteras Hardware (Frías)

Visita [este](https://emurgo.io/en/blog/hardware-wallet-explanation-yoroi-keep-ada-safe) blog de Emurgo para un breve resumen de cómo funcionan las Billeteras Hardware Wallets con Yoroi.
