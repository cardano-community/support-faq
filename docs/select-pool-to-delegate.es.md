
No hay un pool "bueno para todo el mundo" con el que puedes delegar, de lo contrario - todos estarían delegando al mismo pool y la descentralización no tendría sentido :) . Mientras que a muchos usuarios les atraen los pools con los costos más bajos, este es usualmente el factor menos importante para distinguir los stake pools. A continuación detallamos unos cuantos factores que deben ser considerados en el momento de elegir un pool.

> Recuerde, usted - un delegante - es uno de los componentes clave del protocolo de manera indirecta y sus acciones pueden determinar la descentralización, así como la adopción de la plataforma. Ya sea para su beneficio o el de la red - es de suma importancia que elija de manera responsable el pool con el cual delegará.

En esta sección discutiremos los diferentes aspectos que los usuarios deben de tomar en cuenta al momento de seleccionar el pool que ellos desean apoyar. Si no está seguro sobre los parámetros utilizando solamente su billetera, favor apóyese de las plataformas de la comunidad construidas para ayudarle con su decisión. Estas plataformas son:

- [Pooltool](https://pooltool.io)
- [ADAPools](https://adapools.org)
- [ADAStat](https://adastat.net)
- [CardanoScan](http://cardanoscan.io)
- [PoolPeek](https://poolpeek.com/)

La mayoría de estos sitios le permitirán filtrar usando varios parámetros para ayudarle con su decisión. Además, tenga en cuenta los siguientes puntos:

#### El Operador del Pool

  Cuando haga staking, lo primero y más importante que querrá saber será sobre el operador del pool y su presencia en la comunidad. Cuando las cosas tomen un giro para mal, deberá poder contactar con los dueños/operadores del pool. La mayoría de los pools tendrán sus enlaces a sus redes sociales ya sea en el sitio web asociado con el pool, o a través de la información extendida de metadatos. No podemos juzgar a alguien que decida mantenerse anónimo, pero puede estar seguro de que los que han estado en la comunidad por un tiempo no pondrán en riesgo su reputación.  

#### Número de pools operadas por un solo operador

  Hay unos cuantos operadores que gestionan múltiples pools con un marketing atractivo de costos y un pledge bastante bajo. Están en todo su derecho de hacerlo - permitido por el protocolo y es algo controversial - la estética del pool es cuestionable (ya que siempre está la opción de aumentar los costos en vez de crear nuevos pools). Lo que este tipo de pools está haciendo (tal vez sin querer) es empezar un [ataque Sybil](https://es.wikipedia.org/wiki/Ataque_Sybil) en el protocolo el cual está diseñado para tener incentivos contra este comportamiento, pero solamente funciona con *razonamiento básico del delegante* en tener cuidado de no darle tanto poder a este tipo de pools. Ejemplos perfectos de este comportamiento son los pools de 1PCT y OCE. Desde el punto de vista de la descentralización, debe mantenerse *lejos de los operadores que tienen varios pools, como regla general*.

#### Canales actualizados

  Lo más probable es que, los operadores de pools habilitarán suscripciones a sus canales (ya sea en Telegram o Twitter o su sitio web). Es importante que se una a estos canales para informarse sobre anuncios de cambio de pledge o costos del pool. De lo contrario, puede que los parámetros del pool cambien sin que se dé cuenta. Si no encuentra una forma de contactar al operador, debería pensar bien si quiere delegar a ese pool.  

#### Punto de Saturación

  Para evitar centralizar en un solo pool todo el stake delegado, luego de haber alcanzado un criterio de delegación en específico (calculado pot `Suministro Total en Circulación`/`nOpt`), donde nOpt actualmente es 500, un pool dejará de obtener un número mayor de recompensas por la cantidad de delegación que posee (actualmente la cantidad máxima es de ~ `64M`). Por lo tanto, la porción de recompensa del delegante individual comenzará a reducirse entre más stake sea delegado al pool.
  En teoría, las recompensas de un pool son óptimas justo en el punto de saturación, delegar en un pool próximo a la saturación, significa que podría saturarse (por lo que necesitará estar pendiente de este nivel). En cambio, si delega a un pool más pequeño significa que sus recompensas no serán muy afectadas, puede ayudar a expandir la red no participando en pools sobresaturados (o cerca de estar saturados). Dependiendo de la cantidad de stake que vaya a delegar, idealmente debería delegar en un pool cuyo Live Stake se encuentre entre 5% a 70% del punto de saturación.

#### Costos

  Operar un stake pool básico no es necesariamente tan difícil, pero un pool con buena seguridad, disponibilidad, mantenimiento y visibilidad requerida conlleva gastos de tiempo y monetario. El protocolo, por lo tanto, permite a los pools especificar sus costos a cobrar basado en ciertos parámetros. Note que este costo es *restado solamente de las recompensas* que la red calcula para el pool, antes de distribuir las recompensas a los delegantes. Como delegante, a continuación le damos unos cuantos parámetros que debería saber al momento de revisar los costos del pool:

#### Pledge del Pool

  El pledge es el compromiso de los dueños de un pool para mantener cierto valor de ada en su pool en todo momento (poniendo sus propias criptomonedas como pledge). Un valor de pledge mayor trae consigo un valor mayor de recompensas. Sin embargo, note que, en los parámetros actuales del protocolo, la diferencia neta en las recompensas no se ve muy afectada por un pool con pledge de 100K vs un pool con pledge de 1M (ej.: para fines de comparación, delegando 100K a un pool con 100K de pledge puede generarle 5159 ADA vs un pool con 1M de pledge puede generarle 5161 ADA, anualmente). Por otro lado, delegar con un pool con 10M de pledge puede generarle 5223 ADA, asumiendo el mismo escenario por un año. Puede ver cómo afecta el pledge y los demás parámetros usando la [calculadora de staking de IOHK](https://cardano.org/calculator).

#### Costos Fijos del Pool

  Estos es la cantidad mínima de recompensas que obtendrá el pool antes de que las recompensas por bloques sean distribuidas a los delegantes del pool. El parámetro del actual protocolo dicta un mínimo de 340 ADA como el mínimo valor del costo fijo. Este valor es para evitar que los pools compitan por tener un costo de 0 lo cual no es sustentable para el protocolo a largo plazo. Note que este es el costo fijo del total de recompensas entre todos los delegantes del pool.
  
#### Margen del Pool (%)

  Es el porcentaje que el pool obtendrá del total de las recompensas del pool. Comparado con el total de recompensas generadas por el pool (eg: 10000 ADA), el margen del delegante (ej.: 2.5% del total de las recompensas del pool) no es afectado de manera significativa por un margen del pool de un 1% (i.e. 230.9 ADA) v/s 4% (224.9 ADA) realmente no afecta las recompensas del delegante por un margen significativo, a menos que ese delegante forme parte de un gran porcentaje del stake delegado al pool. Las recompensas son afectadas en su mayoría por la lotería de la asignación de slots y por el rendimiento del pool y no tanto por la diferencia del margen. Se recomienda *NO* apresurarse y elegir un pool con 0% de margen si no cumple con los puntos expuestos anteriormente.
  
#### Rendimiento

  Este parámetro es una estimación del rendimiento del pool basada en cuánto el protocolo *cree* que un pool pudo haber generado vs cuánto realmente generó. Cada bloque es recompensado por el protocolo (hasta que llegan al punto de saturación), por lo tanto un delegante querrá quedarse con un pool cuyo rendimiento sea mayor a 80-85%. Note que no podemos decir con certeza el 100% de rendimiento porque los bloques hechos por los pools también dependerán de cuántos bloques fueron asignados al pool. La asignación de bloques es algo aleatoria, la cual es proporcional (como una ruleta reservando un número mayor de slot correspondientes) al monto de stake delegado.
  
#### Ranking en la Billetera

  El ranking de la billetera de Daedalus *NO* toma en cuenta ciertos factores (suerte asociada con la asignación de slots para los pools, aun si es proporcional al stake, el factor de descentralización tiene un fuerte impacto en la aleatoriedad), ni tampoco considera el monto de stake que el usuario desea agregar. Si bien esto no debe seguirse a ciegas, es un buen punto de referencia a largo plazo para que los delegantes vean qué tan deseable es el pool según las especificaciones originales de las billeteras.  
  
Esperamos que lo anterior le ayude a elegir un pool de su agrado. Si desea agregar algo a esta lista, puede hacerlo abriendo un issue o PR en el repositorio GitHub usando el ícono en la parte superior derecha de esta página.
