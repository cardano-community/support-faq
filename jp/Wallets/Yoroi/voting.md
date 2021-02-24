
Yoroi (chrom拡張機能) 3.10.0 のリリースを使うと、投票センターを使うことができます。

エンドユーザーとして参加するためには、2つのフェーズがあることを覚えておいてください:
- スナップショットの残高を基礎に投票力を受け取るウォレットを登録する必要があります (日付は各々の投票ラウンドの前に共有されます)。
- 実際の投票はスナップショットが撮られた後に、モバイルアプリで行われます。

各々の投票ラウンドに対して (**fund-3**):
- 登録期間は `17-Feb-2021 to 03-Mar-2021`
- スナップショットは `05-Mar-2021 23:23:00 GMT`.
- 投票のための最小残高のADAは `2950 ADA`.
- ハードウェアウォレットはこのラウンドで参加できません。

#### 投票力登録

投票力登録のために、Chrome拡張機能版Yoroiを使った方法は以下です:

![Yoroi Voting tab](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/voting1.png ':size=50%')

CatalystモバイルアプリをVotingタブからインストールできます。 (links for [iOS](https://apps.apple.com/kg/app/catalyst-voting/id1517473397) and [Android](https://play.google.com/store/apps/details?id=io.iohk.vitvoting)).

![Android Catalyst install](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/mobilevoting1.png ':size=50%')

スマホで、Catalystアプリを開いてアプリの紹介画面を進めて、 "Complete Registration"を押し、画面を進めます。

![Mobile App - Complete Registration](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/mobilevoting2.png ':size=50%')
![Voting wizard](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/mobilevoting3.png ':size=18%')

Yoroiへ戻り、ピンコードを設置アップします。モバイルデバイスで後で使いますので、このPINは安全に保管してください。

![Set up PIN](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/voting2.png ':size=35%')

指示に従い、支払いパスワードを入力します。（2回入力することに注意してください。）残高0の表記にそのまま進めて構いません。これによりブロックチェーンへ登録（ブロックチェーンでのトランザクションのため、０．１７ADAほどのトランザクションフィーがかかります）がされそのウォレット内の残高がスナップショットの一部としてキャプチャされる資格を得ることとなります。

![Set up PIN](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/voting4.png ':size=35%')

Yoroi拡張機能でQRコードが表示されます。QRコードをあなたのCatalystアプリで以下のようにスキャンします。:
!> QRコードはスクショをとってバックアップしましょう。これはCatalystアプリがなくなった場合に、再度Catalystアプリに投票力を復元する唯一の方法です.

![QR Code - extension](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/voting5.png ':size=35%')  

![Scan QR Code - Catalyst](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/mobilevoting4.png ':size=30%')

QRコードのデコード前に、PINをCatalystアプリにいれます:

![Enter PIN](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/mobilevoting5.png ':size=30%')

するとホーム画面に戻ります。この段階では投票力0と表示されていても問題ありません。3月5日に、あなたがスナップショット時にもっていた残高の投票力が付与されます。

![Completion](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/mobilevoting6.png ':size=30%')

上のメッセージが表示されたら投票力登録が成功しています。次のステップは投票期間まで待ってください。

#### よくある質問 :id=FAQ

##### 投票登録を終えましたが、提案のリストはどこですか？

投票期間が始まったらCatalystアプリからみることができます。もしそれまでに勉強したい場合はアイデアスケールから勉強できます。 

##### Yoroiのガイドのようですが、Daedalusの場合はどうしますか？

Daedalus統合の手順は、IOGZendeskサポートチームによって管理されています。投票手順は [こちら](https://iohk.zendesk.com/hc/en-us/articles/900004485866-Project-Catalyst-Fund3-voting-instructions) FQAは [こちら](https://iohk.zendesk.com/hc/en-us/articles/900004448046-Catalyst-Fund3-FAQ)です。

##### Yoroiモバイルはつかえますか?

いいえ、YoroiはChrome/Firefox拡張機能のみです。

##### 投票への参加はステーキング報酬に影響しますか?

いいえ, ステーキングはこれに参加してもしなくても影響しません。

##### ハードウェアウォレットを使えますか?

活発に開発は行われてますが残念ながらこのラウンドではハードウェアウォレットを登録することはできません。以下の質問をチェックしてください。

##### 資金を ledger/trezor から Yoroi へ移動して登録して、戻すことはできますか？

最小限の取引手数料を使って、オンラインウォレットをステーキング登録し、スナップショットの数分or数時間前に (`05-Mar-2021 23:23:00) ハードウェアウォレットからホットウォレットへ移動できます。 スナップショットが作成されたことが確認できたらまたはードウェアウォレットへ戻すことができます。これによりステーキングが影響を受けないことが保証されます。

上記以外の質問がある場合は、 [FAQ](https://docs.google.com/document/d/1qYtV15WXeM_AQYvISzr0a0Qj2IzW3hDvhMBvZZ4w2jE) をチェックして、 [Catalyst chat](https://t.me/ProjectCatalystChat)に参加してください。
