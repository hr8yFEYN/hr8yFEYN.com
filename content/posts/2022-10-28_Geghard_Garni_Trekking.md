---
title: ゲガルド修道院からガルニ神殿までトレッキング
date: '2022-10-28T20:39:26+09:00'
draft: true
show_key_image: false
toc: false
taxonomies:
  tags:
  - 旅行
  - 旅行情報
  - アルメニア
  - トレッキング
extra:
  key_image: https://photos.hr8yfeyn.com/Geghard_Genri_01-320.jpg
---

<a href="https://photos.hr8yfeyn.com/Geghard_Genri_01.jpg"><img src="https://photos.hr8yfeyn.com/Geghard_Genri_01-800.jpg" alt="ガルニ渓谷"></a>

ガルニ神殿とゲガルド修道院を見学するには、バスでゴグト(終点)まで行き、そこから3キロ程度歩いて、
ゲガルド修道院を見学して、またゴグトに戻り、バスでガルニ神殿まで行くのが定番らしいが、
[OpenStreetMap](https://openstreetmap.org)を見ていたらゲガルド修道院からガルニ神殿までトレッキングできそうな道がついていたので、ゲルガド修道院からガルニ神殿まで歩いてきた。
途中、Havuts Tar寺院(日本語だとどう書くのか調べてもわからなかった)によれる。
GPSでトラックログを取らなかったので、
というか時計すらよく見ていなかったので正確にはわからないけど、
ゲガルド寺院からガルニ渓谷までで3時間ぐらいだった。

<link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.2/dist/leaflet.css"
     integrity="sha256-sA+zWATbFveLLNqWO2gtiw3HL/lh1giY/Inf1BJ0z14="
     crossorigin=""/>
<script src="https://unpkg.com/leaflet@1.9.2/dist/leaflet.js"
     integrity="sha256-o9N1jGDZrf5tS+Ft4gbIK7mYMipq9lqpVJ91xHSyKhg="
     crossorigin=""></script>
<div id="map" style="height:360px"></div>
<script>
var map = L.map('map').setView([40.1251, 44.7635], 13);
L.tileLayer('http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
  attribution: 'Map data &copy; <a href="http://www.osm.org">OpenStreetMap</a>'
}).addTo(map);
var icon01 = L.icon({iconUrl: '/images/maps/marker_red_01.png', iconSize: [16, 16], iconAnchor: [8, 8]});
var mrk01 = L.marker([40.13944,44.81796], {icon: icon01}).addTo(map).bindPopup("ゲガルド修道院");
var icon02 = L.icon({iconUrl: '/images/maps/marker_red_02.png', iconSize: [16, 16], iconAnchor: [8, 8]});
var mrk02 = L.marker([40.14071, 44.80345], {icon: icon02}).addTo(map).bindPopup("下り口");
var icon03 = L.icon({iconUrl: '/images/maps/marker_red_03.png', iconSize: [16, 16], iconAnchor: [8, 8]});
var mrk03 = L.marker([40.13877, 44.79955], {icon: icon03}).addTo(map).bindPopup("鉄塔");
var icon04 = L.icon({iconUrl: '/images/maps/marker_red_04.png', iconSize: [16, 16], iconAnchor: [8, 8]});
var mrk04 = L.marker([40.12321, 44.76929], {icon: icon04}).addTo(map).bindPopup("Havuts Tar修道院");
var icon05 = L.icon({iconUrl: '/images/maps/marker_red_05.png', iconSize: [16, 16], iconAnchor: [8, 8]});
var mrk05 = L.marker([40.11447, 44.74023], {icon: icon05}).addTo(map).bindPopup("ガルニ渓谷");
var icon06 = L.icon({iconUrl: '/images/maps/marker_red_06.png', iconSize: [16, 16], iconAnchor: [8, 8]});
var mrk06 = L.marker([40.11288, 44.73002], {icon: icon06}).addTo(map).bindPopup("ガルニ神殿");
</script>

<ol style="background-color:rgb(245,245,245);font-size:95%">
<li>ゲガルド修道院</li>
<li>渓谷への下り口</li>
<li>鉄塔(これを目指して道路から下る)</li>
<li>Havuts Tar修道院</li>
<li>ガルニ渓谷(シンフォニー・オブ・ストーン)</li>
<li>ガルニ神殿</li>
</ol>


ゲガルド修道院までは、エレバンのガイ・バスステーション(Gai Bus Station)から266番のバスでゴグト(45分程度)まで行き、そこから3キロ程度あるく。
バスの料金は500ドラム。最近、値上がったらしい(2022年10月)。

----

<a href="https://photos.hr8yfeyn.com/Geghard_Genri_02.jpg"><img src="https://photos.hr8yfeyn.com/Geghard_Genri_02-800.jpg" alt="渓谷への下り口"></a>
ゲガルド寺院からガルニ方面に15分程度行ったところから地図によると渓谷に下りられそうな道がいくつかあるのだけど、
どの道も私道のようで門がしてあって下りられない。木に登って赤い実をとっているおじさんがいたので聞くと木から下りてきて、まず赤い実と胡桃を左右のポケットにいっぱいくれてから、下り口まで案内してくれた。いわれないと、まず気がつかなさそうな道。フェンスを右にして、鉄塔まで下っていけとのことなので、急斜面だなと思いながら下っていく。

下り口がわからなくても、多少急勾配だけど鉄塔を目指して下っていけば道に出れる。

<a href="https://photos.hr8yfeyn.com/Geghard_Genri_03.jpg"><img src="https://photos.hr8yfeyn.com/Geghard_Genri_03-800.jpg" alt="赤い実と胡桃"></a>
送電線の鉄塔まで来ると、ロシア製の小さいジープが通れるぐらいの道になる。朝食も食べてないし、昼食も買い忘れたので、おじさんにもらった赤い実と胡桃を食べながら歩く。赤い実はなにやら心臓にいいらしい。

<a href="https://photos.hr8yfeyn.com/Geghard_Genri_04.jpg"><img src="https://photos.hr8yfeyn.com/Geghard_Genri_04-800.jpg" alt="ガルニ渓谷の川"></a>
しばらく歩いて川にでる。川を渡らないで真っ直ぐ行ってもガルニに行くのだけど、Havuts Tar修道院を見たいので川を渡る。渡るのだけど、橋などがないので靴を脱いで渡渉かなと思ったが、少し下流にいくと石の上を渡っていけそうな場所があった。

<a href="https://photos.hr8yfeyn.com/Geghard_Genri_05.jpg"><img src="https://photos.hr8yfeyn.com/Geghard_Genri_05-800.jpg" alt="ガルニ渓谷"></a>
川を渡ってしばらく歩くと開けた場所にでる。牛や馬が放牧されていた。

<a href="https://photos.hr8yfeyn.com/Geghard_Genri_06.jpg"><img src="https://photos.hr8yfeyn.com/Geghard_Genri_06-800.jpg" alt="ガルニ渓谷"></a>
200メートルばかりの登り。危険な箇所はないが、このあたりから道が細くなるので注意。

<a href="https://photos.hr8yfeyn.com/Geghard_Genri_07.jpg"><img src="https://photos.hr8yfeyn.com/Geghard_Genri_07-800.jpg" alt="ガルニ渓谷"></a>
しばらく歩くと、Havuts Tar修道院が見え始める。

<a href="https://photos.hr8yfeyn.com/Geghard_Genri_08.jpg"><img src="https://photos.hr8yfeyn.com/Geghard_Genri_08-800.jpg" alt="Havuts Tar修道院"></a>
Havuts Tar修道院。ゲガルド修道院から1時間半ぐらいだったと思う。

<a href="https://photos.hr8yfeyn.com/Geghard_Genri_09.jpg"><img src="https://photos.hr8yfeyn.com/Geghard_Genri_09-800.jpg" alt="ガルニ渓谷"></a>
Havuts Tar修道院からガルニ神殿が見える。1時間ぐらいで行けそうだ。Havuts Tar修道院からは車も通れる道。

<a href="https://photos.hr8yfeyn.com/Geghard_Genri_10.jpg"><img src="https://photos.hr8yfeyn.com/Geghard_Genri_10-800.jpg" alt="ガルニ渓谷"></a>
ガルニ神殿に近づくと、ガルニ渓谷の「シンフォニー・オブ・ストーンズ」が見えてくる。写真では、うまいこと撮っているから秘境みたいな場所にあるのかと思ったけど、遠くから見るとすぐ近くに大きな道路も走っているし、崖の上には民家もあるし視点が違うと印象も違う。

<a href="https://photos.hr8yfeyn.com/Geghard_Genri_11.jpg"><img src="https://photos.hr8yfeyn.com/Geghard_Genri_11-800.jpg" alt="シンフォニー・オブ・ストーンズ遠望"></a>
ガルニ渓谷見学。すごいなあとは思うものの、見ていたらぼくは少し気持ち悪くなった。しかしどういう現象があるとこんなさけるチーズみたいになるのだろう。いやカニカマか。

<a href="https://photos.hr8yfeyn.com/Geghard_Genri_12.jpg"><img src="https://photos.hr8yfeyn.com/Geghard_Genri_12-800.jpg" alt="シンフォニー・オブ・ストーンズ"></a>
それからしばらく歩いてガルニ神殿。

----

もう10月も終わりだけど、日中はまだ暖かい。
標高2,000メートル以下なら、11月いっぱいは歩けるかな。
