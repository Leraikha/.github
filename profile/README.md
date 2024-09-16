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
#### カジュアル -Casual-（多人数戦）
1. エントリールームへテレポート
2. アリーナのランダム地点へテレポート
3. 弓とプロテクターを配布
4. プリセットからアビリティをセット
5. ゲームスタート
#### デュエル -Duel- (1v1 ランク)
1. エントリールームへテレポート
2. アリーナのチーム地点へテレポート
3. 弓とプロテクターを配布
4. プリセットからアビリティをセット
5. ゲームスタート
#### ウォーズ -Wars- (チーム戦)
1. エントリールームへテレポート
2. アリーナのチーム地点へテレポート
3. 弓とプロテクターを配布
4. プリセットからアビリティをセット
5. ゲームスタート


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
- [x] ハチミツ入り瓶のみドロップできる
- [x] 矢が頭に当たると対象に盲目が付与される
- [ ] 最終攻撃者が死ぬと、その人の最終攻撃者のフラグが外れる
- [ ] 最終攻撃者のフラグは時間経過で消えない


## キャラコン
- [x] Wall Bounce
- [ ] Air Strafe
- [x] Climb Dash
- [x] Climb Air Curve
- [x] Chain Lift


## アビリティ
- [x] 迅疾 ジンシツ
  - [x] ソフトアビリティ『直進』
    - [x] 二次元空間での直線的な高速移動をする
    - [x] クールタイム20秒
  - [x] ハードアビリティ『飛進』
    - [x] 三次元空間での直線的な高速移動をする
    - [x] クールタイム90秒
- [x] 幽影 ユウエイ
  - [x] ソフトアビリティ『陰遁』
    - [x] 瞬時に陰をまとって1秒の無敵状態を得る
    - [x] クールタイム20秒
  - [x] ハードアビリティ『影遁』
    - [x] 影に変化し透明化高速撤退の能力を得る
    - [x] クールタイム90秒
- [x] 天眼 テンガン
  - [x] ソフトアビリティ『洞察の瞳』
    - [x] 半径10ブロックの敵1体を4秒間表示させる
    - [x] クールタイム20秒
  - [x] ハードアビリティ『真実の瞳』
    - [x] 半径20ブロックの全ての敵を8秒間表示させる
    - [x] クールタイム90秒


## 特殊アイテム
- [ ] ハチミツ入り瓶
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
### マスタ
#### rank
|論理カラム名|物理カラム名|型|PK|FK|NN|UK|AI|DEF|備考|
|---|---|---|:---:|:---:|:---:|:---:|:---:|:---:|---|
|ID|id|INT UNSIGNED|〇||-|-|〇|||
|名前|name|CHAR(16)||||||||
|下限レート|lower_rate|INT UNSIGNED|||〇|||||

### トランザクション

#### player_account
|論理カラム名|物理カラム名|型|PK|FK|NN|UK|AI|DEF|備考|
|---|---|---|:---:|:---:|:---:|:---:|:---:|:---:|---|
|ID|id|INT UNSIGNED|〇||-|-|〇|||
|UUID|uuid|CHAR(32)|||〇|〇||||
|Discord|discord|VARCHAR(32)||||||NULL||
|お金|karma|INT UNSIGNED||||||0||
|タグマーク|tag_prefix|VARCHAR(32)||||||NULL|[VIP]みたいな|
|プレイ時間|play_times|DATETIME|||〇|||||
|最終プレイ日|last_login|DATETIME|||〇|||CURRENT_TIMESTAMP||
|作成日|created_at|DATETIME|||〇|||CURRENT_TIMESTAMP||

#### player_battle_record
|論理カラム名|物理カラム名|型|PK|FK|NN|UK|AI|DEF|備考|
|---|---|---|:---:|:---:|:---:|:---:|:---:|:---:|---|
|ID|id|INT UNSIGNED|〇||-|-|〇|||
|レート|rate|INT UNSIGNED||||||1500||
|プレイ数|play_count|INT UNSIGNED||||||0||
|キル数|kill_count|INT UNSIGNED||||||0||
|デス数|death_count|INT UNSIGNED||||||0||
|ヘッドショット数|head_shot_count|INT UNSIGNED||||||0||
|プロテクター破壊回数|break_count|INT UNSIGNED||||||0||
|プロテクター回復回数|recovery_count|INT UNSIGNED||||||0||
|プロテクター強化回数|enchanted_count|INT UNSIGNED||||||0||
|最長射撃距離|longest_shot_distance|DOUBLE||||||0.0||

#### player_ability_validation
|論理カラム名|物理カラム名|型|PK|FK|NN|UK|AI|DEF|備考|
|---|---|---|:---:|:---:|:---:|:---:|:---:|:---:|---|
|ID|id|INT UNSIGNED|〇||-|-|〇|||
|アビリティ|ability_name|BOOL||||〇||FALSE||

#### player_ability_pick
|論理カラム名|物理カラム名|型|PK|FK|NN|UK|AI|DEF|備考|
|---|---|---|:---:|:---:|:---:|:---:|:---:|:---:|---|
|ID|id|INT UNSIGNED|〇||-|-|〇|||
|アビリティ|ability_name|INT UNSIGNED||||〇||0||

...
