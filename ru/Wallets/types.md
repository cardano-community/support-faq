
Теперь, когда вы ознакомились с тем, что такое кошелек, давайте рассмотрим типы кошельков, которые вы можете использовать. Пожалуйста, перейдите по ссылке ниже, чтобы изучить конкретный тип кошелька.

Подводя итог с точки зрения конечного пользователя, можно сказать, что существует в основном два типа интерфейсов кошелька:

### Программные (Горячие) кошельки

Программный кошелек-это интерфейс цифрового кошелька, в котором криптографические ключи (зашифрованные) будут храниться на устройстве, которое вы используете. В программных кошельках существует в основном два типа кошельков, как указано ниже.

<!-- tabs:start -->

#### ** Кошелек с полной нодой **

Пример: Daedalus

Кошелек с полной нодой запускает полный независимый блокчейн-узел и предоставляет возможность управлять вашим кошельком, опрашивая узел. Примером такого кошелька является Daedalus. Есть несколько преимуществ запуска такого узла:
 - Вся история блокчейна доступна локально для вашего узла, чтобы иметь возможность запрашивать в соответствии с вашими потребностями.
 - Ваш узел будет проверять все блоки по мере их создания и синхронизации с вашим устройством, тем самым снижая доверие, необходимое для работы с кошельком.
 - Запуск полного узла - также повышает доступность блокчейна в вашем географическом регионе, обеспечивая лучшую задержку для узлов, создающих блоки.
 - Если есть функция, поддерживаемая узлом, но еще не пользовательским интерфейсом кошелька - вы можете напрямую подключиться к узлу и получить доступ к этой функции.

Наряду с этими преимуществами, запуск узла автоматически означает несколько обязанностей, которые могут рассматриваться как неудобство с точки зрения конечного пользователя, особенно если вы используете только транзакции:
 - Синхронизация всего блокчейна на вашем устройстве требует времени при первоначальной настройке, которое может составлять часы в зависимости от пропускной способности сети и диска устройства.
 - Существуют обязательства по хранению, памяти и сети, необходимые для запуска кошелька, подключенного к полному узлу.
 - Кошельки с полным узлом не могут считаться идеальными для портативных/портативных устройств.
 
#### ** Легкие кошельки **

Пример: Yoroi, ADALite

Легкий кошелек использует интерфейс, который подключается к удаленному узлу для операций - таким образом, освобождая вас от ответственности за управление полным блокчейн-узлом. Они могут быть доступны в виде плагинов/расширений для браузера, веб - сайтов или мобильных приложений. Преимущества использования легкого кошелька:
- Вам не нужно ждать, пока весь блокчейн будет синхронизирован на вашем устройстве, чтобы начать выполнять операции, так как вы подключаетесь к уже запущенному современному узлу через свой кошелек.
- Вы по-прежнему контролируете свои ключи. Распространенное заблуждение, связанное с легкими кошельками, заключается в том, что это небезопасно, потому что ваши ключи передаются по сети. Большинство профессиональных легких кошельков гарантируют, что ваши ключи никогда не покидают ваше устройство и всегда находятся в зашифрованном состоянии даже на вашем устройстве. На данный момент это не должно быть отличием для вас, чтобы выбрать между кошельком с полным узлом и легким кошельком, они так же безопасны, как и ваше устройство._
- Вам не нужно беспокоиться о выполнении обновлений узлов блокчейна, так как это можно сделать на стороне сервера.
- Легкие кошельки могут быть легко интегрированы в портативные/ручные устройства.
- Они, как правило, очень легкие и не имеют высоких требований к хранению/памяти или стабильной сети.

Для получения официальной информации о сравнении, пожалуйста, посетите [this support article](https://iohk.zendesk.com/hc/en-us/articles/360026058573-Daedalus-wallet-compared-to-Yoroi-wallet) от IOHK.

<!-- tabs:end -->

### Бумажные (холодные) кошельки

Бумажные кошельки-это, по сути, кошельки, созданные программными интерфейсами, но сделанные таким образом, чтобы ключи для этих бумажных кошельков никогда не были в Сети. Они обычно предоставляют слова в двух частях - часть, напечатанная на бумаге, и другая часть со словами (в случае Daedalus) или паролем (в случае Yoroi), который гарантирует, что даже если у кого-то есть доступ к бумаге, он не сможет получить доступ к вашим ключам. Моменты, которые нужно запомнить:
- Программное обеспечение, создающее бумажный кошелек, не будет переводить средства на сгенерированный кошелек, это должно быть ручное действие.
- Если по какой-либо причине вы решите восстановить свой бумажный кошелек, ваш кошелек будет восстановлен на цифровом устройстве, которое находится в сети и больше не будет "холодным" кошельком. Таким образом, в этом случае было бы лучше создать новый бумажный кошелек с точки зрения безопасности.

### Аппаратные (холодные) кошельки

Посетите [этот](https://emurgo.io/en/blog/hardware-wallet-explanation-yoroi-keep-ada-safe) блог от Emurgo для краткого обзора того, как аппаратные кошельки работают с Yoroi
