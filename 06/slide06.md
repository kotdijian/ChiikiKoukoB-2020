name: inverse
layout: true
class: center, middle, inverse

---
# 考古学における地域研究 
地域考古学B-2020年度第6回目
2020/6/12
[授業ページトップに戻る](https://kotdijian.github.io/ChiikiKoukoB-2020/)

---
layout: false
###### 1
### 前回の振り返り
* 「[ひなたGIS](https://hgis.pref.miyazaki.lg.jp/hinata/hinata.html)」を使って分布図を作成してみた  

--

### 今日のリソース

* [Googleドキュメント](https://docs.google.com/document/d/1lhbKmEWhqn5ZIRcdGRPH6uIPql74TKYhm1WztlqtN-8/edit?usp=sharing)  

---
###### 2
### 前回のおさらい：作成したデータをひなたGISで表示しよう  

* みなさんの入力データにもとづいて統合リストを作成しました  
    **☞ 13Tokyo_totalcoordSJS.csvを開いてみよう**  
    * データ量が大きく動作が重い場合は、ポイントを右クリック→ファイル→サーバーに保存  
    * うまく開けない人は[こちら](https://bit.ly/2MRgWYk) 
    * またはhttps://bit.ly/2MRgWYkを入力
    * gakugeidai.geojsonも開いてみよう

--

### 地理情報との重ね合わせ

* 「背景」から背景レイヤーを変更してみよう  
    * 地理院_単色地図  
    * 地理院_色別標高図  
    * 陰影図_地理院DEM10／同DEM5  
    * 立体図・地質・地形等フォルダ→日本CS立体図

---
###### 3
### 地図情報について  
1. ズームレベルについて  
    * 無段階に拡大縮小できるわけではない→ズームレベル
    * 参考：[国土地理院の既存の地図の体系と、地理院地図のズームレベル（縮尺）の関係](http://yamao.lolipop.jp/map/2017/gsi/hikaku.htm)  
    
2. DEMとは  
    * Digital Elevation Model：国土地理院「[DEM（数値標高モデル）](https://www.gsi.go.jp/KIDS/KIDS16.html)」  
    * DEMとDSM：国土地理院中部地方測量部「[第12回　航空レーザ測量について　その2](https://www.gsi.go.jp/chubu/minichishiki12.html)  

---
###### 4
### 地図情報について2  
3. タイル地図  
    * 連続する大きな地図をどのようにオンラインで表示するのか → タイル画像に分割（国土地理院「[地理院タイルについて](https://maps.gsi.go.jp/development/siyou.html)」）

4. ベクター（ベクトル）地図  
    * 道路や河川などの「線」のデータもタイルにするのか?
    * ☞ 地理院地図Vector（国土地理院「[国土地理院ベクトルタイル提供実験](https://maps.gsi.go.jp/development/vt_expt.html)」）
   

---
###### 4
### ひなたGISで多様な地理・地図情報と重ね合わせる  

* 地理院_地形分類（自然地形）：地形・条件により土地を分類したもの  

* 川だけ地形地図：河川流路と地形(DEM陰影図)  

* 川と流域地図：河川流路と流域(集水域：DEMから計算)　　

* 全国土壌図

* シームレス地質図v2：地質→地形と地層のなりたち・年代

* 迅速測図：都市開発以前の地図

---
###### 5
### その他のウェブ地図・ウェブGIS

* 地理院地図（国土地理院）→[こちら](https://bit.ly/3dVSNM7)／またはhttps://bit.ly/3dVSNM7  
    * 緯度・経度情報の入っている.csvファイルをドロップすると地図上にプロット  
    
    * 数値地図25000（土地条件）：地形  
    * 5万分の1地質図幅「東京西南部」「青梅」「八王子」 
    
* GoogleEarth（デスクトップ版／[ウェブ版](https://www.google.co.jp/intl/ja/earth/））
    * ウェブ版→3D地球儀  
    * デスクトップ版＝GoogleEarth Pro→GIS  

* [Googleマイマップ](https://www.google.co.jp/intl/ja/maps/about/mymaps/)  
    * Googleスプレッドシートとの連携  
    * データ読み込みは2000件まで 

---
###### 6
### 主題図を作成しよう  
* さて、いよいよ考古学的分析へ  

--

* いまのデータで何ができる?  

--

* もっと絞り込む・並べ替える必要?  

---
###### 7
### 遺跡情報データベース

* いまデータに入力されているもの
    1. (JASID)  
    2. (自治体コード)  
    3. 遺跡番号  
    4. ふりがな  
    5. 遺跡名  
    6. 所在地  
    7. 時代  
    8. 種別  
    9. 主な遺構/概要  
    10.主な出土品  
    11.経度  
    12.緯度  

---
###### 8
### 遺跡情報データベース

* 何をどのように利用したいのか?  

## ☞ 実習してみよう  

