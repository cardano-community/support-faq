Acontinuación encontrarás una lista de preguntas frecuentes hechas a lo largo de los diversos canales de redes sociales en la comunidad de Cardano. Y si ves que algo no ha sido respondido, por favor crea un issue/PR usando el ícono en la esquina superior derecha :smile:

#### Delegué a un pool en epoch `n`, ¿cuándo recibiré mis recompensas? :id=reward-schedule
Para c ualquier cambio en la delegación, las recompensas son reflejadas luegos de **3** transiciones de epochs (por lo tanto, luego de `15-20 days`). Revisa los siguientes detalles para ver cómo funciona:
- Un Epoch en Cardano dura 5 días. Cualquier cambio en la Delegación es capturado en el `snapshot` al final del epoch (esta será la primera transición de epoch).
- El snapshot capturado es considerado *live* (live stake) en la siguiente transición de epoch (segunda transición) Esto quiere decir que el pool al cual has delegado reflejará tu delegación en `n+2` epochs, para calificar a una oportunidad proporcional a su stake (participación) de producir bloques (la cual ahora incluirá tu delegación).
- Los bloques producidos por el pool califican para recompensas, las cuales son calculadas en la siguiente transición de epoch (por lo tanto, el cálculo de recompensas ocurre en el el epoch `n+3`).
- Finalmente, las recompensas son pagadas al final del siguiente epoch `n+3`.
Por lo tanto, si tu delegas en el epoch `n`, tus recompensas serán depositadas a inicios del epoch `n+4` (técnicamente, sería a finales del epoch `n+3`).
Puedes ver la representación visual de lo explicado anteriormente acontinuación (usando `n=213` en el ejemplo):

  ![Rewards Schedule](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/rewards-schedule.jpg)

#### ¿Nos perdemos de recompensas cuando cambiamos la delegación a otro pool? :id=change-delegation
**No.**
Si cambias tu delegación a otro pool dos veces en el epoch, solamente el último cambio será tomado en cuenta para el snapshot del epoch.
Si cambias tu delegación del pool `P1` a `P2`, siempre recibirás las recompensas del pool `P1` hasta que el [período de recompensas](#reward-schedule) para `P2` comience.

#### ¿Cómo monitoreo mis recompensas? Yoroi o Daedalus no muestras las recompensas de cada epoch :id=monitor-rewards
Actualmente, las billeteras no son capaces de mostrar el historial de recompensas debido a un API faltante que pronto será incorporado. Por mientras, hay varias formas de monitorear tus recompensas, puedes usar cualquier dirección de tu billetera (no importa cuál, selecciona una dirección aleatoria de tu pestaña `Wallet > Receive`) y rastrea el historial de recompensas usando cualquiera de las siguientes opciones:
- via tu explorador de internet preferido [pooltool] o [cardanoscan]
- recibe notificaciones via [Pegasus Mobile App](https://pegasuspool.info/) en tu móvil
- recibe notificacion de telegram via [ADAstat](https://t.me/AdaStatBot)

#### No recibí mis recompensas luego de esperar el tiempo sugerido según el calendario de recompensas. ¿Qué hago? :id=missing-rewards
Idealmente, primero deberás de contactar a tu operador de pool. La mayoría de los operadores de pools proveen alguna forma para que tú puedas contactarlos. Pero algunas cosas que querás confirmar por tu cuenta son:
- Si estás esperando recibir recompenas en el epoch x, revisa los bloques producidos por el pool en epoch x-2 (refiérete al calendario [anterior](#reward-schedule) para más detalles). Puedes utilzar cualquiera de los [exploradores de pools](es/explorers.md#list) y revisar el historial del pool para los bloques producidos en ese epoch.
- Si la pool produjo bloques, pero no has recibido tus recompensas, verifica los parámetros del ool - si el costo fijo (el mínimo predeterminado es 340 ADA) para el pool es mayor que las recompensas recibidas, los pueda que los delegadores no reciban recompensas.
- Si el operado no recibió recompensa alguna, eso puede indicar un problema con la configuración de su pool, y lo mejor sería notificarles lo más pronto posible.

#### ¿Necesito reclamar las recompensas y volver a delegar mis ADAs? :id=withdraw-rewards
Las recompensas que recibas automáticamente serán delegadas al pool que actualmente delegas con esa billetera en específica. Esto también se cumple cuando recibas fondos en esa misma billetera. Actualmente tu billetera es la que está delegando a un pool, cualquier cambio ocurrido en el epoch `n` automáticamente será capturado por el snapshot y recibirá las recompensas debidas en el epoch `n+4`. **La única circumstancia en la cual necesitarás retirar tus recompensas será cuando muevas todos tus fondos a una billetera distinta o a un intercambio.** 

[pooltool]: https://pooltool.io
[cardanoscan]: https://cardanoscan.io
[adapools]: https://adapools.org
