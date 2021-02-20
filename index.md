## hoi4MOD制作の巻

いやーね、hoi4のMOD制作することになったんよ。
なんのMODかっていうと日本に天皇の元帥を入れるMOD。いや～めんどくさいことこの上ない！！！！
ということで参考にして作った（参考元：https://detail.chiebukuro.yahoo.co.jp/qa/question_detail/q13179582663)
すげー分かりやすかったです。プログラミング経験pythonで電卓作ったくらいしかないし頭にも残ってなかったからできるかな～って思ってたんだが、普通にできたんだなぁ。
一応簡単に説明しよう。
ローカルファイルからhistory＞countries＞JAP - japan.txt をMODからコピーしてきて、その中の
<html>
<br>set_naval_oob = "JAP_1936_naval_legacy"
<br>から
<br>oob = "JAP_1939"　
<br>あたり？まで（俺もよくわかってない）に
	create_field_marshal = {
	name = "yosihito"

		picture = "taisyo.dds"

	traits = {trickster trait_engineer}

	skill = 5

	attack_skill = 3
		defense_skill = 5
		planning_skill = 3
		logistics_skill = 5
 <br> みたいなのを書く。（コピペもあり）
  <br>説明をしよう！
  
  	create_field_marshal = {
  
  	name = "名前"

	picture = "画像.dds"(ddsファイルで縦156横210)

	traits = {trickster trait_engineer} (しらん！)

	skill = 5 スキルレベル

	attack_skill = 3　攻撃力
		defense_skill = 5　守備力
		planning_skill = 3　計画力？
		logistics_skill = 5　しらん！
  
  みたいな感じ（）よくわからんからちゃんとしたMOD解説のところを見るんだな！！！
  
