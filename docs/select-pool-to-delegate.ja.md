
すべての人が委託すべき１つのプールというものはありませんー皆が同じプールへ委託するのでない限り。しかしそれは分散化されていません :) 多くのユーザーは手数料マージンが最も低いプールに惹かれますが、それは通常、ステークプールを区別するために最も重要ではない要素です。以下に、考慮に入れるべき重要な要素をいくつか挙げます。

> あなた(委任者)は間接的にプロトコルのコアコンポーネントの一つであり、あなたの行動がプラットフォームの採用や分散化を決定する可能性があることを覚えておいてください。それが自分の利益のためであれ、ネットワークの利益のためであれ、誰に委任するかを慎重に選択することが重要です。

!> 広告宣伝をしていないかもしれず、十分な委任も受けていないかもしれないエコシステムへの重大な貢献者達がいます。もしあなたがサポートしたい場合は、 [こちら](community-contrib.md) から貢献者達の詳細を知ることができます。

このセクションでは、委任するときに考慮することについて説明します。単にウォレットの情報だけではパラメータがわからないときは、コミュニティが用意した次のようなプラットフォームを利用してください。
- [Pooltool](https://pooltool.io)
- [ADAPools](https://adapools.org)
- [ADAStat](https://adastat.net)
- [CardanoScan](http://cardanoscan.io)
- [PoolPeek](https://poolpeek.com/)

これらのサイトのほとんどは、あなたが意思決定を助けるために様々なパラメータを使用してフィルタリングすることができます。さらに、以下のポイントに注意してください。

#### プールオペレータ

  ステーキングをするとき、まず知りたいと思うのは、プールオペレーターとそのコミュニティーでの存在です。 プールの所有者/運営者と連絡を取ることができるはずです。 そこにあるほとんどのプールには、プールに関連付けられたWebサイトまたは拡張メタデータ情報のいずれかを介してソーシャルリンクを利用できます。 身元を開示したくない人は判断できませんが、しばらくの間活動している人が評判を落とすようなことはしないと確信できます。 

#### オペレータにより運営されているプール数

  低料金と非常に低い誓約の魅力あるマーケティングで複数プールを運営するオペレーターいます。 彼らはプロトコルで許可されているように、完全にそうする権利の範囲内にありますが、ここには議論の余地があります。これはプールの美学として疑問があります(新しいプールを追加する代わりに、個々のプールの料金を増やすオプションがあるので)。 そのようなプールが（おそらく意図せずに）行っていることは、 [多重人格攻撃](https://en.wikipedia.org/wiki/Sybil_attack#:~:text=In%20a%20Sybil%20attack%2C%20the,diagnosed%20with%20dissociative%20identity%20disorder) の始まりです。プロトコルはこのような振る舞いに対してインセンティブを持つように設計されていますが、それはデリゲータがそのようなプールを強力にしすぎないように注意しているという基本的な理論的根拠に基づいてのみ機能します。そのような振る舞いの完璧な例は1PCTとOCEプールです。分散化の観点からは、一般的には複数のプールを実行しているものには近づかない方が良いでしょう。

#### アップデートチャンネル

  たいていの場合、プールオペレーターはアップデートを入手できる場を提供します（テレグラムグループ、Twitterフィード、Webサイトなど）。 誓約額や手数料の変更などのためにこれらのチャネルに参加することが重要です。 そうしないと、プールパラメータの変更に気づかないかもしれません。 オペレーターに連絡する方法が見つからない場合は、オペレータの選択を再考するほうがよいでしょう。

#### 飽和点

  すべてのステークの委任を単一のプールに集中させないために、ある委任基準（供給量/nOptで計算）に達した後（現在nOptが500である場合）、あるプールはより多くの委任に対してより高い報酬を得られなくなります（現在、これは～64Mに相当します）。したがって、そのようなプールに委任されるステークが増えると、個々の委任者の報酬の部分はさらに減少し始めるでしょう。
理論的には、プールに対する報酬は飽和点で最適ですが、飽和点に近いプールに委任することは、常に過剰に飽和していることを意味する可能性があります（そして、委任を常に監視し続けなければならないでしょう）。その代わり、比較的小さなプールに対して委任することで、あなたの報酬が必ずしも大きな影響を受けることはありませんが、飽和しすぎている（またはすぐに飽和してしまう可能性のある）プールに対して参加しないことで、ネットワークをさらに助けることができます。委任するステークの量にもよりますが、理想的には、ライブステークが飽和ポイントの5%から70%の間のどこかにあるプールとのステークにすることをお勧めします。

#### 手数料

　基本的なstakepoolを立てるのは本当に難しいことではありませんが、セキュリティ、可用性、保守性、および可視性を備えたプールオペレーターの管理には、時間と経費がかかります。 したがって、このプロトコルにより、プールはいくつかのパラメータに基づいて料金を指定できます。 この料金は、委任者にさらに報酬を分配する前に、ネットワークがプールに対して計算した報酬からのみ取られることに注意してください。委任者として、以下はプール料金を見るときに知っておくべきポイントです。

#### プール誓約（資本）
   基本的に、誓約は、プールの所有者がプールの所有者キー（つまり、自分の「ゲーム内のスキン」）を維持することを約束するものです。 誓約が多いほど、報酬が多くなります。 ただし、現在のプロトコルパラメータでは、報酬の全体的な違いは、100Kを誓約するプールと1Mを誓約するプールの影響をあまり受けないことに注意してください（たとえば、基本的な仮定として、100Kを100Kの誓約されたプールに委任すると、5159 v / s 1Mの誓約が得られる可能性があります。 プールは毎年5161 ADAを獲得する可能性があります。ただし、同じ仮定で1000万の誓約済みプールを委任すると、1年間にわたって同じシナリオで5223 ADAを獲得できる可能性があります。IOHKステーキング計算機を使用して、誓約パラメーターとその影響を試すことができます [here](https://cardano.org/calculator)

#### プール固定費
  これは、特定のプールによって作成されたブロックに対する報酬がプロトコルによって委任者に配布される前に、プールが獲得する最低の報酬です。 現在のプロトコルパラメータでは、固定最小コストとして最低340 ADAが規定されています。 この料金は、将来プロトコルにとって持続可能ではない0の料金プールへの競争を防ぐために行われています。 これは、プールに委任するすべての委任者に対する報酬全体からの固定コストであることに注意してください。
  
#### プール変動費 (%)
  これは、プールが総報酬ポットから稼ぐことができる報酬の割合です。プールが生み出す報酬ポット（例：10000 ADA）と比較すると、委任者のマージン（例：プールからの総報酬の2.5％）は、プールのマージンが1％（すなわち230.9 ADA）対4％（224.9 ADA）であることによって、その委任者がそのプールのためのかなりの量のステークを形成しない限り、大きく影響を受けることはありません。報酬は、スロット割り当ての抽選とプールのパフォーマンスによって、マージンの差よりもはるかに大きな影響を受けます。上記で説明した残りのポイントを満たさない場合は、0%プールに向かって走らないことを強くお勧めします。
  
#### パフォーマンス
  これは、プールが実際に行った仕事量に対しての、行ったと考えるステークプロトコルの仕事量に基づくプールのパフォーマンスの見積もりです。 すべてのブロックはプロトコルによって（飽和点まで）報われるため、委任者は80〜85％を超えるパフォーマンスを持つプールを使い続ける必要があります。 ここで決定的に100％とは言えないことに注意してください。プールによって作成される実際のブロックは、プールに実際に割り当てられたブロックの数にも依存するためです。 ここでは、割り当てられるブロック数は少しランダムな部分があります。これは、（ルーレットが対応するより多くのスロットを確保しているように）ステークに比例します。
  
#### ウォレットのランキング
  Daedalus のウォレットランキングは、いくつかの要因（プールへのスロット割り当てに関連した運、ステークに比例していてもランダム化に影響を与える分散化の要因）を考慮しておらず、またユーザーが追加したいステークの量も考慮していません。これは盲目的に従うべきではありませんが、ウォレットの本来の仕様通りにプールがどの程度望ましいかを確認するための長期的な参照ポイントになるでしょう。

上記があなたがあなたの選択のプールを選ぶのを助けることを願っています。 このリストへの追加を確認したい場合は、ページの右上隅にあるアイコンを使用して、このリポジトリに対して問題/ PRを提起してください。