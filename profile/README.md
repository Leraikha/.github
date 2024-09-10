# Leraikha
悪魔的能力と移動性能を誇るプレイヤーによる、完全個人戦弓PvPゲーム。  

## 元ネタ
レライハ（Leraikha）とは悪魔学における悪魔の一人。  
レラージェ（Leraje）レライエ（Leraie,Leraye）、ロレイ（Loray）、オライ（Oray）とも呼ばれる。  
『ゴエティア』によると、30の軍団を率いる序列14番の地獄の大侯爵。  
『大奥義書』によると、サルガタナスの配下にあるという。  
召喚者の前に、弓矢を手にし、緑色の服を着た狩人の姿で現れる。  
戦いと論争を引き起こし、矢によって傷を治癒することができ、敵には壊疽傷を与えることが出来るとされる。  
十二宮の射手座に属するともいわれる。

## ゲームの進行
1. エントリールームへ転送
2. アリーナ中央超上空へテレポート
3. パーティクルと共に視点方向斜め下に常にモーション付与
4. 着地時点で弓とプロテクターを配布
5. ゲームスタート
6. 残り二人になったらタイマンのため中央へテレポート

## プロテクター（鎧）
- [x] 鉄のプロテクター（鎧）は矢を受けると鎖のプロテクター（鎧）に変化する
- [x] 鎖のプロテクター（鎧）は矢を受けると破壊される
- [x] プロテクター（鎧）を攻撃するたびに経験値がたまり、マックスになるとプロテクター（鎧）にエンチャントがつく
- [x] 一回のヒットにつき0.25の経験値分が付与され、4回当てることで経験値バーがマックスになる
- [x] エンチャントのついたプロテクター（鎧）は矢を喰らうとエンチャントが消える
- [x] エンチャントは回復によるプロテクター（鎧）強化に繰り越されない

## 特殊仕様
- [x] ドロップするキー入力でスロット8のアイテムを持ち替えなしで使用できる
- [x] オフハンドとスワップするキー入力でスロット9のアイテムを持ち替えなしで使用できる
- [x] 回復ポーションのみドロップできる
- [x] 矢が頭に当たると対象に盲目が付与される

## キャラコン
- [x] Wall Bounce
- [ ] Air Strafe
- [x] Climb Dash
- [x] Climb Air Curve
- [x] Chain Lift

## アビリティ
- [x] リニアーピーク（直線高速突撃）
  - [x] 砂糖
  - [x] パーティクルを発生させる
  - [x] 視点方向への高速移動
  - [x] クールタイム90秒
- [x] シャドウステップ（影化移動）
  - [x] 火薬
  - [x] パーティクルを発生させながら動く
  - [x] 無敵透明になる
  - [x] 移動速度が上昇する
  - [x] 発動遅延1秒 
  - [x] 効果継続時間8秒
  - [x] クールタイム90秒
- [ ] ジーニアスアイ（全能の眼）
  - [ ] グロウストーンダスト
  - [ ] 最短距離の対象を自分からのみ発光させる
  - [ ] 効果継続時間8秒
  - [ ] クールタイム90秒

## 特殊アイテム
- [ ] 回復のポーション
  - [x] プロテクター（鎧）を一段階上位の物へ回復させる
  - [ ] 初動で2つ所持

## オリジナルイベント
これらのイベントは内部の処理を行った後にイベントとして発火させ、外側のサウンドやパーティクルといった装飾のコードをそれぞれのイベントで実装するためのもの。  
[ProtectorEventAdapterListener](https://github.com/Leraikha/Core/blob/master/src/main/kotlin/mc/leraikha/core/listener/ProtectorEventAdapterListener.kt)は内部の処理。  
[ProtectorEventListener](https://github.com/Leraikha/Core/blob/master/src/main/kotlin/mc/leraikha/core/listener/ProtectorEventListener.kt)は外側の処理。  
- [x] ProtectorEvent
  - [x] ProtectorBreakEvent
  - [x] ProtectorEnchantedEvent
  - [x] ProtectorSetEvent
  - [x] ProtectorRecoveryEvent
- [x] GameEvent
  - [x] GameStartEvent
  - [x] GameEndEvent
  - [x] GameEntryStartEvent
  - [x] GameEntryEndEvent

## データベース
#### player
|論理カラム名|物理カラム名|型|PK|FK|NN|UK|AI|DEF|備考|
|---|---|---|---|---|---|---|---|---|---|
|ID|id|INTEGER UNSIGNED|〇||||〇|||
|UUID|uuid|CHAR(32)|||〇|〇||||
|プレイ時間|play_times|DATETIME|||〇|||||
|作成日|created_at|DATETIME|||〇|||CURRENT_TIMESTAMP||

...
