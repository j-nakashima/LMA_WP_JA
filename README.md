# Learning Measurement for Analytics Whitepaper <small>（分析のための学習測定に関するホワイトペーパー）</small>


> この文書は、[IMS Global Learning Consortium](http://www.imsglobal.org/) による [「Learning Measurement for Analytics Whitepaper」](http://www.imsglobal.org/IMSLearningAnalyticsWP.pdf) の有志による日本語訳です。
>
> 本書は、IMS が策定を進めるオンライン学習測定フレームワーク Caliper の概要を紹介したものです。
>
> - 本書の現著作権は IMS Global Learning Consortium に帰属します。  
>    ©2013 IMS Global Learning Consortium, Inc. All Rights Reserved
> - この翻訳は参考であり、公式のものではありません。
> - 翻訳に関する誤りの報告や改善の提案には、Github の Issue または Pull Request をご利用ください。
> 
> <dl>
> <dt>翻訳</dt>
> <dd>日本電子出版協会（JEPA）／高瀬拓史（イースト株式会社）</dd>
> <dt>公開日</dt>
> <dd>2014-06-30</dd>
> <dt>最終更新日</dt>
> <dd>2014-06-30</dd>
> </dl>


## 機会

オンライン教育の状況は、オンラインデジタルカリキュラムの開発・配信・加入において大幅な成長を続けている。また、豊富なオンライン学習活動を測定・分析できるアカウンタビリティ[^1]は、これまでも大きな関心を集めてきたものであり、今必要とされているものでもある。この関心は、高度にスケール化されたオンラインカリキュラムを配信する MOOCS をはじめとするオンラインプログラムが近年急増していることと相まって、より効率的で詳細なオンライン学習環境のために、教育に「ビッグデータ」解析を取り入れようとする動きを教育テクノロジー[^2]のエコシステムの中に引き起こしている。測定可能なアカウンタビリティに対するこのような関心と需要は、IMSと標準がリーダーシップをとって、学習活動とそのパフォーマンスを極めて細かいレベルで測定可能にする共通基盤を定義するための絶好の機会である。

[^1]: 説明責任。予算配分に関わる。

[^2]: edtech

学習測定用の標準ベースの共通基盤を搭載することで、エコシステム全体のオンラインカリキュラムの品質や有効性やパフォーマンスの解析は、より効率的に達成できる。このオンラインカリキュラムの生産者（すなわち機関、講師、カリキュラム開発者、学習デザイナー等）と消費者（すなわち学習者／生徒）の両者は、より良いかたちで参加、測定、復習を繰り返し、カリキュラムと学習体験の成果を継続的に改善できる。加えて、機関や教育テクノロジーのプロバイダーは、高い需要と価値を持つ、新しい強力なデータ駆動型拡張機能（学習分析、予測分析／パス管理、適応学習、パーソナライゼーション、早期警告、バッジや認定の授与などが挙げられる）を、オンライン学習配信プラットフォームに届けることができる。

このタイムリーで価値ある機会を踏まえて、標準ベースの学習測定フレームワークを実現する上で、その戦略と方針に優先的に取り入れた課題には、主に次のものがある：

- 現在のオンラインカリキュラム配信は非標準的であり、幅広いソリューションやプロバイダーが提供する教育アプリケーションは、そのカリキュラム学習活動の内容と機能を評価する基準がまったく存在していない状況にある。こうした多様なソリューションは、それぞれのプロバイダーの配信プラットフォーム／アプリケーションの中で、高度に連合し、断片化され、‘サイロ化’[3]されている。これらのソリューションの集合は、オンラインの授業やカリキュラムの中でしばしば共存する。中には([Bloom’s Taxonomy], [Common Core], [Predictive Analytics Reporting (PAR) framework][PAR], [Council for the Advancement of Standards in Higher Education -Learning and Developmental Outcomes][CAS standards] といった)標準的な基準に関連した学習の設計／パフォーマンス目標を達成するべく改善を進める動きもあるが、より普遍的で幅広い測定のコンテキストの中で使えるものでなければならない。

[3]: siloed

[Bloom’s Taxonomy]: http://en.wikipedia.org/wiki/Bloom's_Taxonomy

[Common Core]: http://www.corestandards.org/the-standards

[PAR]: https://public.datacookbook.com/public/institutions/par

[CAS standards]: http://www.cas.edu/index.php/cas-general-standards/

- こうした状況を考慮すると、カリキュラムの中やカリキュラム間で測定された学習活動に対して、配信コンテキストを踏まえることなく、統一的かつ一貫した見解を確立するのは難しい;
- 標準化された一貫性のある計測フレームワークと評価基準がなければ、学習活動を効果的に比較したり互いに関連付けたりすることも、カリキュラムの効果を判断することも、学習者同士の相互作用やパフォーマンスへの潜在的影響を評価することも難しい;
- かなり以前から存在する取り組み（すなわち Learning Tools Interoperability™(LTI)™, Learning Information Services (LIS), Question and Test Interoperability™(QTI)™）は、学習活動のカプセル化と活用可能なコンテキストを標準化するために行われた。しかしこれらは、学習測定を行うために拡張する必要がある。
- ビッグデータテクノロジーやデータサイエンスの取り組みといった新しく広範な分野から生まれた規約や標準の多くは、互いに重複したり不足したりしている。これらの技術や取り組みには、NoSQL、クラウドスケールの関係データベース、グラフデータベース、Map-Reduce、ADL Experience/TinCan APIなどがあるが、早期の段階にあったり、オンライン教育に最適化した測定や分析の標準化に利用できるのか不明であったりする。

こうした機会と課題を踏まえると、習測定を目的とした教育用アプリケーション向けモデルの選択要素として、近年登場した基盤的なデータサイエンスの方法や標準や技術を理解し取り入れてゆくことが重要となる。これは単に効率化を高めるばかりでなく、垂直方向への標準化を可能な限り促進し、垂直的に利用可能な教育ソリューションの設計、実装、拡大を進めることができる。

さらに、測定とデータに結びついた教育の「edu graph」（図1）は、（最近登場したソーシャルデータによる「ソーシャルグラフ」に似ているが）、様々な専門分野のコンテキストに渡ってその広さと深さを拡大できるという認識が重要だ。こうした専門分野の情報は、エコシステムや教育のワークフローの中にある、管理／業務、カリキュラムの活動とコンテンツ、共同カリキュラム、学習者／教育者のプロフィールや経歴といった情報源によってコンテキスト化されている。

![図1](figure1.png)

** 図1： 「edu graph」の総合的なデータモード **

*こうして改良された学習測定の影響と価値を実現するためには、まずは、edu grapの小さなサブセットに注力することが重要だ。並行して、増加してゆくedu graphの様々なファセットをカバーするために、容易に対応や拡張できる、標準的なソフトウェアサービスのフレームワークの確立も、長い時間をかけて行う。*

本書における提案は、広大な edu-graph の中の「学習グラフ」のファセットを目標としている。それは、重要カリキュラムに関する学習活動とそれに関連した有効性と達成度の測定に、意図的に焦点を当てたものだ。はじめに学習グラフを対象とした根拠はシンプルだ。それは実際の学習コンテキストに焦点を当てるためである。学習コンテキストこそが教育ワークフロー全体の中心であり、そこから生まれる他のコンテキストがさらに深い洞察や価値を加えてゆくからだ。

## 戦略方針

本書の戦略では、IMSによる既存の仕様とこれから加わるはずの仕様を利用した学習測定と分析の手助けによって、学習システムが学習の相互作用に関わるデータをどのように取得して共有するべきなのか、という高レベルの勧告を述べる。

*この戦略では、ソリューションのより総合的な学習分析ドメインを実現する、標準的な測定フレームワークを通じて、秩序をもたらすことを主眼としている点に注意して欲しい。*

IMSとその標準はまず、関連したデータの提示や取得や整備を安定して行う強固な基盤の確立に、役割を果たす必要がある。これによって高次解析ソリューションのエコシステム全体が、大幅に向上し改良されるはずだ。

この目標を前にすすめるために、IMSでは会員組織や供給業者と協力して、**Caliper** という学習測定フレームワークを定義する予定だ。このフレームワークを図2に示す。

*図2におけるCaliperのスコープは左側の緑色の矩形として示される。*

![図2](figure2.png)

**図2：IMS Caliper - 学習測定フレームワーク**

IMS Caliper は次のコンセプトで設計されている。

- **IMS Learning Metric Profiles** は（行動とそれに関連したコンテキストの）評価基準に沿った学習活動中心のフォーカスを提供する。この評価基準は、消費者と生産者がカリキュラムに基づいて活動の利用や編成を行う学習ツールの配信活動や学習プラットフォームにわたって取得される。また独自の拡張や機能をプロファイルに追加できるようにもする。
- **IMS Learning Sensor API および Learning Events** は標準化された計測機器と評価基準の取得を行い、ツールやその配信プラットフォームや、関連した評価基準を収集する解析サービス・ソリューションを整理する。
- **IMS LTI™/LIS/QTI™ leverage and extensionsen** はツールの相互運用性と、講座、学習者、成果などの重要な関連コンテキストを含む基本的な学習情報モデルによって、細かく標準化された学習測定を強化統合する。以後のセクションではこれらのフレームワークの要素について、より詳細に述べる。

### IMS Learning Activity Metric Profiles

一般的に学習カリキュラムは、ひとつ以上の学習活動の集合やシーケンスとして作成、配信される。ほとんどの学習活動は、ひとつの（複合的な活動の場合は、それ以上の）ジャンルにグループ分けされる。ジャンルには、読解、アセスメント、メディア、コラボレーションなどがある。これは学習活動のそれぞれのジャンルを、ベースラインの一貫した評価基準から始まるように、構成し最適化するのに役立つ。

IMS Learning Metric Profiles は **Learning Activity Metrics** の標準化および構造化された集合の定義を目的としている。Learning Activity Metrics はそれぞれの **アクション (action)** に固有の細かい **測定 (measurement)** をあらわす。**アクティビティ（activity）**のそれぞれのジャンルは、アクティビティに対するあらゆるアクションに関連した **コンテキスト(context)** を持っている。さらに、**エンゲージメント(engagement)**やパフォーマンスといった、凡ジャンルの **Foundational Metrics** があり、あらゆるアクティビティについて、汎用的な評価基準による一般的な測定を行うことができる。あらゆる学習活動は（ひとつ以上の）評価基準プロファイルを持つことが可能で、それによって取得と管理が必要なあらゆる<u>メジャーメント</u>を収集し交換する。

IMSではもっとも一般的な学習活動のタイプのために、Learning Metric Profiles の最初の集合を定義する作業を続けている。それは LTI™、LIS、QTI™といった既存の／策定中の／将来計画されているIMS標準のコンポーネントや拡張に使われることだろう。これらのIMS標準では、評価基準に対して取得するコンテキスト要素（情報モデル）を指定している。<u>アクティビティメトリック</u>と情報モデルの両者はメトリックプロファイルを定義する。すなわち、ベースとなる「スキーマ」を提供して、標準ベースの測定とシステム間での学習データの交換を可能にするのである。

図3はIMSが会員や供給業者とともに開発しようとしているMetric Profilesのタイプの（最終決定したものではない）サンプルを示している。

![図3](figure3.png)

**図3: IMS Metric Profiles のサンプル**

IMS Learning Analyticsグループでは <u>メトリックス</u>と、edu-graphの多様な側面に求められる学習や発展の成果を定義するためのさまざまな組織による尽力を、Caliper Metrics Profiles に活用し取り入れてゆく予定だ。そこには次のものが含まれる（限定するものではない）

- [Predictive Analytics Reporting (PAR) フレームワーク][PAR] のデータモデル：IMS Context and Engagement metrics の一部をなす。
- [Common Core Standards][Common Core]：IMS Performance metricsの一部をなす。
- [CAS standards for student developmental and learning outcomes for higher education][CAS standards]：IMS Performance metricsの一部をなす。

### IMS Learning Sensor API および Learning Events

**IMS Sensor API** は**Learning Activity Metric Profiles**と密接に結びついており、学習ツール／システムや関連した学習コンテンツ要素から生まれたデータの計測、収集、交換をサポートする。これによって、どんなAnalytics Storeやその関連APIからも標準的な<u>メトリックス</u>にアクセスできるようになる。

その中核部分として、 **Sensor API** は<u>学習活動</u>の相互作用に基づいた **Learning Event** の交換をサポートする予定だ。図3が示すように、Learning Eventは **-“LearningContext” -“Action” -“ActivityContext”** の三者からなるデータ形式として表現される。これは W3C RDF Triple における "subject/predicate/object" の形式をベースとしている。すなわち、ある目的語（主語）から別の目的語（目的語）やリテラルにリンクするのに述語を経由している。このケースではLearning EventはLearning Activityとともに相互作用の測定を表現することができる。

Learning Event は **Sensor endpoint** によって利用される。これらのエンドポイントは Learning Event を利用しようとするどんなアプリケーションからも利用でき、HTTP/REST といった広く使われているプロトコルをサポートするはずだ。

![図4](figure4.png)

**図4：　IMS Sensor API - Learning Event**

これを可視化する方法としてまず **LearningContext** について述べる。一般に<u>学習コンテキスト</u>とは教育と学習が生まれる環境のことだ。そこには講座、講師、生徒、学習プラットフォーム、プログラム、機関といったものが含まれる。

Learning **Activity** は LearningContext の教育と学習を促進するために導入される。これらの活動には一般に、読解、ビデオ、クイズ、ディスカッションなどが含まれる。通常これらの活動はグループ化され、所定の学習経路に順序づけられる。

最後に、教育と学習の過程において、LearningContext と Activity におけるエンティティ同士の相互作用がある。これを **Action** と呼ぶ。

これら三つのデータセットを **LearningEvent** とする組み合わせは、LearningContext における Activity を伴った相互作用を完全に記述するためのものだ。この三者の組み合わせに加えて、LearningEvent はタイムスタンプを持っている。

図4が示すように、学習の相互作用において、Learning Event の三者のエレメントはそれぞれ、ひとつ以上のエンティティを定義している。これらのエンティティは合わさって、学習環境の中のエンティティの繋がりをベースにした **Learning Graph** を作り上げる。それぞれのエレメントは既存のIMSの仕様と語彙をベースに記述することになるだろう。これは策定中の IMS Learning Activity Metric profiles でも同様である。

Learning Event と Metric Profile は完全にオープンなメカニズムと、学習グラフにおける学習の測定と分析のための厳格なスキーマとのバランスを取ることを意図している。Metric Profile は非常に軽量なスキーマを利用することを意図している。その一方で、Ed Tech コミュニティのニーズをサポートするために、極めて反復的な方法でプロファイルを拡大し、特定のアプリケーション／システムに固有のデータを整備できるようにもする。

またこのメカニズムは、既存の「オープンな」トリプルをベースにしたAPIをSensor APIにマッピングして整備することもできる。そしてこうした既存の「オープンな」APIは、IMS Activity Metric ProfilesにもとづいてLearning Eventを利用する。その一例として Experience/TinCan API が挙げられる。Caliper の Sensor API と Experience API とは、トリプルを介したデータ通信において共通の基盤を共有している。しかし が挙げられる。しかし、Caliper フレームワークは次に示すとおり、そのエコシステムに、より網羅的である。

- Learning Metric Profile を介して学習環境に固有のビューを持つ
- フレームワーク／仕様の重要なコンポーネントとして LTI™ を持つ
- データを相互運用するために、LISやQTI™といった既存の仕様／標準が組み込まれている
- edu-graphの多様な側面に求められる、学習や発展の成果を定義するためのさまざまな組織による尽力を、取り入れようとしている

この両者は次の点において互換性があることに注意して欲しい。

- IMS Learning Event は一般的な subject（主語）-verb（述語）-object（目的語） に変換することで TinCan LRSでも利用できる。
- TinCanのトリプルはIMS Sensor APIで利用できる。（これにはLearning Activity Metric Profileへのマッピングが必要だ。このマッピングは TinCan のトリプルについてのあらゆる有用な分析を始める前に、終えておくべきである。）

しかしながら、TinCanのイベントを扱うフレームワークのような機能は、まったく付加的なものである点に注意するべきだ。なぜなら、Caliper Sensor APIが提供する本来の機能は、学習イベントを取得して整理し、目的の analytics store に送り届けることだからだ。もし TinCan が低レベルのイベント通信として学習活動を含む非常に幅広いコンテキストの追跡に使われているのなら、Caliper Learning Eventに統合マッピングするだけでよい。

### IMS Learning Tools Interoperability および Learning Information ServicesExtensions

IMS Learning Tools Interoperability™(LTI) の仕様は、現在の教育テクノロジーの分野で、相互運用性のメカニズムとして成功を収めており、最も広く使われているもののひとつだ。それは学習システムとツールの統合された学習体験を講師、コース設計者および学習者に提供する。LTIの現在のバージョンは、シームレスな統合運用を可能にしているが、そこで生まれる学習データは、LTIに参加したそれぞれのツールの中で孤立したままだ。そこで IMS では Metric Profile と Sensor API/Learning Event に加えて、次のことができる拡張を定義しようとしている。

- LTI tools can specify one or more metric profiles in their LTI descriptor;
- LTIツールはそのLTI記述しの中でひとつ以上の Metric Profile を指定できるようにする。
- LTI consumers as part of the LTI handshake can specify IMS Sensor API end-point to which the tools can push data conforming to the metric profiles during tool usage.
- LTI ハンドシェイクを構成するLTIの利用者が、IMS Sensor API のエンドポイントを指定することで、ツールが使用時に Metric Profile に適合したデータを送信できるようにする。

図5では、LTIフレームワークに対してこの拡張が意図する範囲を示している（赤くハイライトされた箇所）。

![図5](figure5.png)

**図5： 測定フレームワークをサポートするための IMS LTI の拡張**

これらの拡張によって、LTIの利用者とツールはSensor API を使った Metric Profileに従ってデータを交換できるようになるだろう。

IMSが現在進めている作業は、LISの成果物の穴埋めや拡大を行うために、LTIの拡張を提案するだけでなく、Caliperの導入によって生じたあらゆる不足を補おうとするものだ。例えば、ユニークな個人のIDに関連するアクションのように、あらゆるパラメータ化されたイベントのコンテキストを表現、認可／解決するための方法論を定義して取り入れる活動は、後に続く仕様やフレームワークのワークグループの構想に影響を与えるだろう。

## 適用シナリオ

このセクションではIMS Caliperのすべての要素を適用するシナリオの概要を述べる。IMSの会員組織はこのフレームワークを近い将来実現するべく共同作業を続ける予定であることに注意して欲しい。そのシナリオを図6に示す。ここに示すとおり、関連しあうエンティティには次のものがある。

- **LTI** をサポートする学習プラットフォーム
- LMSのコースに対応した読解とVideoのActivity用の二つの **LTI アプリケーション** 。これらのLTIアプリケーションはいずれも、そのジャンルのための **IMS Learning Activity Metric Profile** と **Sensor API** をサポートし、Sensor APIの **エンドポイント** に **Learning Event** を送信できる。
- IMS Sensor API をサポートした **分析サービス**。この分析サービスは学習プラットフォームに分析ダッシュボードの提供も行う。

![図6](figure6.png)

**図6：IMS Learning Analytics Measurement Framework の適用シナリオ**

このシナリオのイベントシーケンスを次に示す。

- 学習プラットフォームの管理者は、二つのLTIアプリケーションを設定する。LTI configuration URL/XML はこの学習プラットフォームに、これらのアプリケーションがそれぞれ読解とビデオのMetric Profileをサポートしていることを示す。*LTI v2（現在パブリックドラフトの状態）では、LTI アプリケーション／ツールの設定は利用者／ツールの相互作用が実行するREST APIによって自動化される点に注意が必要だ。これによって、LTIの設定は大きく簡略化される。加えて次に示す Sensor Endpoint URLの設定も LTI v2の一部として定義される Tool Proxy Registration flow の中に含めることができる。
- 学習プラットフォームの管理者はLTIの設定の中で Sensor API Endpoint URL を設定する。このURLは Analytics Service によって提供される。この URL は内蔵された API Key 認証アクセスを行うことができる。
- 講師はLTI アプリケーションを使ってReadingとVideoのActivityを登録する。
    * この二つのActivityを登録するために、講師は LTI ランチを初期化する。これらのアプリケーションはIMS Metric Profileをサポートしているので、ランチの間にLMSは Sensor API Endpoint URLをランチパラメータのひとつとして登録する。
    * アプリケショーンはSensor API Endpoint をランチの一部として受け入れ、格納して将来の利用に備える。
- 生徒は学習プラットフォームの中のコースにアクセスを開始し、宿題の一貫としてReadingやVideoを利用し始める。利用する間、生徒は幾つかの典型的なアクションを行う。
    * ページを読む
    * セクションをハイライトする
    * ブックマークを追加する
    * ビデオを見る
    * 特定の再生時間についてメモをとる
- LTI アプリケショーンは生徒のアクションを記録する。学習プラットフォームはランチの間に、Sensor API endpointを提供しているので、個々のアプリケショーンは学習イベントをSensor API endpointに送信し始める。
- Analytics Serviceは
    * IMS Caliper frameworkを介して取得・整理されるメトリックスのための代表的な利用サービスのプロキシである。Analytics Serviceと、接続や蓄積を行うインターフェイスとスタックのようなあらゆる関連サービスは、標準ベースのフレームワークという観点から見て、IMS Caliper frameworkの範囲外となる点に注意して欲しい。
    * 学習イベントを自身のストアに記録する。
    * メトリックスの詳細な分析を、ダッシュボードや推奨／警告、適応シーケンスといった高次の機能によってサポートし、提供する。
    * Analytics Serviceの供給者には、LMSの供給者、適応学習の供給者、予測分析の供給者などが多くあるが、これらに限定されているわけではない。
    * LMSを介して分析ダッシュボードに示されるが、これは Analytics Service の持つ価値の一例にすぎない。学習測定フレームワークを活用した追加機能は、潜在的に LTI アプリケショーンとしてカプセル化され、簡単に他のアプリケショーンのコンテキストに届けることができる。

## 結論と提言

IMS Caliperの学習測定フレームワークは、オンライン学習配信エコシステムの中の非常に深刻な問題に向けれ、価値ある、標準に準拠した、影響力の強いソリューションを示す。現在まで、このエコシステムには、次々に生まれる膨大な供給者からのコンテンツ／学習の活動要素に対して、不十分で一貫性のない断片化した基礎的な測定と評価基準の機能しか持たなかった。
（活動要素の）取得と整備をサポートするフレームワークに従って、それが何であり、何を測定するべきなのかという必要なアラインメントと構造を提供することによって、この IMS Caliper は、達成可能で価値ある開始位置を示すことに注力した。

明らかにCaliperフレームワークは柔軟で拡張可能なものであり、反復的なビルドアウト、改善、機能拡張を容易にする。さらにこのフレームワークは、時間や解空間が発達するにつれて、隣接する他の補完的な分析フレームワークを加えることができる。ここで提案されたソリューションは、価値を与える方向と範囲をシンプルに確立する。

さらなる詳細な定義、仕様およびサポートするサービスフレームワークの実装は、IMSワークグループのロードマップとタスクが優先されるため、今後になるだろう。Caliper の相互依存的な要素の実装のサポートと実現を行うために、さらに重要なこととして、統一された一貫性のある標準的な学習測定のアプローチに合わせるために、この作業はそれぞれの(すなわち Learning Analytics、LTI、LIS、QTIなどの)IMSワークグループの中で行われる、総体的かつ共依存的なものになるだろう。

## 付録 A 用語集

<table>
<thead>
<tr>
<th>用語</th><th>説明</th>
</tr>
<thead>
<tbody>
<tr>
<td>Caliper</td><td>IMSの学習測定フレームワーク。学習活動が生成するメトリックスの標準化された表現、取得および整備を提供し、 Analitics Store/Service を可能にするあらゆる適合 Sensor API endpoint からの利用を目標とする。</td>
</tr>
<tr>
<td>Edu Graph</td><td>アプリケーションとユーザーによる広大なソーシャルネットワーキングエコシステムのデータノード、エッジおよび要素から成るソーシャルグラフのように、edu-graphはオンライン教育エコシステムのために、教育に最適化した広大なデータのグラフを表現する。</td>
</tr>
<tr>
<td>Learning Activity</td><td>一般にレッスンやカリキュラムとして表現される学習シーケンスを単一のコンポーネントにカプセル化するウェブコンテンツや機能を提供する教育アプリケーション（すなわち LTI ツール）。Activityは必要に応じて割り当てや等級付けができる。</td>
</tr>
<tr>
<td>Learning Event</td><td>Learning Activityのコンテキストの中で取得される測定の最小要素であり、Activity Context、Action、Learning Contextから成るジャーナル化された出来事として表現される。</td>
</tr>
<tr>
<td>Learning Graph</td><td>Edu Graph データ・モデルのサブグラフとして、このグラフは学習を中心とした細かいLearning Activityが生成するメトリックスに焦点を当てている。カリキュラムへの参加、パフォーマンス／有効性、Activity固有のコンテキストを持った測定に関連する。</td>
</tr>
<tr>
<td>Learning Information Services (LIS)</td><td><a href="http://www.imsglobal.org/lis/">IMS Learning Information Services specification</a>を参照のこと。</td>
</tr>
<tr>
<td>Learning Tools Interoperability™ (LTI™)</td><td><a href="http://www.imsglobal.org/toolsinteroperability2.cfm">Learning Tools Interoperability specification</a>を参照のこと。</td>
</tr>
<tr>
<td>Metric Profile</td><td>Learning Activity　Agnostic（すなわち、エンゲージメントやパフォーマンスなど） と Learning Activity Genre Specific（すなわち、Reading、Quizzing、Media など）との細かいメトリックスの標準化された集合。Profileは標準的な一貫した形でCaliper frameworkを介したMetricsの取得と整備に利用される。</td>
</tr>
<tr>
<td>Question and Test Interoperability™ (QTI™)</td><td><a href="">IMS Question & Test Interoperability specification</a>を参照のこと</td>
</tr>
<tr>
<td>Sensor API</td><td>Metric Profileに包括的に結び付けられたLearning Eventと、これらのイベントを利用するエンドポイントを含むAPI。</td>
</tr>
</tbody>
</table>