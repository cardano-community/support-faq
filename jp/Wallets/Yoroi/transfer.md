バイロンまたはITNウォレットからYoroiのシェリーウォレットに資金を請求または転送できます。

!> 以下は [Yoroiインストール済](Wallets/Yoroi/install.md) *かつ*  [shelleyウォレットを作成済](Wallets/Yoroi/create.md) または [shelleyウォレットを復元済](Wallets/Yoroi/restore.md) なことを前提にしています。.

ウォレットとその時代とリカバリーフレーズの対応表は [こちら](wallets.md#heirarchical-deterministic-hd-wallets)

サイドバーの復元送金をクリックして対応する時代をクリックします:

![Claim / Transfer page](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-1.jpg ':size=40%')

#### バイロンウォレット

<!-- tabs:start -->

##### ** レガシーダイダロスウォレット **

これはダイダロス（ホットウォレット+ペーパーウォレット+マスターキーへのアクセス権を持つユーザー）バイロンユーザー向けです。以下のように、復元しようとしているウォレットのタイプを選択します。

![Claim / Transfer Byron Daedalus Wallets](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-2.jpg ':size=25%')

##### ** Icarus / Yoroiウォレット **

これは、Yoroi / ADALite拡張機能+モバイルByronユーザー向けです。復元しようとしているウォレットのタイプを選択します。

![Claim / Transfer Byron Icarus/Yoroi Wallets](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-3.jpg ':size=25%')

<!-- tabs:end -->

#### Shelley-era Wallet (Shelley Incentivised Testnet報酬)

このオプションは、15ワードのリカバリーフレーズまたはマスターキーを使用して、Yoroiウォレット（現時点では）から報酬を引き出します。これにより、参加していて回収できる報酬がある場合は、ITN報酬を回収することもできます。レジャー/トレザーおよび24ワードのシードベースのウォレットユーザーの場合、Dashboardの同じウォレット内のタブから報酬を引き出すことができます。

リカバリを続行するには、最初に開いているウォレットの上部が「Shelley-standard wallet」と以下のようになっていることを確認してください：

![Claim Shelley Rewards](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-shelley-reward.jpg ':size=30%')

10 ADAをこの開いているウォレットに持っていることをお勧めします（実際に必要な料金はおそらく1 ADA未満になるでしょう）。Shelley-Era Walletをクリックして、適切な選択肢を選択します。

![Select type of reward to withdraw](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-claim-shelley-reward-type.jpg ':size=25%')

##### Chrome拡張機能から暗号化された秘密鍵にアクセスする

リカバリーフレーズにアクセスできない場合は、Yoroiウォレットの秘密鍵を取得することもできます。秘密鍵にアクセスするには、ブラウザでYoroi拡張機能を開き、「Developer Tools」にアクセスします。Chromeの場合、以下のように進められます。

![Yoroi Chrome Dev Tools](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/chrome-dev-tools.jpg ':size=30%')

新しいペインが開くのが見えるはずです。[アプリケーション]タブに移動し、[Storage]> [IndexedDB]> [yoroi-schema]> [Key]と移動します。ウォレットのIDが表示されますので、展開すると、暗号化されたハッシュが表示されるのでそれをコピーします。（次に、上記シェリーの報酬を要求するために貼り付けるように求められたら貼り付けます）。

![Yoroi get encrypted private key](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/yoroi-get-priv-key.jpg ':size=30%')

キーは以前に使用した送金パスワードを使用して暗号化され、ハッシュを使用する場合も送金パスワードを入力する必要があることに注意してください。

!> ！> Shelley testnet（ITN）ウォレットには、メインネットファンドではなく、報酬のみが含まれていました。メインネットの資金はShelley Incentivized Testnetで起こったこととは無関係であり、2019年11月29日以降にメインネットの資金に対して何の措置も取らなかった場合でも、上記の [バイロン時代のウォレットを復元](#byron-era-wallet) のセクションを利用してメインネットの資金にアクセスできます。
