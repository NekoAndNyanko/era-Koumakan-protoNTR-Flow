﻿-------------------------------------------------------------------------------------------

-era紅魔館protoNTR用妊娠処理等変更・修正パッチ++-


簡易説明
	妊娠関連の処理を一部追加、変更するパッチ
	
変更・追加内容
	●登録キャラの膣内射精時、コマンドにより子宮内に入る精子量が変動するようになる
	●子供のステータス表示にて名前の後ろに成長段階が表示される
	　表示されるのは成長期まで、それぞれ 赤子→幼児(幼女)→成長期 と表示される
	
	
	●排卵誘発剤及びピルの使用条件の追加
	　・妊娠している場合使用できない
	　・娘の場合、成長期まで成長している必要がある
	　　但し主人公が[禁断の知識]を取得している場合は例え赤子でも使用できる
	
	
導入手順
	"era紅魔館protoNTR Ver.0.006"に"era紅魔館protoNTR修正パッチ130909"を適用した後に
	このパッチを入れてください



	
改造を施した既存ファイル
PRINT_STATE.ERB
	14行目
		子供のステータス表示追加

SHOP_ITEM.ERB
	236,267行目
		排卵誘発剤及びピルの使用条件の追加
		
生理機能追加パッチ
	25行目あたり
		生理周期の処理の位置を少し変更
		
		
妊娠処理変更パッチ
	63行目あたり
		登録キャラの膣内射精時、コマンドによる精子量の変動追加
		コマンド[挿入子宮口責め]以外のＶ挿入コマンドでの射精の場合
		子宮内に入る精子の量が3割減少する
	242行目以降
		子供の成長状態表示の呼び出しを追加
		
		
2013/09/10 UP
	
	改造はご自由に
-------------------------------------------------------------------------------------------






表・コマンド別膣内射精における妊娠確率の違い

条件１ 射精される側の子宫内体积は5000
条件２ 射精する側の精力の初期値は1000
条件３ 膣内射精時のコマンドは全て同じ、例えば1回目が子宮口責めによる射精ならそれ以降も同じコマンドで膣内射精を行う
条件４ 射精される側は排卵日で、一日終了時に妊娠のチェックが入る

以上の条件で3回膣内射精をした際の精子量と妊娠確率が以下の通り

----------------
  コマンド  射精1回目  射精2回目  射精3回目  合計精子量  妊娠確率
子宮口責め       1000        842        676        2518    50％
  それ以外        700        599        504        1797    36％
----------------

妊娠確率は (子宮内の精子量/子宫内体积)
精力の減少量は次第によっては増減するので一つの目安として見てね


