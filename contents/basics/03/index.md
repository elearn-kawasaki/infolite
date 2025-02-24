---
layout: page
title: ネットワークの仕組みと情報検索
date: 2017-05-22 18:34:26 +0900
purposes:
    - ネットワークの仕組みを学ぶ
    - 情報検索について学ぶ
---

<div>
    <div class="panel panel-info">
    <div class="panel-heading">本講に関する学習動画</div>
        <div class="panel-body">
            <p>本講の授業内容に関する【説明動画】が1つあります。サイドメニューの【動画再生】で公開している【図書館とデータベースの利用方法】も必ず視聴してください。</p>
            <p><font color="red">注意：大人数が一斉に動画を再生すると動画が再生されないことがあります。時間をずらして視聴してください。</font></p>

<div id="class_movie"></div>
<p><button type="button" class="btn btn-info pull-right" data-toggle="modal" data-target="#overviewModal">
<!--<p><button type="button" class="btn btn-info" data-toggle="modal" data-target="#overviewModal">-->
<i class="fa fa-play-circle-o fa-lg"></i>&nbsp;説明動画
</button>
<div class="modal fade" id="overviewModal" tabindex="-1" role="dialog" aria-labelledby="overviewModalLabel" aria-hidden="true">
<div class="modal-dialog"><div class="modal-content">
<div class="modal-header">
<button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
<span class="modal-title" id="overviewModalLabel">授業内容</span>
</div>
<div class="modal-body">
<div class="flowplayer is-splash color-light img-responsive" style="max-width:854px;">
<video>
<source type="video/mp4" src="https://infolit.uec.tmu.ac.jp/mov/03_network.mp4">
</video>
</div>
</div>
</div></div>
</div></p>
        </div>
    </div>
</div>

インターネットの仕組み
----------------------

インターネットを利用するにあたり、インターネットの簡単な仕組みについて説明します。これらは講義中だけでなく、今後学内でインターネットを利用して情報収集や電子メールの送受信を行う際に必要な知識となります。

### ネットワークの階層構造

複数のコンピュータがある場合に、コンピュータ同士を相互につなぎ合わせてデータのやりとりができるようにしたものが"ネットワーク"です。研究室や家庭など、限られたエリアのコンピュータでネットワークを構築したものを"LAN（Local Area Network）"と呼びます。
東京都立大学のキャンパス内でも、各研究室、あるいは各建物内にLANが構築されています。これら南大沢キャンパス内のすべてのLANをまとめたネットワーク（学内LAN）には、"TMUNER"という名称がつけられています。

-   [TMUNER](http://www.comp.tmu.ac.jp/tmuner/)

このような、範囲が限られているネットワーク（LAN）同士をつなぎ合わせ、広域にしたネットワークがインターネットです。インターネットの領域は世界に広がっているため、日本に限らない範囲で情報交換が行えます。情報交換の具体的な手段としては、WWW（World
Wide Web）や電子メールなどがあげられます。

このように、インターネットに代表されるコンピュータネットワークは階層化されています。最小の単位としてはネットワークに接続された１台のパソコン（PC）、その次は教室のネットワーク、そして南大沢キャンパス内のネットワーク（TMUNER）、といったように徐々に範囲が広がっていきます。さらに、大学の外はプロバイダによってインターネットに接続されているのです。

{% screenshot net_layer.png "" %}

インターネットのはじまりといえるコンピュータのネットワークは、1960年代後半のアメリカで始まりました。当初は軍事関係の機関を中心に研究開発が進みましたが、しばらくして軍事関係のネットワークは分かれ、その後、徐々に世界各国の大学のコンピュータやネットワークが相互接続されていきました。この研究開発の途中でネットワークの規約が統一されはじめ、メーカーやオペレーティングシステム（OS）、ソフトウェアが異なっていてもインターネットに接続できるようになりました。そして1991年、素粒子物理学研究所（CERN）の研究員ティム・バーナーズ＝リーによって"World Wide Web プロジェクト"が発表されました。その結果、大学などのコンピュータや大型コンピュータだけでなく、家庭用のパソコンまで多くのコンピュータがインターネットに接続され、現在のように無数のコンピュータが結ばれたインターネットが形成されました。

インターネットには国境がなく、世界中のどこにいても同じ情報を手に入れることができます。しかし、インターネットを利用するためには通信回線などのインフラが整備されていなければなりません。世界的にみても、インターネットへの常時接続環境が整っているのは先進国の都市部が中心で、地方や離島では普及が遅れています。このため、情報を手に入れやすい人と手に入れにくい人との間の格差、"デジタル・デバイド（情報格差）"などの新たな問題も生じています。

<table>
<tbody>
<tr>
<th>1957年</th><td>アメリカ国防総省の傘下にAdvanced Research Projects Agency （ARPA）が新設されました。<br />この<strong>ARPAは、後にインターネットの前身となるARPANETを作りました。</strong></td>
</tr><tr>
<th>1961年</th><td>アメリカの電話中継基地が爆破され、国防総省の回線が一時中断した事で、指揮統制系統の重要性が問われるようになり、 国防総省の下でも<strong>通信システムの研究が本格的に始まりました。</strong></td>
</tr><tr>
<th>1965年</th><td>ARPAの<strong>最初の広域ネットワーク実験を実施。</strong><br />マサチューセッツ工科大学とカリフォルニアにある会社のコンピュータをソフトウェアで自動接続する事が出来ました。</td>
</tr><tr>
<th>1969年</th><td>ARPANET開始、接続も次々と成功。<br />UCLA（カリフォルニア大学ロサンゼルス校），UCSB（カリフォルニア大学サンタバーバラ校），スタンフォード研究所，ユタ大学の順に接続点が増えていきます。</td>
</tr><tr>
<th>1972年</th><td>電子メールの基本ソフトウェア誕生。</td>
</tr><tr>
<th>1974年</th><td>公衆パケット交換網サービス開始。</td>
</tr><tr>
<th>1976年</th><td>ダイヤルアップ接続の開発。<br /><strong>一般の電話回線からメールやファイルを間欠的に送受信できるようになりました。</strong></td>
</tr><tr>
<th>1989年</th><td>World Wide Web（WWW)とHTML、HTTPの誕生。</td>
</tr><tr>
<th>1995年</th><td>Windows95、Internet Explorerの登場。<br />これによって、一般の人達がより簡単にインターネットを見ることが出来るようになり、 インターネット人口が爆発的に増えるきっかけとなりました。</td>
</tr>
</tbody>
</table>

### ネットワーク上の規約（TCP/IP）

インターネットにはさまざまなメーカーのコンピュータが接続されていて、オペレーティングシステム（OS）も、使われているソフトもばらばらです。この環境の違いを気にせずインターネットを使うことができるのは、"共通の情報通信規約"が決められているからです。この規約のことを"プロトコル（Protocol）"と呼びます。プロトコルにはさまざまな種類がありますが、インターネットで主に利用されているプロトコルは"TCP/IP（Transmission
Control Protocol / Internet Protocol）"と総称されています。

TCP/IPのうち代表的なプロトコルについて、機能を紹介します。

<dl>
<dt>WWW（World Wide Web） [HTTP]</dt>
<dd>文章の中に画像や映像などを埋め込み、それぞれを互いに結びつけた仕組みです。</dd>
<dd>WWWにおける情報はInternet Explorerなどの"Webブラウザ"を使うことで誰でも自由に閲覧することができます。この情報は"HTML（HyperText Markup Language）"という簡単な言語を使って記述されているため、誰でも手軽に情報を発信することもできます。また、文章中に設定されている"ハイパーリンク"によって、他の情報へ簡単に移動することができることも特徴のひとつです。この機能によって情報同士が複雑に結び付けられ、まるでクモの巣のようになっていることから"Web"という名前がつけられているのです。みなさんが"インターネット"という言葉で連想するのはこのサービスのことでしょう。</dd>
<dt>電子メール（E-Mail） [SMTP, POP, IMAP]</dt>
<dd>特定の相手に文章を送るための仕組みです。</dd>
<dd>"メールサーバ"に個人のメールボックス（私書箱）を設置しておき、メーラー（メールを読み書きするためのソフト）をインストールしたパソコンからメールを読み書きします。メールサーバには、送信に利用するSMTP（Simple Mail Transfer Protocol）サーバと、受信に利用するPOP（Post Office Protocol）またはIMAP（Internet Message Access Protocol）サーバの２種類があります。個人のパソコンからのメールを SMTPサーバが受け取ると、宛先のメールサーバに送られます。外からのメールも一度SMTPサーバが受け取り、私書箱を管轄するPOP/IMAPサーバにメールの管理を委ねます。以下がその概念図です。</dd>
</dl>

{% screenshot net_mail.png "" %}

<dl>
<dt>ファイル転送 [FTP]</dt>
<dd>ネットワークに接続されたコンピュータに保存されているデータを計算機間で転送し、やりとりすることができる仕組みです。</dd>
<dd>例えばパソコンでWebページ（HTMLファイル）を作り、それを自分のWebページ用のサーバに転送する（アップロード）ことによって、Webページをインターネット上に公開することができます。この利用方法ではサーバの利用権が必要なのですが、不特定の利用を可能にする匿名FTP（Anonymous FTP）というのもあります。</dd>
<dt>リモートログイン [SSH, Telnet]</dt>
<dd>ネットワークに接続されたコンピュータを、離れたところから利用することができる仕組みです。</dd>
<dd>一般的なパソコンは原則として一人で一台を利用する仕組みになっていますが、UNIXサーバなどの大型コンピュータはマルチユーザ（複数利用者）の環境に対応しています。これらの大型コンピュータはパソコンよりも高度な演算をすばやく行うことができるため、研究などの用途で複数が一台を利用するという状況がでてくるわけです。東京都立大学の学内にもこの大型コンピュータがあり、ネットワークを通して研究のために利用されています。</dd>
</dl>

### IPアドレスとドメインネーム

インターネットには無数のコンピュータが接続されています。そのため、コンピュータを指定するために住所が使われています。

インターネット上の住所にあたるものは"IPアドレス"（Internet Protocol Address）と呼ばれます。これは0~255の数字を4つ組み合わせたもので、それぞれは"."（ピリオド）で区切られています。

>   133.86.26.1

"133.86."という番号は東京都立大学南大沢キャンパスをさします。その次の２組の数字は東京都立大学の場合、教室や建物のネットワーク、ネットワーク内のコンピュータの番号というつけ方になっています。
"26"であれば1号館3階の320教室、そして"1"というのは320教室の1番目の端末です。
このIPアドレス（IPv4）は、256の4乗分、つまり約43億個のアドレスを設定することができるためインターネット上で重複することがありません。そのため、世界のどこからでもこの133.86.26.1というIPアドレスは常に"都立大南大沢1号館320教室の1番機"のことをさしています。

しかし、このIPアドレス(IPv4)は、約43億個のIPアドレスを設定できますが、近年のインターネット人口の増加によってIPv4では足りなくなってきました。
そこで最近では、今までのIPv4（Internet Protocol version 4）に代わる新たな規格としてIPv6（Internet Protocol version 6）が提案されています。このIPv6というIPアドレスは、以下のように0~65535までの数字を16進数で表した上で、8つ組み合わせ、":"（コロン）で区切られて表記されます。

>   123:4567:89ab:cdef:123:4567:89ab:cdef

このIPv6では、340澗（かん）個（約43億の4乗個）と無限に近い数のアドレスを設定することができるため、これからのインターネットの広がりに対しても十分に対応することが可能です。

-   [IPv6ことはじめ](http://www.v6pc.jp/jp/whats/index.phtml)（[IPv6普及・高度化推進協議会](http://www.v6pc.jp/jp/)より）
-   [IPv4アドレスの在庫枯渇に関して](http://www.nic.ad.jp/ja/ip/ipv4pool/)（[JPNIC](http://www.nic.ad.jp/ja/)より）

IPアドレスは番号なので、そのアドレスがどこのどういうコンピュータを示しているのか分かりません。そこで、通常はコンピュータにつけた名前を使った表記を使います。こちらの住所表記を、"ドメインネーム"と呼びます。

>   www.tmu.ac.jp

ドメインネームは階層に分けることができます。末尾から順に見ていくと、日本（jp）の学術団体（ac）である東京都立大学（tmu）にあるWebサーバ（www）という意味になっています。この階層わけの見方がわかると、ドメインネームを見るだけでどこの国のどのような組織にあるコンピュータの情報なのかすぐわかるようになります。

東京都立大学にあるすべてのコンピュータには名前がつけられ、すべて固有のIPアドレス・ドメインネームがつけられています。公開されているサーバ（コンピュータ）に関しては、これらのIPアドレスやドメインネームを指定することで決められたプロトコルで情報をやり取りすることができます。

Webブラウザでウェブサイトを見るときには、自分が見たいページのアドレスをアドレスバーに入力します。このアドレスは、"URL（Uniform Resource Locator）"の形式であらわされています。例えば東京都立大学のウェブサイトを見る場合、入力するアドレスは "https://www.tmu.ac.jp/" となります。今まで説明してきたことを踏まえて考えると、これは「日本（jp）の学術団体（ac）である東京都立大学（tmu）にあるWebサーバ（www）にいって、WWWのプロトコル（http）で情報を見る」という意味になっているわけです。

また、URLは場所によって表記が異なる場合があります。

-   https://www.yahoo.co.jp/ （Yahoo!Japan）
-   http://www.kisokyo.tmu.ac.jp/kyomu/ （東京都立大学 大学教育センター教務課）
-   https://www.tmu.ac.jp/for_students.html （大学ウェブサイト内の在学生へのお知らせ）

Yahoo!の場合はもっともシンプルで、「日本（jp）の商用組織（co）であるYahoo!（yahoo）にあるWebサーバ（www）」というドメインネームがそのままURLになっています。
2番目の教務課の場合は、ドメインネームで指定した「日本（jp）の学術団体（ac）である東京都立大学（tmu）の中の大学教育センター（kisokyo）にあるWebサーバ（www）」というドメインネームに加え、「そのサーバの中の"kyomu"というディレクトリ（フォルダ）の中にある情報」というURLとなっています。
また、3番目のお知らせについては「日本（jp）の学術団体（ac）である東京都立大学（tmu）にあるWebサーバ（www）」というドメインネームに加えて、「そのサーバの中の"for_students.html"というファイル」という具体的なファイルまで指定したURLになっています。

ドメイン名の一番右側に表記される文字を「トップレベルドメイン」と呼びます。東京都立大学のウェブサイト（http://www.tmu.ac.jp/）では「jp」にあたります。

このトップレベルドメインは大まかに以下の２つに分けられます。

<dl>
<dt>分野別トップレベルドメイン（gTLD）</dt>
<dd>登録にあたって一定の条件があるものや、誰にでも登録できるものなど、さまざまなドメイン名があります。</dd>
<dt>国コードトップレベルドメイン(ccTLD）</dt>
<dd>国際規格であるISO 3166によって、２文字の国コードが定義されています。その国内の個人や企業が使用することを想定しているドメイン名ですが、誰にでも取得できるようにしているものもあります。</dd>
</dl>

<div class="row">
<div class="col-sm-6">
<table>
<thead>
<tr>
<th colspan="2">分野別トップレベルドメインの例</th>
</tr>
</thead>
<tbody>
<tr>
<td>com</td>
<td>商業用</td>
</tr><tr>
<td>edu</td>
<td>教育機関用</td>
</tr><tr>
<td>gov</td>
<td>米国政府機関用</td>
</tr><tr>
<td>net</td>
<td>ネットワーク用</td>
</tbody>
</table>
</div>
<div class="col-sm-6">
<table>
<thead>
<tr>
<th colspan="2">国コードトップレベルドメインの例</th>
</tr>
</thead>
<tbody>
<tr>
<td>jp</td>
<td>日本</td>
</tr><tr>
<td>uk</td>
<td>イギリス</td>
</tr><tr>
<td>to</td>
<td>トンガ</td>
</tr><tr>
<td>tv</td>
<td>ツバル</td>
</tr>
</tbody>
</table>
</div>
</div>

トップレベルドメインはどんどん新しいものが増え、分類なども変化しています。興味があれば、インターネットなどを活用して調べてみましょう。

では、実際にTCP/IPやコンピュータネットワークについてネットワークツールを使って調べてみましょう。

<div class="alert alert-warning" role="alert">
<strong>情報処理教室における制約事項</strong>
<p>情報処理教室では、コンピュータの不正な使用を防止するために、機能に一定の制限を設けてあります。したがって、以下で扱うツールの一部に関しては、情報処理教室では使えないものもあります。</p>
<p>これについては、本節末にリンクを設けましたので、外部のWeb上のサービスなどを参考にしてください。</p>
</div>

### ipconfig

ipconfigは、IPアドレスなどネットワークインターフェイスについてのチェックや設定に用いられるネットワークツールです。 まず、[スタートメニュー] - [すべてのプログラム] - [アクセサリ] - [コマンド プロンプト]を開きます。

{% screenshot cmd.png "コマンドプロンプト" %}

次に、以下のように入力し、エンターキーを押します。すると、今使っているコンピュータのIPアドレスなどが表示されます。

    ipconfig

{% screenshot ipconfig.png "ipconfig" %}

### nslookup (name server lookup)

次に`nslookup`を使ってみます。 nslookupは、インターネットのネームサービスであるDNS(Domain Name System)へ名前の問い合わせに用いられるネットワークツールです （DNSは、コンピュータのホスト名をIPアドレスと関連づけているシステムです）。
以下のように入力し、エンターキーを押してください。 この時、半角スペースを忘れないよう注意してください。

    nslookup www.tmu.ac.jp

{% screenshot nslookup.png "nslookup" %}

ここで表示されているのはwww.tmu.ac.jp、つまり東京都立大学のWebサイトのIPアドレスです。複数のIPアドレスがあるのは、本学ウェブサイトへの集中したアクセスがあった際の対応として、各サーバに負荷を分散しているからです。

nslookupでは、逆にIPアドレスからドメインネームを得ることもできます。 
コマンドプロンプトに`nslookup `と入力し、続けて先ほど分かった東京都立大学のWebサイトのIPアドレスを入力してください。 その後、エンターキーを押してください。

    nslookup 49.212.138.160

{% screenshot nslookup_rev.png "nslookup による逆引き" %}


情報検索
--------

### 情報検索とは

1990年代後半からＷＷＷは爆発的な勢いで拡大していき、ＷＷＷ上にある情報量も膨大な量となっていきました。
その大量にある情報の中から必要な情報を抽出するために、注目されたのが「情報検索」の技術でした。

ここからはその情報検索について学び、実際にブラウザを利用しながら必要な情報を手に入れるためのスキルを身につけていきましょう。


WWWでの情報検索
---------------

### ブラウザ利用と初期設定ホームページ

情報処理教室のパソコンでは、Webを閲覧するソフト（Webブラウザ）として"Microsoft Edge"が用意されています。

Edge を起動したときに最初に表示されるページ（ホーム）は、TMUNER（http://www.comp.tmu.ac.jp/tmuner/）になっています。このウェブサイトには、本学のパソコンの利用方法や、インターネットを利用する際に重要な情報が掲載されています。更新されたら必ず目を通すようにしましょう。

-   [TMUNER](http://www.comp.tmu.ac.jp/tmuner/)

ブラウザには、よく訪れるウェブサイトをお気に入りとして登録しておく機能がついています。Edge ではハブの"お気に入り"で操作することができます。他のブラウザでは名称が違うこともありますが、同様の機能があります。
また、インターネットの情報は日々更新されているため、今見ているページが将来削除されたり、あるいは改変される可能性があります。ページを自分のパソコンに保存することでいつでも保存した時の情報を見ることができます。

### URLとアドレスバー

先ほど説明したとおり、Webブラウザでは自分が見たいページのアドレスを直接ブラウザ上部のアドレスバーに入力します。

{% screenshot edge_tmuner.png "Edge のアドレスバー" %}

### サーチエンジン

Webではさまざまな人が情報を発信しているため、その情報量はとても膨大です。知りたい情報がある場所（URLなどで示されるアドレス）がわかっている場合はすぐにたどり着くことができますが、多くの場合は検索機能を使って求める情報を探すことが必要となります。検索はみなさんがインターネットを使う上で日常的に行っていると思いますが、より効率のよい検索ができるよう簡単に説明していきます。

検索機能を提供しているシステムのことを、検索エンジン（サーチエンジン）と呼びます。

<dl>
<dt>全文検索（ロボット）型</dt>
<dd>googleに代表される検索エンジンです。</dd>
<dd>ロボットと呼ばれるソフトウェアがインターネット上のウェブサイトを巡回し、自動的に情報を収集してデータベース化します。ユーザーが検索フォームからキーワード検索を行うと、データベースに基づいてすべてのウェブサイトの文章を検索し、全て表示します。
長所としては、情報量が多い、データベースの更新頻度が高いことが挙げられます。その一方で、関係のない情報が結果に含まれることも少なくないという短所もあるため、以下に示す検索テクニックを活用して情報を取捨選択することが重要です。</dd>
</dl>


### 検索テクニック

検索を行うにあたって、様々な検索で使える共通のテクニックというものが少なからず存在します。
演算子等を利用した方法や検索するためのキーワードの取り方などがこれに当たります。ここからはそういった検索テクニックを見ていきましょう。

演算子等（半角大文字）には次のようなものがあり、検索ボックスにそのまま入力して使います。

<table>
<thead>
<tr>
<th>演算子等</th>
<th>意味</th>
<th>例</th>
<th>説明</th>
</tr>
</thead>
<tbody>
<tr>
<td>AND</td>
<td>両方を含む</td>
<td><code>情報 リテラシー</code>（複数の単語を半角スペースで区切る）</td>
<td>「情報」と「リテラシー」の両方を含む</td>
</tr><tr>
<td>OR</td>
<td>いずれかを含む</td>
<td><code>情報 OR リテラシー</code></td>
<td>「情報」もしくは「リテラシー」のいずれかを含む</td>
</tr><tr>
<td>NOT</td>
<td>含まない</td>
<td><code>-情報</code>（単語の前に半角ハイフンをつける）</td>
<td>「情報」を含まない</td>
</tr><tr>
<td>""</td>
<td>完全に一致</td>
<td><code>"情報リテラシー"</code></td>
<td>「情報リテラシー」に完全に一致する文字列を含む</td>
</tr>
</tbody>
</table>

{% screenshot search_technique.png "演算子のイメージ" %}

また、ロボット型の検索エンジンの代表であるgoogleには応用的な機能がついています。単位換算や乗換案内など、特定のウェブページを調べる以外の用途にも利用することができます。また、WEB上の検索エンジンでは、簡単な計算を実行したり、英語名から日本語名を調べたりすることもできます。

{% appendix ../appendix/google.html "googleの使い方" %}


学術情報の検索
----------

この実習は以下のスライドに沿って進めます。

-   [学術情報検索実習](library.pdf)

1.  東京都立大学の図書館概要
1.  学術情報に関する重要ポイント－学術情報・情報メディア・情報の信頼性
1.  図書を探す
1.  論文（記事）を探す
1.  図書館が提供するサービス

### 学術情報の定義

学術情報とは、
>“学術研究の成果として生み出された情報およびそれがさらに編集、圧縮、加工されて生成された情報。観測、測定、計算データや記録、学術文献（学術論文、報告書、学術図書や書誌、索引誌、抄録誌など）、それに個人的なコミュニケーションが含まれる。（以下略）”
> 日本図書館情報学会用語辞典編集委員会『図書館情報学用語辞典第4版』丸善出版, 2013. p.32

つまり、「研究活動の中で生み出される情報」が学術情報だといえるでしょう。

イメージしやすいものとしては、論文、図書、データ、などが挙げられます。
これらの学術情報の中から、今回は"図書"について取り上げ、検索の仕方を具体的に学んでいきます。


### 図書の検索

東京都立大学図書館のウェブサイトからは、本学に収蔵されている図書を中心に、レポート作成や研究に有用な資料の場所を検索することができます。蔵書を検索するためには、図書館のトップページから[蔵書検索]を利用します。

実際に、東京都立大学図書館で検索をしてみましょう。今回は、以下の図書を検索してみます。

> 千野信浩『図書館を使い倒す! : ネットではできない資料探しの「技」と「コツ」』 (新潮新書 ; 140) 新潮社, 2005

まず、東京都立大学図書館のページを開いてください。

-   [東京都立大学図書館](http://www.lib.tmu.ac.jp/)

&#9312; 画面中央付近の水色の蔵書検索ボックスをクリックします。この時に、[詳細検索]を選択するとより詳細な設定で、[横断検索]を選択すると一部学外のデータベースからも検索することができます。


{% screenshot opac1.png "" %}

&#9313; 調べたい本の情報を入力します。今回は少し曖昧なキーワードで検索してみます。「図書館　コツ」と入力して検索してみましょう。

{% screenshot opac2.png "" %}

&#9314; 結果が表示されました。キーワードに当てはまる図書が複数あることがわかります。このうち探していた『図書館を使い倒す! : ネットではできない資料探しの「技」と「コツ」』の図書名をクリックします。

{% screenshot opac3.png "" %}

&#9315; すると、『図書館を使い倒す! : ネットではできない資料探しの「技」と「コツ」』は本館（南大沢）の 2 階一般書架や日野館の小型本コーナー、荒川館の新書コーナーに貸し出し用のものがあるようだとわかりました。

{% screenshot opac4.png "" %}



探している本が本学にない場合には、他のどこの図書館にあるのかを調べることができます。大規模な検索サービスとしては、全国の大学図書館の所蔵から検索できる"CiNii Books"や、国立国会図書館の所蔵から検索できる"NDL-OPAC"などが代表的です。

-   [CiNii Books](http://ci.nii.ac.jp/books/)
-   [NDL-OPAC](http://opac.ndl.go.jp/)

このほか、著作権の切れた小説や古文書的な図書などを検索・閲覧できるサービスもあります。

-   [近代デジタルライブラリー](http://kindai.ndl.go.jp/)（国立国会図書館）
-   [青空文庫](http://www.aozora.gr.jp/)

{% appendix ../appendix/dbsample.html "特殊なデータベースの検索例" %}

### 図書館の案内

東京都立大学図書館では、学内で利用可能な電子リソース（本・雑誌、論文・記事、辞書・辞典、新聞記事などの文献検索データベース）を「学術情報をオンラインで利用しよう」にまとめ、提供しています。
冊子版は、図書館本館と学部学科図書室にて受け取ることができます。
PDF版の閲覧については、学内者限定公開の資料となっています。以下のウェブサイトをご参照いただき、注意事項を確認した上で、kibacoの図書館講習会コースからアクセスしてください。

-   [学術情報をオンラインで利用しよう](https://www.lib.tmu.ac.jp/minami-osawa/news/11661.html)

また、図書館本館の利用については、PDF版の「本館利用のしおり」が公開されています。

-   [図書館本館利用のしおり](https://www.lib.tmu.ac.jp/minami-osawa/guide.html)





練習問題1
---------

1.  以下のトップレベルドメイン（ドメイン名の一番右側に表記される文字）について、その用途を調べてみましょう。
    1. .jp
    1. .edu
    1. .gov
    1. .uk
    1. .to


練習問題2
---------

インターネットを活用して、以下の設問について情報を集め、自分の言葉でまとめてください。また、検索に用いたサイトや情報を引用したページについても説明をつけてください。

1.  サッカー用語でボランチとはどういう動作を担当する役割で、もともとはどういう意味でどこからきたものかまとめてください。
1.  5月27日10：00に南大沢駅を出発して、大岡山駅まで電車で行く経路のうち最短時間のものを調べて、説明してください。
1.  羽田空港を出発して6月1日12：00までに徳島空港に到着する適当な航空便を検索して、その便名をまとめてください。
1.  高校に専門科目として「情報」がおかれた理由を調べてください。また、公式には何を根拠にして、いつから実施されたかをまとめてください。


タイピング練習
--------------

第１講で行ったタイピング練習について、担当教員の指示に従い、終わらなかった問題を入力してみましょう。

-   [問題１](../01/typing_1R.pdf)
-   [問題２](../01/typing_2R.pdf)
-   [問題３](../01/typing_3R.pdf)
-   [問題４](../01/typing_4R.pdf)

各例文ごとに別のファイルに保存しましょう。
なお例文だけ打ち込んであとでプリントすると、どのプリントが誰のであるかわからなくなります。またファイルを提出する場合もファイル名だけでは認証が面倒となります。例文に先立ち自分の**学修番号**と**名前**および自分だけ判るメッセージを入れてください。


参考リンク
----------

### 学内サイト

-   [TMUNER](http://www.comp.tmu.ac.jp/tmuner/)
-   [東京都立大学図書館](http://www.lib.tmu.ac.jp/)
-   [図書館刊行物](http://www.lib.tmu.ac.jp/publication.html)（東京都立大学図書館）

### 学外サイト

-   [Yahoo! Japan](http://www.yahoo.co.jp/)
-   [google](http://www.google.co.jp/)
-   [WEB Directory](http://park18.wakwak.com/~directorys/)
-   [Bing](http://www.bing.com/)
-   [CiNii Books](http://ci.nii.ac.jp/books/)
-   [NDL-OPAC](https://ndlopac.ndl.go.jp/)
-   [Webcat plus](http://webcatplus.nii.ac.jp/)
-   [近代デジタルライブラリー](http://kindai.ndl.go.jp/)（国立国会図書館）
-   [青空文庫](http://www.aozora.gr.jp/)


