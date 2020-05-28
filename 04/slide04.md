name: inverse
layout: true
class: center, middle, inverse

---
# 考古学における地域研究 
地域考古学B-2020年度第4回目
2020/5/29
[授業ページトップに戻る](https://kotdijian.github.io/ChiikiKoukoB-2020/)

---
layout: false
###### 1
### 前回までの振り返り
* 考古学資料・情報を集める ＞ 文献一覧  
* 分布図作成の準備 ＞ 位置情報の収集  
* ひなたGISを使って分布図を作成しよう ＜ ここから  

--

### 事後学習課題の確認  
* 東京都遺跡地図からデータのコピペ・一覧化  
    **一覧表で提供してくれていたら便利ですよね?**  

--
### 今日のリソース
* **[Googleドキュメント第4回まとめ](https://drive.google.com/open?id=10ije2uWAW9R9Wv80i6-Mw48z9d_37dsCtuqcFpLB5sA)**  

---
###### 2
## 1.作成したリストを地図に表示してみよう  
* 作成したのはGoogleスプレッドシートです  
* ひなたGISに読み込めるのは.csv形式です  
    * .csv形式とは? ([ウィキペディア](

* 著作権法　（[Wikipedia「著作権法」](https://ja.wikipedia.org/wiki/%E8%91%97%E4%BD%9C%E6%A8%A9%E6%B3%95)）  
    * 複製権
    * 上演権・演奏研・上映権・口述権
    * 公衆送信権・送信可能化権
    * 翻訳権・翻案権
    * 展示権・頒布権・譲渡権・貸与権

* 著作者人格権：公表権+氏名表示権+同一性保持権
    
* 著作隣接権：実演・レコード製作・放送事業者  

---
###### 4
## 0.著作物の利用と著作権法（結）
* 次のものは著作物にあたるかどうか考えてみよう  
    * 発掘調査報告書  
--
    * 遺跡一覧表と遺跡地図  
--
    * 遺構や遺物の実測図  
--
    * レイアウトと照明を工夫した写真／俯瞰写真  

---
###### 4-2
## 著作権法35条の改正と令和2年度の特例(前回補足)  

* [文化庁　著作権](https://www.bunka.go.jp/seisaku/chosakuken/index.html)
    * [著作権法の一部を改正する法律 概要](https://www.bunka.go.jp/seisaku/chosakuken/hokaisei/h30_hokaisei/pdf/r1406693_01.pdf)

* [著作物の教育利用に関する関係者フォーラム](https://forum.sartras.or.jp/info/004/)
    * 「改正著作権法第３５条運用指針（令和２（2020）年度版）」を公表    
        * https://forum.sartras.or.jp/info/004/
        * https://forum.sartras.or.jp/wp-content/uploads/kongounyo.pdf
        * https://forum.sartras.or.jp/wp-content/uploads/unyoshishin2020.pdf

→ PDFコピーの配布は受講生に限定します  

---
###### 5
## 1.地域考古学研究のリソース1　文献リストの作成  
* 書誌情報とは?  
    * 管理するのは1冊の「本」?／タイトル・内容が同一の「書誌」?
    * 「文献リスト」はどっち?  
* 文献リストの書式・項目について  
    * [『考古学研究』](https://kokogakukenkyukai.jp/toukou.html)  
    * [『旧石器研究』](http://palaeolithic.jp/contribution.htm)  
    * [『文化財と自然科学』(PDF)](http://www.jssscp.org/files/journalsubmission.pdf)  

* しかし書誌の特定は難関 → 著者(名字)+刊行年の重複、記載のぶれ...  
* UID, URI, URL, DOI：「一意に」書誌を識別する情報  
---
###### 6
## 調べる対象はどれだけあるのか?
1. NDL Search：タイトル=考古学 AND 出版地=日本, データベース=国立国会図書館オンライン, 資料種別=本, 所蔵館=国立国会図書館 or 他機関  
2. CiNii Books, タイトル=考古学, 資料種別=図書・雑誌, 言語種別=日本語  

|年代|NDL Search|CiNii Books|増加率N|増加率C|
|:---------:|----:|----:---|--:|-----:|
|～1950|283|430|-----|---|
|1951～1960|148|167|---|---|
|1961～1970|186|250|125.7%|149.7%|
|1971～1980|408|537|219.4%|214.8%|
|1981～1990|631|820|154.7%|152.7%|
|1991～2000|951|1469|150.7%|179.1%|
|2001～2010|1696|1772|178.3%|120.6%|
|2011～2020|1308|1243|77.1%|70.1%|

---
###### 7
## 1.地域考古学研究のリソース2　文献資料検索の補足
* [UID](http://e-words.jp/w/UID.html)：Unique Identifier. ある対象をほかとは区別する一意の識別子  
* [URI](https://ja.wikipedia.org/wiki/Uniform_Resource_Identifier)：Uniform Resource Identifier. 統一資源識別子。  
* [URL](https://ja.wikipedia.org/wiki/Uniform_Resource_Locator)：Uniform Resource Locator. 統一資源位置指定子。ウェブ空間上の場所を既定する。  
* [DOI](https://ja.wikipedia.org/wiki/%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E3%82%AA%E3%83%96%E3%82%B8%E3%82%A7%E3%82%AF%E3%83%88%E8%AD%98%E5%88%A5%E5%AD%90)：Digital Object Identifier. ウェブ上のドキュメントの識別子。学術論文で多用される。  

* 例）[『デジタル技術による文化財情報の記録と利活用』](https://sitereports.nabunken.go.jp/ja/33189)  

* 機械可読(machine readable)と人間可読(human readable)  

---
###### 8
## 2.地域考古学研究のリソース2　地図サービス

**どんなウェブ地図を使ったことがありますか?**

--
* [Googleマップ](https://www.google.co.jp/maps/)／[Google Earth](https://www.google.co.jp/intl/ja/earth/)  
* [Googleマイマップ](https://www.google.co.jp/intl/ja/maps/about/mymaps/)  

* [Bingマップ](https://www.bing.com/maps)／[Yahoo!地図](https://map.yahoo.co.jp/)  

--

* [地理院地図](https://maps.gsi.go.jp/)／[地理院地図Globe](https://maps.gsi.go.jp/globe/index_globe.html)  

--

* [ひなたGIS](https://hgis.pref.miyazaki.lg.jp/hinata/) →あとでやります!!  

---
###### 9
## 3.地域考古学研究のリソース3　地理情報

**知ってますか?**
* [地質図Navi](https://gbank.gsj.jp/geonavi/)  

--

* [国土交通省GISホームページ](https://nlftp.mlit.go.jp/index.html)  

--

* [歴史的農業環境閲覧システム](https://habs.dc.affrc.go.jp/)  

---
###### 10
## 4.地域考古学研究のリソース4　考古学情報

**遺跡地図**
* [文化財保護法95条](https://elaws.e-gov.go.jp/search/elawsSearch/elaws_search/lsg0500/detail?lawId=325AC1000000214#384)  
>「国及び地方公共団体は、周知の埋蔵文化財包蔵地について、資料の整備その他その周知の徹底を図るために必要な措置の実施に努めなければならない。」  

* [東京都遺跡地図情報インターネット提供サービス](https://tokyo-iseki.metro.tokyo.lg.jp/)  
検索してみよう!!

* 【参考】[国土数値情報　都道府県指定文化財データ](https://nlftp.mlit.go.jp/ksj/gml/datalist/KsjTmplt-P32.html)  
    * 東京都は未整備・未公表  

---
###### 11
## 5.地域考古学研究のツール1　位置情報・空間情報を軸にまとめる
1. **考古学情報**：遺跡の位置、内容(時代・遺構・遺物の種類...)  

--

2. **地理情報**：地形・地質...  

--

3. **地図の上に、考古学情報と地理情報を重ねる。相互の関係を検討する...**
--
    1. 基礎地図の上に描画する：場所の確認  
--
    2. 地形や地物との関係を知る  
--
    3. その他の地理情報との関係を知る  

## 地域考古学研究の第一歩  
--
* **さらに高度な空間分析も、まずはここから**

---
###### 12
## 5.地域考古学研究のツール1　位置情報・空間情報を軸にまとめる
### GIS(地理情報システム)
* [ウィキペディア「地理情報システム」](https://ja.wikipedia.org/wiki/%E5%9C%B0%E7%90%86%E6%83%85%E5%A0%B1%E3%82%B7%E3%82%B9%E3%83%86%E3%83%A0)  

* [GISとは…](https://www.gsi.go.jp/GIS/whatisgis.html)  

* 質問：GIS使ったことありますか?  
    * ArcGIS  
    * QGIS  
    * カシミール3D  
    * その他  

---
###### 13
## 6. 地域考古学研究のツール2　web GISとは?
* 個別のPCにソフトウェアをインストールせず、サーバー上で実行される  
* ウェブブラウザだけで使える ⇔ インターネット接続は必要  

--

* ここでは「[ひなたGIS](https://hgis.pref.miyazaki.lg.jp/hinata/) 」を使います
    * GISの理解・導入に適している  
    * さまざまな地理情報を直観的に表示できる  
    * 自分で操作できる  

---
###### 14
## 6.実習：東京都遺跡地図を題材に
1. 区市町村ごとにリストを作る  


--
2. ひなたGISに読み込む  


--
3. 東京都遺跡地図を参考に位置を読み取る  


--
4. ひなたGISで位置座標の一覧を取得する  


--
5. 遺跡一覧に位置座標を加える  


--
6. 位置座標付きの一覧リストの完成!


---
###### 15
## 7. 事後学習課題

1. 東京都遺跡地図で担当の市域を検索、遺跡一覧を表示する  

2. 情報をコピーしGoogleスプレッドシートへペースト、行列を入れ替えて一覧表を作成  

3. ひなたGISを利用して、位置情報（緯度・経度）を取得する。  
    * 便利機能：Google Chrome→TabResize  

4. 分担はGoogleドキュメントのとおり  

5. 入力先はGoogleスプレッドシートにタブが作成していあります。  

---
###### 16
### 参考文献
* 奈良文化財研究所 2019 『デジタル技術による文化財情報の記録と利活用』奈良文化財研究所研究報告21 ([全国遺跡報告総覧](https://sitereports.nabunken.go.jp/ja/33189)／[奈文研リポジトリ](https://repository.nabunken.go.jp/dspace/handle/11177/6882)  

* 奈良文化財研究所 2020 『デジタル技術による文化財情報の記録と利活用2』奈良文化財研究所研究報告24 ([全国遺跡報告総覧](https://sitereports.nabunken.go.jp/ja/69974)／[奈文研リポジトリ](https://repository.nabunken.go.jp/dspace/handle/11177/6950))  

---
###### 17
## ご案内

**[3D写真計測ワークショップ](https://kotdijian.github.io/arch3dphotogrammetry/)をオンラインで開催します。興味のある方はどうぞ**

