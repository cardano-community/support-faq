
!> 以下の手順は、[Yoroiをインストール済み](Wallets/Yoroi/install.md)であることを前提としています。

回復フレーズを使用して、YoroiでYoroiウォレットまたはペーパーウォレットを復元できます。以下の手順は、シェリーウォレットに*のみ*適用されることに注意してください。レガシー（バイロン/ ITN）ウォレットは、[このページ](Wallets/Yoroi/transfer.md)の手順で請求できます

以下の画面でプロセスを確認してください。

>  Shelleyウォレットをすでに作成/復元していて、別のShelleyウォレットを復元したい場合は、 [ここ](Wallets/Yoroi/create.md#adding-or-switching-between-wallets) の指示に従って、 新しいウォレットを追加して、以下のページにアクセスしてください

以下に示すように、ホーム画面でウォレットの復元を選択します。

![Home Page](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-home.jpg ':size=50%')

選択します： `Cardano`:

![Currency](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-select-currency.jpg ':size=30%')

復元するウォレットのタイプを選択するように求められます。

![Restore 1](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-restore-wallet-1.jpg ':size=30%')

復元するウォレットに基づいて適切なオプションを選択し、対応するスクリーンショットについては以下のタブを使用してください。

<!-- tabs:start -->

#### ** 15単語のリカバリーフレーズ **

YoroiとADALiteのウォレットは、新しい「ホット」ウォレットを作成するときに、15ワードのリカバリフレーズをデフォルトとして提供します。このようなシェリーウォレットを復元する場合は、このオプションを使用します。
現在、復元できるリカバリフレーズには2つのタイプがあります。使い方を簡単にするために、「Shelley時代のウォレット」のみを復元するようにしてください。このドキュメントの冒頭で述べたように。 「バイロンウォレット」オプションは、トランザクション履歴（例：税金計算処理に使用するなど）の目的でのみ必要です。

![Restore 15-word Shelley Wallet](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-restore-wallet-15-type.jpg ':size=30%')

ウォレットを識別するウォレット名を入力し、15ワードのリカバリフレーズを入力し、このウォレットに使用する新しい送金パスワードを選択します。

![Restore 15-word Shelley Wallet - details](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-restore-wallet-15-mnemonics.jpg ':size=30%')

#### ** 24単語のリカバリーフレーズ **

Daedalus Mainnetはデフォルトで、シェリーウォレットを作成するときに24ワードの回復フレーズを提供します。このようなウォレットを復元する場合は、このオプションを使用してください。

ウォレットを識別するウォレット名を入力し、24ワードの回復フレーズを入力し、このウォレットに使用する新しい送金パスワードを選択します。

![Restore 24-word Shelley Wallet - details](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-restore-wallet-15-mnemonics.jpg ':size=30%')

#### ** ペーパーウォレット **

Yoroiでは、シェリーと互換性のある紙の財布を作成できます。このようなシェリーウォレットを復元する場合は、このオプションを使用します。

ウォレットを識別するウォレット名を入力し、覚えておくように求められた***ペーパーウォレットからの***21ワードの回復フレーズと***ペーパーウォレットのパスワード***を入力します（両方とも必須です。あなたはペーパーウォレットを作成するときに警告を受け入れました-復元するときに「両方」を所有する責任があることを示されています。）、この財布に使用する新しい送金パスワードを選択します。

![Restore 24-word Shelley Wallet - details](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-restore-paper-wallet.jpg ':size=30%')

<!-- tabs:end -->

アカウントのチェックサム（識別のための車のナンバープレートのような）と確認のための各時代/タイプのウォレットのアドレスが表示されます。次へクリックしm進みます。

![Verify wallet](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-restore-verify.jpg ':size=40%')

おめでとう！ Shelleyウォレットの復元に成功しました!!
