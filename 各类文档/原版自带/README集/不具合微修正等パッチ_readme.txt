﻿-------------------------------------------------------------------------------------------

-era紅魔館protoNTR用 不具合微修正等パッチ-


簡単なパッチの説明
スレ814
	3)本来寝ている筈の時間に自慰をするキャラが出る(条件は不明だが起床を午前6時にするとおき易いかも？)
	4)訪問者によって納屋等に連れ込まれて犯されている最中でも自慰の為に自室に戻る
	6)パンチラ等でぱんつを確認した後も？下着？になる、押し倒して確認してもうふふ終了後に？下着？に
	7)ノーパンだと？下着？すらないからはいてない事が即わかる
	
	↑これらを解消し
	
	5)自慰の最中を覗いたり写真に撮ったりCCDカメラで撮影しても普段通り
	
	↑の覗き部分を少し追加するパッチ
	
導入手順
	"era紅魔館protoNTR Ver.0.009"に"era紅魔館protoNTR修正パッチ140110"を適用した後に
	このパッチを入れてください
	
追加フラグ
	CFLAG
	388,ぱんつ確認
		  
		  
ファイルの変更・追加・削除一覧
	CLOTHES.ERB
		130行目あたり
			はんつ確認フラグリセット
	COMF404.ERB
		103行目あたりから
			自慰覗きイベント追加
		194,237行目あたり
			はんつ確認フラグセット
	INFO_STATE.ERB
		51行目あたり
			下半身下着が見える状態ならフラグ取得
		1138行目あたり
			分岐変更
	MOVEMENT.ERB
		1082行目
			睡眠時に自慰中フラグリセット
		1265行目
			睡眠判定
	PRINT_STATE.ERB
		130行目あたり
			分岐変更
		635行目
			分岐追加

		
14/01/11 UP

-------------------------------------------------------------------------------------------


不具合解消情報

3)
	睡眠時に自慰中フラグをリセットし、自慰条件に睡眠判定を追加
4)
	自慰判定に訪問者との接触判定を追加、接触していると自慰をしなくなる
6)
	ぱんつ確認用のフラグを追加、覗きなどで一度ぱんつを視ると穿きかえるまでの間表示されるように
7)
	表示方法を変更

これで大丈夫なはず

5)
	自慰覗きイベントの処理を追加
	イベント上の地の文や追加ソースは後々拡張する

