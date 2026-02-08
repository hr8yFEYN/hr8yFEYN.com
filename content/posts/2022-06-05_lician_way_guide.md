---
title: リキアン・ウェイ (旅行情報 2022年4月)
date: '2022-06-05T16:32:25+09:00'
draft: true
show_key_image: false
description: トルコ南西部のフェティエからアンタルヤまで地中海沿い歩くリキアンウェイの旅行情報
taxonomies:
  tags:
  - 旅行
  - トルコ
  - リキアン･ウェイ
  - 旅行情報
extra:
  key_image: https://photos.hr8yfeyn.com/Lycian_Way_Signpost-320.jpg
  keywords:
  - 旅行
  - トルコ
  - リキアンウェイ
  - リキアン・ウェイ
  - 旅行情報
  toc: true
---

<a href="https://photos.hr8yfeyn.com/Lycian_Way_Signpost.jpg"><img src="https://photos.hr8yfeyn.com/Lycian_Way_Signpost-800.jpg" alt="リキアン・ウェイのサインポスト"></a>

<div style="margin: 1em 5% 3em 5%">
<em>
<p>
リキアン・ウェイを歩こうとはりきってトルコに来たのだけど、
全体の２/３を歩いたところで膝が痛くなってきたので早々に敗退した(フェティエ〜フィニケ)。
なので、そんなに詳しいことも書けないのだけど書ける範囲で書いた。
</p>

<p>
2022年4月に歩いた時の情報です。当時のレートは 1トルコ・リラ = 8.2円。
</p>
</em>
</div>


# 基本情報
リキアン・ウェイ(英語 Lycian Way, トルコ語 Likya Yolu)は、トルコ南西部のフェティエからアンタルヤまでを地中海沿いに[リュキア](https://ja.wikipedia.org/wiki/リュキア)の遺跡をめぐる全長500キロ以上のトレイル。

途中でリタイアしたので正確にはわからないけど、全ルートを歩くと20日ぐらいかかると思う。
初老のおじいちゃんが、20キロ以上のバックパックを背負ってフェティエからフィニケまで15日だったので、
健脚のひとなら20日もかからないと思う。

無料のリキアンウェイの公式(?)アプリがある([iPhone](https://apps.apple.com/jp/app/lycian-way-lite/id1463178442), [Android](https://play.google.com/store/apps/details?id=trekkinginturkey.cultureroutesinturkey.com))。
[Wikipeida](https://en.wikipedia.org/wiki/Lycian_Way)と[Wikivoyage](https://en.wikivoyage.org/wiki/Lycian_Way)にリキアンウェイの記事がある。
[OpenStreetMap](https://openstreetmap.org)にルートが載っている。
ルート上の遺跡、宿泊施設、レストラン、商店、テント適地、水場なども載っている。

Wikivoyageによると、安全対策としてはサソリがいるので靴を履く時に中にサソリがいないか確認、テントは開けっぱなしにしないということらしい。
だけど、ぼくは一度もサソリを見なかった。小さなヘビはよく見たけど。その他は、特に危険なことはないとのこと。


# 宿泊
基本的には、1日に歩ける範囲内にペンションやキャンプ場などがある。

ぼくはパトラとカシュでキャンプ場に泊まった他は、地図に載っているテント適地にテントを張っていたので、
ペンションがどんなものかわからないけど、
ひとから聞いた話だと食事が付いて200〜400リラぐらいらしい。

キャンプ場は50〜100リラで、シャワーとキッチンが使えてる。だいたいWiFiもある。
リゾート地だと200リラというところもあるらしい。

全ルートを歩く場合、ミラからフィニケまでは(2泊3日かかった)、途中に宿泊施設がないのでキャンプ道具が必要(Wikivoyageにそう書いてある)。

リキアン・ウェイでは、基本的にどこにテントを張ってもいいらしい。


# 食料・水
大きな町には当然スーパーなどがあり何でも買える。
小さな村や集落でもトレイル上に商店がある場所もあるが、
集落の商店は休むこともあるようなので、町で次の町までの最低限の食料は買っておいた方がいい。

ペンションやキャンプ場は軽食なども提供しているよう。

地図上に水場(井戸や貯水槽)があっても枯れていたり、
汚くて飲めないことも多いので(特に標高の低い海岸沿いなど)、
村や集落で、次の村や集落までの水を十分に補給した方がいい。

ストーブは、OD缶はトレイル上の町では手に入らないのでガソリン・ストーブがいい。
ぼくはのんびりキャンプがてらのハイキングのつもりだったので焚き火をした。
テント敵地にはだいたい焚き火の跡があった。

# ルート・地図
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/leaflet/1.7.1/leaflet.css" />
<script src="https://cdnjs.cloudflare.com/ajax/libs/leaflet/1.7.1/leaflet.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/leaflet-gpx/1.7.0/gpx.min.js"></script>
<div id="map" style="height:360px"></div>

<script>
var map = L.map('map');
L.tileLayer('http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
  attribution: 'Map data &copy; <a href="http://www.osm.org">OpenStreetMap</a>'
}).addTo(map);

var gpx = '/Lician_Way-OSM.gpx';
new L.GPX(gpx, {async: true, gpx_options: {joinTrackSegments: false}, marker_options: {startIconUrl: false, endIconUrl: false, shadowUrl: false}}).on('loaded', function(e) {
  map.fitBounds(e.target.getBounds());
}).addTo(map);
</script>

<span style="font-size:85%">
<a href="/Lician_Way-OSM.gpx">Lician_Way.gpx</a>
</span>


リキアン・ウェイのルート上には、赤と白のストライプで道標(Waymark, [写真](https://upload.wikimedia.org/wikipedia/commons/c/c8/Likya.yol.isareti.jpg))が付いている。
基本的にしっかり付いているのでそれほど迷うことはないが、町や村からトレイルに入るところが分かり難いことが多々あった。しばらく道標を見かけなかったら、あまり進んでしまう前に、最後に見た道標まで戻って道を間違っていないか確認した方がいい。

ルートの分かり難いところや、道標の間隔が長いところなどには、積み石がしてあったりする。

リキアン・ウェイ公式のアプリにも地図が載っているが、
地図の縮尺が大き過ぎて地図としては使えないと思う。

Maps.me([iPhone](https://apps.apple.com/jp/app/maps-me-offline-maps-gps-nav/id510623322), [Android](https://play.google.com/store/apps/details?id=com.mapswithme.maps.pro))のオフライン地図で十分そうだけど、道が入り組んでいるところは分かりにくそう。
歩いてる時にあった人たちは、Gaia GPS([iOS](https://apps.apple.com/jp/app/gaia-gps-mobile-trail-maps/id1201979492), [Android](https://play.google.com/store/apps/details?id=com.trailbehind.android.gaiagps.pro))というアプリを使っている人が多かった。
地図上にルートが引かれているので、Maps.meよりはよそうだった。
あと現在地からの距離の計算とかができて便利そうだった。
ただサブスクリプションで年20ユーロするらしい。


## フェティエ(Fethiye) 〜 オヴァジュク(Ovacık)
フェティエ〜オヴァジュクはリキアン・ウェイではないが、
フェティエから歩き始める人が多いよう。
Wikivoyageのガイドだと、フェティエのイェニ・ハミディイェ・モスク(Yeni Hamidiye Cami)からスタートになっている。

カラキョイには、商店、レストランがある。

カラキョイからオヴァジュクまでは、海岸沿いにオヴァジュクに行くルートと、
直接オヴァジュクまで行くルートがある。直接オヴァジュクに行くルートが公式らしい。


## オヴァジュク(Ovacık) 〜 ファラルヤ(Faralya) | 12.3km
- コザアチ(Kozağaç) : 水場、軽食あり
- キルメ(Kirme) : 宿や商店、食堂、水場があり
- ファラルヤ(Faralya) : 宿、商店、食堂、水場があり


## ファラルヤ(Faralya) 〜 カバック(Kabak) | 5.7km
途中、水場あり。

- カバック(Kabak) : 宿、商店、食堂、水場あり


## カバック(Kabak) 〜 アルンジャ(Alınca) | 6.9km
ビーチに下りない方のルートだと、途中に水場あり。細かったので時期によっては枯れるのかもしれない。

- アルンジャ(Alınca) : 宿、商店、食堂、水場あり


## アルンジャ(Alınca) 〜 ベル(Bel) | 13.9km
ゲルからベルに直接行くルートと、シディマ(Sidyma)を経由するサイド・トレイルがある。
遺跡があるというのでシディマ経由のルートを歩いたが、
あまり歩かれていないようだし、遺跡というほどのものもないので、
直接ベルに行くルートでよさそう。

アルンジャからゲルに向かう途中に、食堂、水場あり。

- ゲル(Gel) : 商店、食堂、水場あり
- ベル(Bel) : 宿、商店、食堂、水場あり


## ベル(Bel) 〜 ガヴラル(Gavurağlı) | 7.3km

- ガヴラル(Gavurağlı) : 宿、水場あり


## ガヴラル(Gavurağlı) 〜 クサントス(Xanthos) | 19.2km
ガフラルからパタラ・ビーチに向かう途中に水場あり。その先、レトン遺跡まで水場はない。
パタラ・ビーチからレトン遺跡までは道路を8キロ歩く。レトン遺跡、クサントス遺跡までバスに乗ることもできるよう。
レトン遺跡(8:00〜19:30 15リラ)の周辺にスーパー、商店あり。

クニックは比較的大きな町でスーパーや小さなバスターミナルもあるが宿泊施設はないとのこと。
Wikivoyageには政府が経営するゲストハウスがあると書いてあったので探せばあるのかもしれない。

- パタラ・ビーチ : 宿あり
- クニック(Kınık) : 商店、食堂あり


## クサントス(Xanthos) 〜 ユジムリュ(Üzümlü) | 14.0km
クサントスからチャブドゥル(Çavdır)までは道路を4キロ。
チャブドゥル(Çavdır)からユジムリュ(Üzümlü)の間は、水路の遺跡の上をを歩く区間がある。

- チャブドゥル(Çavdır) : 商店、スーパー、食堂、水場あり
- ユジムリュ(Üzümlü) : ペンション、食堂、商店、水場あり


## ユジムリュ(Üzümlü) 〜 パタラ(Patara) | 23.7km
アクベル(Akbel)からパタラ(Patara)までは、それほど登り下りのない道。
途中、水路の遺跡がある。パタラ遺跡(40リラ)。

- アクベル(Akbel) : 宿泊、商店、食堂、水場あり
- ゲレミシュ(Gelemiş) : 宿泊、商店、食堂、ATMあり


## パタラ(Patara) 〜 カルカン(Kalkan) | 19.0km
パタラからカルカンまで水場はない。

水路遺跡からカルカン(Kalkan)までは、
ぼくが歩いたルートでは1番険しい箇所だった。
それでも危険というほどではなかった。

- カルカン(Kalkan) : 宿泊、スーパー、食堂、ATMあり


## カルカン(Kalkan) 〜 サルベレン(Sarıbelen) | 14.0km
カルカン(Kalkan)からサルベレンまで登り。途中、井戸あり。

- サルベレン(Sarıbelen) : 宿泊、商店、水場あり


## サルベレン(Sarıbelen) 〜 ギョクチェオレン(Gökçeören) | 12.4km
サルベレンからギョクチェオレンまで水場なし。

- ギョクチェオレン(Gökçeören) : 軽食堂、水場あり


## ギョクチェオレン(Gökçeören) 〜 チュクルバ(Çukurbağ) | 20.7km
ギョクチェオレン(Gökçeören)からHacıoglan dersiまで8kmはなだらかな道。
フェロス遺跡(Phellos)までは登り。チュクルバ(Çukurbağ)までは下り。

チュクルバ(Çukurbağ) : 水場あり


## チュクルバ(Çukurbağ) 〜 カシュ(Kaş) | 7.0km
サインポストには、カシュ(Kaş)はAntiphellosと書かれている。

チュクルバ(Çukurbağ)からカシュ(Kaş)の手前3kmまでは平らな道。そこからカシュまで急な崖を下って行く。

- カシュ(Kaş) : 宿泊、レストラン、スーパー、ATMあり

## カシュ(Kaş) 〜 リマナズ(Limanağzı) | 4.2km
海岸沿いの平らな道。水場はない。

## リマン・アウズ(Liman Ağızı) 〜 ボアズジュック(Boğazcık) | 13.9km
ボアズジュックまで水場なし。

## ボアズジュック(Boğazcık) 〜 ユチャウズ(Üçağız) | 18.5km
ボアズジュックからすぐアポロニア遺跡がある。途中、アペルレア遺跡もある。

- ウチャウズ(Üçağız) : 宿泊、レストラン、商店あり


## ユチャウズ(Üçağız) 〜 カパクル(Kapaklı) | 8.9km
途中、シメナ遺跡(カレ Kale)あり。近くに水場もある。

## カパクル(Kapaklı) 〜 ミラ(Myra) | 12.0km
ここは新ルートがあるようだったが、ぼくはWikivoyageのルートで歩いていたので旧ルートで歩いた。
新ルートはカパクルからトリサ(Trysa)を通ってミラに行くらしい。

- デムレ(Demre) : 大きな町で宿泊、レストラン、ATM等なんでもある

## ミラ(Myra) 〜 フィニケ(Finike) | 38.2km
この区間には宿泊施設はない。商店、食堂もない。ミラからフィニケまで2泊3日程度かかる。
標高1,800メートル以上の地点を通る。リキアン・ウェイでのもっとも標高の高い地点らしい。
水場は枯れていたり、汚いところが多いので、補給できるところで十分に補給しておいた方がいい。

- フィニケ(Finike) : 大きな町でホテル、レストラン、ATM等なんでもある
