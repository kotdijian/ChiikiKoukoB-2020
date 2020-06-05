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
    * リストは自治体ごとを基本とするが、一部分割している  
    * .csv形式 (UTF-8, BOMなし)  
    * ファイル名の上5ケタは[自治体コード](https://www.soumu.go.jp/denshijiti/code.html)  
    * 内容：東京都遺跡地図所収8項目（遺跡番号、ふりがな、遺跡名、所在地、時代、種別、主な遺構／概要、主な出土品）+自治体コード+JASID  
    * JASID(Japan Archaeological Site ID: 10ケタ)＝自治体コード(5ケタ)+遺跡番号(自治体ごと:3ケタ)+枝番号(2ケタ、枝番ナシは00)
    * ファイル名に"_coord"がついているものは位置座標、ただし手動で与えられた代表点でありシェープではない。内容はJASID+緯度経度  
    * 位置座標の正確性は保証されない  
    * ファイル名に"_ref"がついているものは書誌情報。JASID+「[全国遺跡報告総覧](https://sitereports.nabunken.go.jp/ja)」ID (or [NCID](https://www.nii.ac.jp/nels/man/descript/item_list.html))  

## Contributing／コントリビューション
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.  
プルリクエスト歓迎。大規模な変更はイシューからどうぞ。  

## Contributors／協力者  
* 13109_Shinagawa-ku／品川区：[@ta-niiyan](https://twitter.com/ta_niiyan)  
* 13112_Setagaya-ku08／世田谷区8, 13214_Komae-shi／狛江市, 13210_Koganei-shi／小金井市：Atsushi Noguchi ([kotodijian](https://github.com/kotdijian) or [@fujimicho](https://twitter.com/fujimicho)  
