A continuación, encontrará una lista de preguntas frecuentes hechas a lo largo de los diversos canales de redes sociales en la comunidad de Cardano. Y si ve que algo no ha sido respondido, por favor crea un issue/PR usando el ícono en la esquina superior derecha :smile:

#### Delegué a un pool en epoch `n`, ¿cuándo recibiré mis recompensas? :id=reward-schedule

Para cualquier cambio en la delegación, las recompensas son reflejadas luego de **3** transiciones de epochs (por lo tanto, luego de `15-20 days`). Revise los siguientes detalles para ver cómo funciona:

- Un Epoch en Cardano dura 5 días. Cualquier cambio en la Delegación es capturado en el `snapshot` al final del epoch (esta será la primera transición de epoch).
- El snapshot capturado es considerado *live* (live stake) en la siguiente transición de epoch (segunda transición). Esto quiere decir que el pool al cual has delegado reflejará su delegación en `n+2` epochs, para calificar a una oportunidad proporcional a su stake (participación) de producir bloques (la cual ahora incluirá su delegación).
- Los bloques producidos por el pool califican para recompensas, las cuales son calculadas en la siguiente transición de epoch (por lo tanto, el cálculo de recompensas ocurre en epoch `n+3`).
- Finalmente, las recompensas son pagadas al final del siguiente epoch `n+3`.
Por lo tanto, si usted delega en el epoch `n`, sus recompensas serán depositadas a inicios del epoch `n+4` (técnicamente, sería a finales del epoch `n+3`).
Puede ver la representación visual de lo explicado anteriormente a continuación (usando `n=213` en el ejemplo):

  ![Rewards Schedule](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/rewards-schedule.jpg)

#### ¿Nos perdemos de recompensas cuando cambiamos la delegación a otro pool? :id=change-delegation

**No.** Si cambia su delegación a otro pool dos veces en el epoch, solamente el último cambio será tomado en cuenta para el snapshot del epoch. Si cambia su delegación del pool `P1` a `P2`, siempre recibirá las recompensas del pool `P1` hasta que el [período de recompensas](#reward-schedule) para `P2` comience.

#### ¿Cómo monitoreo mis recompensas? Yoroi o Daedalus no muestran las recompensas de cada epoch :id=monitor-rewards

Actualmente, las billeteras no son capaces de mostrar el historial de recompensas debido a un API faltante que pronto será incorporado. Mientras, hay varias formas de monitorear sus recompensas, puede usar cualquier dirección de su billetera (no importa cuál, seleccione una dirección aleatoria de la pestaña `Wallet > Receive`) y rastree el historial de recompensas usando cualquiera de las siguientes opciones:

- vía su explorador de internet preferido [pooltool] o [cardanoscan]
- reciba notificaciones vía [Pegasus Mobile App](https://pegasuspool.info/) en su móvil
- reciba notificación de Telegram vía [ADAstat](https://t.me/AdaStatBot)

#### No recibí mis recompensas luego de esperar el tiempo sugerido según el calendario de recompensas. ¿Qué hago? :id=missing-rewards

Idealmente, primero deberá contactar a su operador de pool. La mayoría de los operadores de pools proveen alguna forma para que pueda contactarlos. Pero antes querrá confirmar ciertos detalles:

- Si está esperando recibir recompensas en el epoch x, revise los bloques producidos por el pool en epoch x-2 (refiérase al calendario [anterior](#reward-schedule) para más detalles). Puede utilizar cualquiera de los [exploradores de pools](es/explorers.md#list) y revisar el historial del pool para los bloques producidos en ese epoch.
- Si el pool produjo bloques, pero no ha recibido tus recompensas, verifique los parámetros del pool - si el costo fijo (el mínimo predeterminado es 340 ADA) para el pool es mayor que las recompensas recibidas, puede que los delegantes no reciban recompensas.
- Si el operador no recibió recompensa alguna, eso puede indicar un problema con la configuración de su pool y lo mejor sería notificarles lo más pronto posible.

#### ¿Necesito reclamar las recompensas y volver a delegar mis ADAs? :id=withdraw-rewards

Las recompensas que reciba automáticamente serán delegadas al pool que actualmente delega con esa billetera en específico. Esto también se cumple cuando reciba fondos en esa misma billetera. Actualmente su billetera es la que está delegando a un pool, cualquier cambio ocurrido en el epoch `n` automáticamente será capturado por el snapshot y recibirá las recompensas debidas en el epoch `n+4`. **La única circunstancia en la cual necesitará retirar sus recompensas será cuando mueva todos sus fondos a una billetera distinta o a un intercambio.**

[pooltool]: https://pooltool.io
[cardanoscan]: https://cardanoscan.io
[adapools]: https://adapools.org
