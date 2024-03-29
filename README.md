
# 近代短歌データベースのリポジトリ
[近代短歌データベース](http://kindaitankadatabase.com/)に関するデータを掲載しています。

データの利用に際しては、[上記サイト](http://kindaitankadatabase.com/)の「データの利用について」をご参照ください。  



## テキストデータの構成について
- データベースに収録しているテキストデータは、短歌本文に加え、歌人, 歌集, 制作年, 出版年をメタデータとして付与しています。  
- 制作年、出版年の記録方法にはいくつか種類があります。詳しくは下記データ例および、[上記サイト](http://kindaitankadatabase.com/)「制作年と出版年について」をご参照ください。



| データ例 | 制作年・出版年について |
| :--- | :--- | 
| A|霜ふりて一もと立てる株の木の林はあはれに黑ずみにけり,斎藤茂吉,赤光,1905,1913 | 制作年、出版年が判明 |
| B|その昔しまだ乙女子の姉君と若菜つみけんかつしかの里,斎藤茂吉,短歌拾遺,1905,\[1905\] | 制作年が1905年と判明、未刊行（歌集未収録歌）のため出版年は制作年を補記 |
| C|その子二十櫛にながるる黑髮のおごりの春のうつくしきかな,与謝野晶子,みだれ髪,0000,1901 | 制作年が不明のため「0000」、 出版年は判明 |
| D|生きてわれ聽かむ響かみ棺を深くをさめて土落す時,窪田空穂,まひる野,1899-1905,1905 | 制作年が1897年から1901の間と判明、出版年も判明 |



## リポジトリのデータについて
**itiji.txt**

- 検索システムSolrに登録している異体字対応表です。[デジタル版渋沢栄一伝記資料　新旧文字置換対照表](https://eiichi.shibusawa.or.jp/denkishiryo/digital/main/index.php?kanji)をもとにデータを作成しています。

**底本.csv** 

- テキストデータの底本情報について記載しています。

**歌集制作年・出版年.csv**

- 歌集ごとの制作年、出版年について記載しています。 「○」はグラフ集計対象外の歌集、 「●」はグラフ集計、年数検索いずれも対象外の歌集をであることを表しています。
- 「制作年を補記」は「[yyyy]」の形式で制作年を補記している歌集を表しています。
- **凡例**

| 記録例 | 年数検索 | グラフ集計 |説明|対応するデータ例|
| :--- | :--- | :--- |:--- |:--- |
| yyyy-yyyy | 対象 | 対象 |特定の年で制作年/出版年が判明（実際のメタデータにはyyyyの形で記録）|A|
| 制作年を補記 | 対象 | 対象 |草稿等、歌集未刊行の場合に出版年を補記|B|
| ●0000 | 対象外 | 対象外 |制作年/出版年が不明|C|
| ○yyyy-yyyy| 対象 | 対象外 |範囲で制作年/出版年が判明|D|
