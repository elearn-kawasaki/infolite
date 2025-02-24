---
layout: page
title: 表計算ソフトによるデータ処理 （２）
date: 2016-03-15 17:02:54 +0900
purposes:
    - Microsoft Excelを用いたグラフ作成方法の習得
flowplayer_conf:
    - embed: false
    - ratio: 0.75
---

<div>
    <div class="panel panel-info">
        <div class="panel-heading">本講に関する学習動画</div>
        <div class="panel-body">
            <p>本講の授業内容に関する【説明動画】が2つあります。これらの動画に加えて、本講で作成するファイルを完成させるために必要なExcelの機能について詳細に説明している【操作動画】もあります。操作動画は、その機能について説明している箇所で視聴できます。</p>
            <p><font color="red">注意：大人数が一斉に動画を再生すると動画が再生されないことがあります。時間をずらして視聴してください。</font></p>

            <div id="class_movie"></div>
            <p>
                <button type="button" class="btn btn-info pull-right" data-toggle="modal" data-target="#overview">
                    <!--<p><button type="button" class="btn btn-info" data-toggle="modal" data-target="#autosumModal">-->
                    1. 演算子・式・参照・関数について<i class="fa fa-play-circle-o fa-lg"></i>&nbsp;説明動画
                </button>
                <div class="modal fade" id="overview" tabindex="-1" role="dialog" aria-labelledby="overviewModalLabel" aria-hidden="true">
                    <div class="modal-dialog">
                        <div class="modal-content">
                            <div class="modal-header">
                                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                                <span class="modal-title" id="overviewModalLabel">授業内容</span>
                            </div>
                            <div class="modal-body">
                                <div class="flowplayer is-splash color-light img-responsive" style="max-width:854px;">
                                    <video>
                                        <source type="video/mp4" src="https://infolit.uec.tmu.ac.jp/mov/xl01_basic2.mp4">
                                    </video>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </p>
            <br /><br />
            <p>
                <button type="button" class="btn btn-info pull-right" data-toggle="modal" data-target="#graph">
                    <!--<p><button type="button" class="btn btn-info" data-toggle="modal" data-target="#autosumModal">-->
                    2. グラフ作成について<i class="fa fa-play-circle-o fa-lg"></i>&nbsp;説明動画
                </button>
                <div class="modal fade" id="graph" tabindex="-1" role="dialog" aria-labelledby="graphLabel" aria-hidden="true">
                    <div class="modal-dialog">
                        <div class="modal-content">
                            <div class="modal-header">
                                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                                <span class="modal-title" id="graphLabel">授業内容</span>
                            </div>
                            <div class="modal-body">
                                <div class="flowplayer is-splash color-light img-responsive" style="max-width:854px;">
                                    <video>
                                        <source type="video/mp4" src="https://infolit.uec.tmu.ac.jp/mov/xl02_graph.mp4">
                                    </video>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </p>
        </div>
        </div>
</div>


関数、絶対参照と相対参照
------------------------

**関数**、**絶対参照と相対参照**は、Excelを初めとする表計算ソフトにおいて、とても重要な機能の一つです。
関数を用いることで、色々な種類の複雑な計算を一瞬で導き出すことができます。
また、絶対参照と相対参照を行うことによって、無限に続くとも思える数値を入力せずに計算を行うことができます。

次のファイルをダウンロードして、Excelで開いてください。そして、表を完成させてみましょう。

-   [いちご狩りファイル(ichigo.xlsx)](./ichigo.xlsx)

{% screenshot itigo.png "いちご狩りファイルの初期状態" %}
   
{% screencast function_insert "関数の使い方" %}

### SUM関数

    =SUM(数値1,[数値2],...)

`()` 内の数値の総和を出す関数です。

&#9312; まず、各人のいちごの"合計(g)"を求めます。前回説明していますので、復習のつもりでやってみましょう。 "F3" を選択します。

&#9313; 次に[ホーム]リボン - [編集]タブ - [オート SUM]をクリックします。

{% screenshot sum1.png "オートSUM（ポップヒント：オートSUM）" %}

&#9314; すると、自動的に選択範囲が関数に入力されます。[Enter]を押すと、総和が "F3" に入力されます。

{% screenshot sum2.png "オートSUMを押した結果" %}

### 相対参照

&#9312; オートフィルを使って、全ての合計を出します。選択したセルの右下にある[■]の上にカーソルを持って行き、一気に "F12" まで引き延ばします。

{% screenshot sum3.png "計算結果のオートフィル：十字カーソル合わせ" %}

{% screenshot sum4.png "計算結果のオートフィル：下までドラッグ" %}

&#9313; ところでExcelの数式の部分に注目します。

{% screenshot sum5.png "数式バー" %}

&#9314; 次に "F12" に選択します。すると、数式が変わりました。

{% screenshot sum7.png "数式の自動変化" %}

{% screenshot sum6.png "数式の自動変化（注目）" %}

オートフィルはコピー＆ペーストと同じ機能を果たしています。
しかし、ペーストされたのは、セル番号が違う数式です。
つまり、コピーされたセルに記録されていたのは、セル番号ではなく、セルの位置です。
これが**相対参照**です。

相対参照は入力されているセルを基点として、各セルの位置を記録しておく参照方法です。
そのため、コピー＆ペーストした結果、ペーストされたセルから同じだけ移動した位置にあるセルを参照します。

{% screenshot sum8.png "参照部分の自動移動" %}

### AVERAGE関数

    =AVERAGE(数値1,[数値2],...)

`()`内の数値の平均を出す関数です。

&#9312; 各人が平均でどのくらいのいちごを採ったのか、調べてみましょう。まず "E13" を選択し，`平均` と入力します。

&#9313; 次に、"F13" を選択します。[ホーム]リボン - [編集]タブ - [オートSUM]の[▼] - [平均]をクリックします。

{% screenshot average1.png "編集タブから平均を選択" %}

{% screenshot average2.png "平均" %}

&#9314; [Enter]を押します。すると、平均が出てきました。

{% screenshot average3.png "平均計算結果" %}

{% screencast function "関数の使い方" %}

### RANK関数

    =RANK(数値,範囲,順序)

範囲内の数値が何番目の順位かを導き出します。順序には `0`（降順／高い方が順位が高い）か `1`（昇順／低い方が順位が高い）が入ります。

&#9312; 誰が一番食べたのか。関数で出すことができます。 "A3" を選択します。

&#9313; [ホーム]リボン - [編集]タブ - [オート SUM]の[▼] - [その他の関数]をクリックします。もしくは、[数式]リボン - [関数ライブラリ]タブ - [関数の挿入]をクリックします。

{% screenshot rank1.png "編集タブからその他の関数" %}

&#9314; 関数の検索で検索をかければ出てきますが、ここでは[関数の分類] - [統計] - `RANK.EQ` - [OK]をクリックします。

{% screenshot rank3.png "関数の挿入から「統計」" %}

{% screenshot rank4.png "出てきた関数「RANK.EQ」を選択" %}

&#9315; 関数の引数のウインドウの数値に順位を調べたい数値を入れます。ここでは、 "F3" を選択します。

&#9316; 次に範囲を比べる数値の全体を選択します。ここでは "F3" から "F12" までを選択します。さらに順序を降順にするために `0` と入れます。

{% screenshot rank5.png "関数の引数（ひきすう）ウィンドウ" %}

{% screenshot rank6.png "関数の設定項目" %}

&#9317; [Enter]を押します。すると、上杉の食事量の順位が出ました。

{% screenshot rank7.png "関数設定の結果" %}

### 絶対参照

&#9312; オートフィルを使って、各人の順位を出します。 "A3" から "A12" まで伸ばします。

&#9313;  "A5" と "A6" 、 "A11" を見てください。`2` が３つあります（緑枠）。これは順位としておかしいので、修正しなくてはなりません。 "A12" を選択して、数式に注目してください。相対参照しているため、RANK関数の範囲がずれていることがわかります。（赤枠がA3の範囲、青枠がA12の範囲を表す）

{% screenshot rank8.png "相対参照の弊害" %}

&#9314; ここで、絶対参照を使って、正しい順位を導き出しましょう。まず "A4" から "A12" までを選択 - 右クリック - [数式と値のクリア]でクリアします。

&#9315;  "A3" を選択します - 数式バーの範囲の部分の "F3" にカーソルを移します - [F4] キーを押します。

{% screenshot rank9.png "参照セルの固定" %}

&#9316; "F3" が "＄F＄3" に変わりました。`$` がついた列・行は、固定された状態になります。これが絶対参照の状態です。同様に "F12" も [F4] キーで絶対参照の状態にします。

&#9317; オートフィルで先ほどと同じように "A3" から "A12" まで伸ばします。

&#9318; 先ほどとは違う結果が出ました。 "A12" を選択して、範囲が変わっていないことを確認してください。

{% screenshot rank10.png "正常化された順位" %}

これが**絶対参照**です。
絶対参照は表計算ソフト上のセル番号で位置を記録しておく参照方法です。
どの位置にあっても、同じセルを参照することができます。
絶対参照と相対参照をうまく使い分けることによって、より便利にExcelを使うことができます。

### ROUNDUP関数

    =ROUNDUP(数値,桁数)

指定した桁数になるように数値を切り上げます。

&#9312; 各人の料金を出します。Gの列を選択して、右クリック - [挿入]をクリックします。 "G2" に `あまおう（円）` と入力します。

&#9313; 次に "G3" を選択します - [ホーム]リボン - [編集]タブ - [オートSUM]の[▼] - [その他の関数]をクリックします。もしくは、[数式]リボン - [関数ライブラリ]タブ - [関数の挿入]をクリックします。

&#9314; "関数の検索"で"切り上げ"の検索をします。候補の中から `ROUNDUP` を選択して、[OK]をクリックします。

{% screenshot roundup1.png "関数の挿入から「ROUNDUP」を選択" %}

&#9315; 今回は、あまおうの値段が 100g単位であるため、数値に `C3/100` と入れます。

&#9316; 次に桁数に `0` を入れます。ここで指定した桁数より下の位の数字が存在する場合、指定した桁数になるように切り上げされます -[OK]をクリックします。

{% screenshot roundup2.png "引数の設定" %}

数値は `0.98` ですが、切り上げになるので、 `1` になります。ここでは、セルの表示形式を "通貨" にしておくと、' &yen; 1 ' と表示され、料金らしくなります。

&#9317; これだけでは、料金になりません。続いて、数式バーにカーソルを移して、数式を完成させましょう。 `=ROUNDUP(C3/100,0)` の後に `*` と打ち、 "J3" を選択します。[F4]キーを押して、絶対参照にするのを忘れないでください。最終的に、 `=ROUNDUP(C3/100,0)*$J$3` とします。

{% screenshot roundup3.png "計算式の追加" %}

これで上杉のあまおうの料金が導き出されました。このようにして、関数は数式の中に入れることもできます。

&#9318; オートフィルで "G3" から "G12" まで伸ばして、料金を全て出しましょう。正しくできていれば、このようになります。

{% screenshot roundup4.png "料金計算の結果" %}

&#9319; これだけでは、あまおうの料金しか求められていません。時間に余裕があれば、他の品種の料金も求めてみてださい。

切り上げの他にも `=ROUNDDOWN(数値,桁数)` という切り捨てや `=ROUND(数値,桁数)` という四捨五入の関数もあります。 


基本グラフの作成
----------------

前回まではデータを数値のままで扱ってきましたが、今回は、数値からグラフ化することで、より視覚的にわかりやすくするための方法を学びます。
データファイルは、前回作成した人口統計表のデータファイルを使用します。

{% screenshot populationfinal.png "前回の授業の人口データ" %}

### グラフの作成

{% screencast graph "グラフの作成" %}

実際にグラフを作成してみましょう。

&#9312; まず、グラフを作成したい領域を選択します。

&#9313; 次に、[挿入]リボン - [グラフ]タブ - [縦棒] - ![](pic/graphvertical.png) *集合縦棒* を選択します。

{% screenshot graph1.png "グラフの種類の選択" %}

グラフが作成されました。このまま使ってもあまり支障はありませんが、項目名が見辛くなってしまっているので、変更していきましょう。

{% screenshot graph2.png "グラフデータの初期選択範囲" %}

{% screenshot graph2a.png "グラフの初期状態" %}

&#9312; まず、編集したいグラフをクリックしてアクティブにしておきます。"グラフツール"がリボンに出てきました。

&#9313; 次に、"グラフツール" - [デザイン]リボン - [データ]タブ - [データの選択]をクリックします。

{% screenshot graph3.png "グラフデータの選択（ポップヒント：データの選択）" %}

&#9314; "データ ソースの選択"ウィンドウが表示されました。

{% screenshot graph4.png "データソースの選択" %}

&#9315; 次に、項目名を変えてみましょう。"人口(単位万人) 男女計" をクリックしてアクティブにしておき、"凡例項目（系列）" - [編集]をクリックします。"系列の編集"ウィンドウが表示されました。

{% screenshot graph5.png "系列の編集" %}

&#9316; "系列名"の `=Sheet1!$B$2:$B$3` を `=Sheet1!$B$3` に変更してみましょう。これで、`人口(単位万人) 男女計` となっていたのが `男女計` に直りました。

&#9317; 同様に"人口(単位万人) 男"と"人口(単位万人) 女"の系列も変更しておきましょう。

&#9318; 次に、横軸ラベルの範囲を確認します。横軸の編集は"横（項目）軸ラベル" - [編集]をクリックします。

{% screenshot graph6.png "軸ラベルの編集" %}

&#9319; "軸ラベルの範囲"が `=Sheet1!$A$4:$A$12` となっています。今回は変更する必要がありません。

{% screenshot graph7.png "軸ラベルの範囲（参照）" %}

{% screenshot graph7a.png "軸ラベル確認後" %}

これで、グラフの設定が一通り終わりました。
また、Excelでは自動的にグラフの設定を行ってくれるので、それに合わせた表作りをすれば、さらに簡単に終わらせることもできます。

どのような表作りが適切なのか、考えてみてもよいでしょう。

### グラフの編集

これまでは、データから単純にグラフを作るところまでを扱ってきました。
実際には、さらに見やすくするための加工が必要になってきます。

#### プリセットの視覚スタイルの利用

Excelにはプリセットで使用できる視覚スタイルが数多く用意されています。

&#9312; まず、"グラフツール" - [デザイン]リボン - [グラフのスタイル]タブの ![](pic/other.png) *その他* をクリックします。

{% screenshot graphdesign1.png "その他のグラフデザイン" %}

&#9313; 次に、好みの視覚スタイルを選び、クリックしてみてください。グラフがプリセットの視覚スタイルに変更されます。

{% screenshot graphdesign2.png "その他のグラフデザイン：詳細" %}

#### グラフタイトルや軸ラベルの挿入

グラフを見ただけで内容がわかるようにするためには、タイトルや軸ラベルなどの説明が欠かせません。今回はこれらを追加していきましょう。

&#9312; まず、グラフタイトルを追加します。
"グラフツール" - [デザイン]リボン - [グラフの要素を追加]タブ - [グラフタイトル]をクリックしてください。この教材では[グラフの上]を選択しています。

{% screenshot graphtitle1.png "グラフタイトルの挿入" %}

&#9313; グラフタイトルが挿入されました。グラフタイトルをクリックすると、グラフタイトルを編集することができます。

{% screenshot graphtitle2.png "グラフタイトル挿入例" %}

&#9314; 次に軸ラベルを入力してみましょう。
"グラフツール" - [デザイン]リボン - [グラフ要素を追加]タブ - [軸ラベル]をクリックしてください。ここで各軸ラベルを設定できます。

&#9315; まずは[第１横軸ラベル]をクリックして横軸にラベルを付けます。

{% screenshot graphlabel1.png "横軸へのラベル挿入" %}

&#9316; 横軸にラベルが挿入されました。グラフタイトルと同様にクリックすると、ラベルを編集することができます。

{% screenshot graphlabel2.png "横軸ラベルの挿入例" %}

&#9317; 次に[第１縦軸ラベル]をクリックして縦軸にラベルを付けます。

{% screenshot graphlabel3.png "縦軸へのラベルの挿入" %}

&#9318; 縦軸にラベルが挿入されました。こちらも同様にクリックすると、ラベルを編集することができます。

{% screenshot graphlabel4.png "縦軸ラベルの挿入例" %}

#### 誤差範囲の設定

データには誤差がつきものですが、この誤差範囲もグラフに表示することができます。

&#9312; まず、"グラフツール" - [デザイン]リボン - [グラフの要素を追加]タブ - [誤差範囲]をクリックします。

{% screenshot grapherror1.png "誤差範囲を選択" %}

&#9313; 後は、適用したい方式の誤差範囲をクリックすると、誤差範囲が表示されます。

{% screenshot grapherror2.png "例：標準偏差" %}

#### グラフの書式設定

グラフの書式は、基本的に"グラフツール" - [書式]リボン - [現在の選択範囲]タブ - [選択対象の書式設定]で変更することができます。

&#9312; まず、"グラフツール" - [書式]リボン - [現在の選択範囲]タブのプルダウンメニューを、変更したいものに変えます。（変更したいところをクリックしても変わります。）

{% screenshot graphdesign3.png "グラフの書式" %}

&#9313; 次に、"グラフツール" - [書式]リボン - [現在の選択範囲]タブ -[選択対象の書式設定]をクリックします。

{% screenshot graphdesign4.png "書式設定を選択" %}

&#9314; 出てきた"書式設定"メニューには、選択対象に合わせた書式設定の項目が表示されます。

{% screenshot graphdesign5.png "書式設定メニュー" %}

主な例としては以下のようなものです。

<dl>
<dt>系列のオプション</dt>
<dd>系列同士の重なりや、要素の間隔、第二軸の使用などが設定できます。</dd>
<dt>凡例のオプション</dt>
<dd>凡例の位置などを設定できます。</dd>
<dt>軸のオプション</dt>
<dd>目盛間隔や交点の処理、ラベルの位置など、軸に関しての設定ができます。</dd>
<dt>表示形式</dt>
<dd>目盛やラベルなどの表示の仕方を設定します。基本的にはセルの表示形式と同じように設定できます。</dd>
<dt>配置</dt>
<dd>軸のラベルなどの配置を設定することができます。</dd>
<dt>縦軸（横軸）誤差範囲</dt>
<dd>縦軸（横軸）の誤差範囲の表示方式を設定します。</dd>
<dt>塗りつぶし</dt>
<dd>選択対象の背景色などを設定することができます。</dd>
<dt>枠線の色</dt>
<dd>選択対象の枠線の色を設定します。</dd>
<dt>枠線のスタイル</dt>
<dd>選択対象の枠線の線種や角を丸めるなどをすることができます。</dd>
<dt>影</dt>
<dd>選択対象に影をつけることができます。これによって視覚的に背景からうまく分離することが可能です。</dd>
<dt>3-D 書式</dt>
<dd>選択対象を三次元的に傾けたり、光源や質感を変更することで視覚的な効果を生むことができます。</dd>
</dl>

これらの書式設定を組み合わせて駆使すれば様々なグラフを作ることができます。色々なものを試して、より見やすいグラフ作成を目指しましょう。

{% screenshot graphdesign.png "グラフの完成例" %}

#### グラフの種類変更

グラフを選択し、[挿入]リボン - [グラフ]タブを用いてグラフの種類を変えます。

#### グラフの消去

グラフを選択して[Delete]キー、あるいは[ホーム]リボン - [編集]タブの ![](pic/clear.png) *クリア* の[すべてクリア]をクリックして消去します。

### グラフの種類

Excelで作成できるグラフには、棒グラフ（ヒストグラム）のほかにもさまざまな種類があり、扱うデータによって使い分けることができます。

まず、以下のような表を作成しましょう。合計数量と合計金額には数式を入れて求めてみましょう。わからなかったら前回の [数式処理](../01/index.html) を見直しましょう。

{% screenshot graphtype.png "サンプルデータ" %}

#### 折れ線グラフ

複数の系列のデータを比較するときに便利です。
ここでは、曜日別の売り上げ変化を表しています。

{% screenshot graphtype1.png "折れ線グラフの場合" %}

#### 円グラフ

全体に対する割合を示すときによく使われます。
ここでは、合計売り上げ金額の割合を表しています。

{% screenshot graphtype2.png "円グラフの場合" %}

#### レーダーグラフ

構成要素の偏りなどを見るときに便利な図です。

{% screenshot graphtype3.png "レーダーグラフの場合" %}


第2軸を用いた複合グラフの作成
---------------------------------

これまで作成したグラフは、x軸とy軸のスケールが一つずつでしたが、異なる二つのy軸を持つグラフを作ることもできます。

ここでは、降水量と気温のグラフ（雨温図）を作ります。

&#9312; まず、以下の表を作成します。

{% screenshot graphtype5.png "気温と降水量のデータ" %}

&#9313; 次に、グラフを作成したい領域を選択し、棒グラフを作ります。

&#9314; 次に、グラフの気温の項目を選択（グラフ内の気温系列の棒要素をクリック）し、[挿入]リボン - [グラフ]タブ - [折れ線]の中の任意の折れ線を選びます。

{% screenshot graphtype6.png "グラフの種類の選択" %}

&#9315; さらに、気温の項目を選択したまま、"グラフツール" - [書式]リボン - [現在の選択範囲]タブ - [選択対象の書式設定]をクリックします。

選択対象 `系列"平均気温"` を選択します。

{% screenshot graphtype7.png "平均気温を選択" %}

&#9316; [系列のオプション]の中の"使用する軸"を[第2軸]にします。

{% screenshot graphtype8.png "第2軸を設定" %}

これで第2軸を設定することができました。

{% screenshot graphtype9.png "第2軸追加状態" %}

グラフが作成されたら、これまでと同じように編集を加えましょう。

{% screenshot graphtypefin.png "グラフの完成例" %}


Excelの表・図のWord文書への貼りつけ(ペースト)
---------------------------------------------

今後レポートを提出する際など、Excelで作成した図や表を、Wordにコピーしたいと思うことが多くなると予想されます。
ここで簡単にExcelの図、表のコピーとWordへのペーストについて確認しましょう。

### 表のコピー＆ペースト

&#9312; 図表を貼り付けたいWordファイルを開く、あるいは新規作成します。

&#9313; Excelを起動し、表を作成します。罫線も入れ、最終的な形にしておくことが望ましいです。（ただし、罫線やデータの配置などはWordからも編集できる）

&#9314; Excelにて対象表部分をドラッグして選択し、[ホーム]リボン - [クリップボード]タブの ![](pic/copy.png) *コピー* を選択します。あるいはショートカットキー（Windowsであれば[Ctrl]+[C]）を利用します。

{% screenshot copy1.png "" %}

&#9315; Wordの画面を表示させます。挿入したい位置にカーソルを置き、[ホーム]リボン - [クリップボード]タブの ![](pic/paste.png) をクリックします。あるいはショートカットキー（Windowsであれば[Ctrl]+[V]）を使います。

{% screenshot copy2.png "" %}

&#9316; Excelの表がペーストされました。必要であれば、貼り付けた際に出てくる ![](pic/paste2.png) をクリックして、貼り付ける形式を変更します。

{% screenshot copy3.png "" %}

### 図のコピー・ペースト

&#9312; Excelにてグラフ・図を作成します。図はExcelですべて最後の最後まで仕上げておくのが望ましいです。

&#9313; 先の表と同じように選択してコピーします。

&#9314; Wordに移ります。先の表と同様に貼り付けます。

&#9315; Excelのグラフがペーストされました。必要であれば、貼り付けた際に出てくる ![](pic/paste2.png) をクリックして、貼り付ける形式を変更します。

{% screenshot copy4.png "" %}

なお、外部のExcelファイルとワード内に貼り付けたグラフをリンクさせることもできるので、Excel内の数字を変えて試してみましょう。


その他の機能
------------

今までに紹介した以外にも、Excelには様々な機能があります。余裕がある人は挑戦してみましょう。

