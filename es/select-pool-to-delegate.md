
No hay un pool "bueno para todo el mundo" con el que puedes delegar, de lo contrario - todos estaría delegando al mismo pool y la descentralización no haría sentido :) . Mientras que muchos usuarios les atraen los pools con los cosots más bajos, este es usualmente el factor menos importante para distinguir los stake pools. A continuación detallamos unos cuantos factores que deben ser considerados al momento de elegir un pool.

> Recuerda, tú - un delegante - eres uno de los componentes clave del protocolo de manera indirecta y tus acciones pueden determinar la descentralización así como la adopción de la plataforma. Ya sea para tus beneficios o para el beneficio de la red - es se suma importancia que elijas de manera responsable el pool con el cual delegarás.

En esta sección discutiremos los diferentes aspectos que los usuarios deben de tomar en cuenta al momento de seleccionar el pool que ellos desean apoyar. Si no estás seguro sobre los parámetros utilizando solamente tu billetera, favor apóyate de las plataformas de la comunidad construidas para ayudarte con tu decisión. Estas plataformas son:
- [Pooltool](https://pooltool.io)
- [ADAPools](https://adapools.org)
- [ADAStat](https://adastat.net)
- [CardanoScan](http://cardanoscan.io)
- [PoolPeek](https://poolpeek.com/)

La mayoría de estos sitios te permitirán filtrar usando varios parámetros para ayudarte con tu decisión. Además, nota los siguientes puntos:

#### El Operador del Pool  
  Cuando hagas staking, lo primero y más importante que quieres saber será sobre el operador del pool y su presencia en la comunidad. Cuando las cosas tomen un giro para mal, deberás de poder ponerte en contacto con los dueños/operadores del pool. Lá mayoría de los pools tendrán sus enlaces a sus redes sociales ya sea en el sitio web asociado con el pool, o vía la información extendida de metadatos. No podemos juzgar a alguien que decida mantenerse anónimo, pero puedes estar seguro que los que han estado en la comunidad por un tiempo no pondrán en riesgo su reputación.  

#### Número de pools operadas por un solo operador
  Hay unos cuantos operadores que operan múltiples pools con un marketing atractivo de costos bajos y un pledge bastante bajo. Están en todo su derecho de hacerlo - permitido por el protocolo, y es algo controversial - y la estética del pool es cuestionable (ya que siempre está la opción de aumentar los costos del pool en vez de crear nuevos pools). Lo que este tipo de pools están haciendo (tal vez sin querer) es empezar un [ataque Sybil](https://es.wikipedia.org/wiki/Ataque_Sybil) en el protocolo. El protocolo está diseñado para tener incentivos contra este comportamiento, pero solamente funciona con *razonamiento básico del delegante* en tener cuidado de no darle tanto poder a este tipo de pools. Ejemplos perfectos de este comportamiento son los pools de 1PCT y OCE. Desde un punto de vista de la descentralización, quieres mantenerte *lejos de los operadores que tiene varios pools, como regla general*.

#### Canales actualizados
  Lo más probable, los operadores de pools habilitarán suscripciones a sus canales (ya sea en telegram o twitter o su sitio web). Es importante que te unas a estos canales para informarte sobre anuncios de cambio de pledge o costos del pool. De lo contrario, pueda que los parámetros del pool cambien sin que te des cuenta. Si no encuentras una forma de contactar al operador, deberías de pensar bien si quieres delegar a ese pool.  

#### Punto de Saturación
  Para evitar centralizar en un solo pool todo el stake delegado, luego de haber alcanzado un criterio de delegación en específico (calculado pot `Suministro Total en Circulación`/`nOpt`), donde nOpt actualmente es 500, un pool dejará de obtener un número mayor de recompensas por la cantidad de delegación que posee (actualmente la cantidad máxima es de ~ `64M`). Por lo tanto, la porción de recompensa del delegante individual comenzará a reducirse entre más stake sea delegado al pool.
  En teoría, las recompensas son óptimas en un ounto justo en el punto de saturación, delegar a un pool cerca del punto de saturación significa que está más cerca de estar sobresaturado (y necesitarás estar pendiente del nivel de saturación). En vez, delegando a un pool más pequeño en comparación significa que tu recompensas no serán impactadas por mucho, pero puede ayudar a expandir la red al no participar en pools sobresaturadas (o cerca de estar saturadas). Dependiendo de la cantidad de stake que vayas a delegar, idealmente deberías de delegar en un pool cuyo Live Stake se encuentre entre 5% a 70% del punto de saturación.

#### Costos

  Operar un stake pool básico no es necesariamente tan difícil, dado un operador de pool con buenas prácticas de seguridad, disponibilidad, mantenimiento y visibilidad requerida incurren en costos de tiempo y monetarios. El protocolo, por lo tanto, permite a los pools especificar sus costos a cobrar y lo permite basado en ciertos parámetros. Nota que este costo es *restado solamente de las recompensas* que la red calcula para el pool, antes de distribuir las recompensas a los delegantes. Como delegante, a continuación te damos unos cuantos parámetros que deberías saber al momento de revisar los costos del pool:

#### Pledge del Pool
  El pledge es el compromiso de los dueños de un pool para mantener cierto valor de ada en su pool en todo momento (poniendo sus propias criptomonedas como pledge). Un valor de pledge mayor trae consigo un valor mayor de recompensas. Sin embargo, nota que en los parámetros actuales del protocolo, la diferencia neta en las recompensas no se ve muy afectada por un pool con pledge de 100K vs un pool con pledge de 1M (eg: para fines de comparación, delegando 100K a un pool con 100K de pledge puede generarte 5159 ADA vs un pool con 1M de pledge puede generarte 5161 ADA, anualmente). Por otro lado, delegar con un pool con 10M de pledge puede generarte 5223 ADA, asumiendo el mismo escenario por un año. Puedes ver cómo afecta el pledge y los demás parámetros usando la calculadora de staking de IOHK que se encuentra [aquí](https://cardano.org/calculator).

#### Costos Fijos del Pool
  Este es la cantidad mínima de recompensas que obtendrá el pool antes de que las recompensas por bloques sean distribuidas a los delegantes del pool. El parámetro del actual protocolo dicta un mínimo de 340 ADA como el mínimo valor del costo fijo. Este valor es para evitar que los pools compitan por tener un costo de 0 lo cual no es sustentable para el protocolo a largo plazo. Nota que este es el costo fijo del total de recompensas entre todos los delegantes del pool.
  
#### Margen del Pool (%)
  Este es el porcentaje  que el pool obtendrá del total de las recompensas del pool. Comparado con el total de recompensas generadas por el pool (eg: 10000 ADA), el margen del delegante (eg: 2.5% del total de las recompensas del pool) no es afectado de manera significativa por un margen del pool de un 1% (i.e. 230.9 ADA) v/s 4% (224.9 ADA) realmente no afecta las recompensas del delegagante por un margen significativo, a menos que ese delegante forme parte de un gran porcentaje del stake delegado al pool. Las recompensas son afectadas en su mayoría por la lotería de la asignación de slots y por el rendimiento del pool y no tanto por la diferencia del margen. Se recomiendo *NO* apresurarse i elegir un pool con 0% de margen si no cumple con los putnos discutidos anteriormente.
  
#### Rendimiento  
  Este parámetro es una estimación del rendimiento del pool basada en cuánto el protocolo *cree* que un pool pudo haber generado vs cuánto realmente generó. Cada bloque es recompensado por el protocolo (hasta que llegan al punto de saturación), por lo tanto un delegante querá quedarse con un pool cuyo rendimiento sea mayor a 80-85%. Nota que no podemos decir con certeza el 100% de rendimiento porque los bloques hechos por los pools también dependerán de cuántos bloques fueron asignados al pool. La asignación de bloques es algo aleatoria, la cual es proporcional (como una ruleta reservando un número mayor de slot correspondientes) al monto de stake delegado.
  
  #### Ranking en la Billetera  
  El ranking de la billetera de Daedalus *NO* toman en cuenta ciertos factores (suerte asociada con la asignación de slots para los pools, aún si es proporcional al stake, el factor de descentralización tiene un fuerte impacto en la aleatoriedad), ni tampoco considera por el monto de stake que el usuario desea agregar. Si bien esto no debe seguirse a ciegas, es un buen punto de referencia a largo plazo para que los delegadores vean qué tan deseable es el pool según las especificaciones originales de las billeteras.  
  
Esperamos que lo anterior te ayude a elegir un pool de tu agrado. Si deseas agregar algo a esta lista, puedes hacerlo abriendo un issue o PR en el repositorio github usando el ícono en la parte superior derecha de esta página.
