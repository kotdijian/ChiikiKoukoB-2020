# .csv list of registered archaeological sites in Tokyo Metropolice／東京都遺跡地図リスト化データ
This is digitized lists of archaeological sites in Tokyo, based on [Tokyo Metropolitan government Internet map of archaeological sites (Japanese Only)](https://tokyo-iseki.metro.tokyo.lg.jp/), publsihed by Tokyo Metropolitan Board of Education.  
これは[東京都遺跡地図情報インターネット提供サービス](https://tokyo-iseki.metro.tokyo.lg.jp/)にもとづき、東京都の遺跡（埋蔵文化財包蔵地）の情報をリスト化したものです。  

## Usage／ご利用にあたって

This work has been initiated as a part of a class of "Regional Archaeological Studies B" offered at Tokyo Gakugei Univesity in 2020 Spring semester.   
    * The lists organized by each municiparity and some are sub-divided  
    * Format in .csv (UTF-8 without BOM)  
    * The first 5 digit number of each file name is the [Local Government Code](http://data.e-stat.go.jp/lodw/en/provdata/lodRegion)  
    * contents: 8items of Tokyo Metropolitan government Internet map of archaeological sites, such as: site ID (by each municipality); read-kana; site name; location(by street address); age/ period; type of site; major features; major artefacts, plus Local Government Code and JASID  
    * JASID (Japan Archaeological Site ID) is the original 10 digit UID composed of Local Government Code (5 digit)+ site ID (3 digit)+ sub-ID (2 digit, NA=00). 
    * The files ended with "_coord" are geo-coordinates, not by shape but by manually chosen representative point, referable with JASID  
    * Thus no guarantee of accuracy on these coordinates so far  
    * The files ended with "_ref" are reference info, by URL in [SORAN (Comprehensive Database of Archaeological Site Reports in Japan)](https://sitereports.nabunken.go.jp/en) (or NCID: reference ID organized by NII-Japan).  

東京学芸大学2020年度春学期開講「[地域考古学B](https://portal.u-gakugei.ac.jp/syllabus/)」(教育支援課程教育支援専攻文化遺産教育サブコース60737000)の一環として作成を開始しました。  

1. 基本データ  
* 13Tokyo_total.csv: 東京都遺跡地図収録8項目+JASID+自治体コード+位置座標(経度・緯度)  
* 13Tokyo_totalAge.csv: 東京都遺跡地図【時代】列の入力項目を01ベクトルに変換したもの、JASID+遺跡名+旧石器時代～近世+時代不明。変換コードは"JAS_DataManagementFor13Tokyo.Rmd"を参照  
* 13Tokyo_totalcoord.csv: "13_Tokyo_total.csv"から座標値欠損レコードを除去したもの  

2. ソースデータ(sourceサブディレクトリ)  
    * 入力・整形作業は自治体ごとを基本とするが、一部分割しておこなった  
    * 基本リストは.csv形式(UTF-8, BOMなし)  
    * ファイル名の上5ケタは[自治体コード](https://www.soumu.go.jp/denshijiti/code.html)  
    * 内容：東京都遺跡地図所収8項目（遺跡番号、ふりがな、遺跡名、所在地、時代、種別、主な遺構／概要、主な出土品）+自治体コード+JASID  
    * JASID(Japan Archaeological Site ID: 10ケタ)＝自治体コード(5ケタ)+遺跡番号(自治体ごと:3ケタ)+枝番号(2ケタ、枝番ナシは00)
    * ファイル名に"_coord"がついているものは位置座標、ただし手動で与えられた代表点でありシェープではない。内容はJASID+緯度経度  
    * 位置座標の正確性は保証されない  
    * ~ファイル名に"_ref"がついているものは書誌情報。JASID+「[全国遺跡報告総覧](https://sitereports.nabunken.go.jp/ja)」ID (or [NCID](https://www.nii.ac.jp/nels/man/descript/item_list.html))~ (未実装)  

3. 座標・遺跡情報統合リスト(byMunicipalityサブディレクトリ)  
    * 分割入力されたもの、および位置座標を自治体単位で統合。ファイル名自治体コード+自治体名に"_total"を付す  
    * 内容は"13Tokyo_total.csv"を自治体コードで分割したものと等価  
    * .csv形式(UTF-8, BOMなし)  
    * 検証と統合は"JAS_DataManagementFor13Tokyo.Rmd"による 
    * ただし位置座標の正確性は保証されない  

4. 時代別統合リスト(byAgeサブディレクトリ)
    * 各時代別の一覧リスト  
    * "13Tokyo_total.csv"を各時代=1(= TRUE)で分割したものと等価(=時代別リスト間で重複あり)  
    * "13Tokyo_total_"に各時代名を付す(palaeolithic, jomon, yayoi, kofun, nara, heian, medieval, earlymodern, unknown  
    

## Contributing／コントリビューション
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.  
プルリクエスト歓迎。大規模な変更はイシューからどうぞ。  

## Contributors／協力者  
* 13109_Shinagawa-ku／品川区, 13111_Ota-ku／大田区：[@ta-niiyan](https://twitter.com/ta_niiyan)  
* 13110_Meguro-ku／目黒区, 13112_Setagaya-ku08／世田谷区8, 13208_Akishima-shi／昭島市, 13210_Koganei-shi／小金井市, 13212_Hino-shi／日野市, 13214_Komae-shi／狛江市, 13218_Fussa-shi／福生市, 13223_Musashimurayama-shi／武蔵村山市, 13227_Hamura-shi／羽村市, 13303_Mizuho-machi／瑞穂町：Atsushi Noguchi ([kotodijian](https://github.com/kotdijian) or [@fujimicho](https://twitter.com/fujimicho)  
* 13101_Chiyod-ku／千代田区, 13103_Minato-ku／港区, 13104_Shinjuku-ku／新宿区, 13105_Bunkyo-ku／文京区, 13113_Shibuya-ku／渋谷区, 13114_Nakano-ku／中野区, 13115_Suginami-ku／杉並区, 13116_Toshima-ku／豊島区, 13205_Ome-shi／青梅市, 13228_Akiruno-shi／あきる野市, 13305_Hinode-machi／日の出町, 13307_Hinohara-mura／檜原村, 13308_Okutama-machi／奥多摩町：collaboration of [@ta-niiyan](https://twitter.com/ta_niiyan) and Atsushi Noguchi ([kotodijian](https://github.com/kotdijian) or [@fujimicho](https://twitter.com/fujimicho)  
