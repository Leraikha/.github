# Leraikha
悪魔的能力と移動性能を誇る狩人による、完全個人戦弓PvPゲーム。  

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
2. 全員が準備完了になり次第5秒カウント開始
3. 透明化を付与
4. アリーナのランダム地点へテレポート
5. 初期アイテムを配布
6. プリセットからアビリティをセット
7. 10秒の透明化後に矢を配布
8. ゲームスタート 5分
9. 2分後に範囲を縮める 110から60へ
10. 4分後に範囲を縮める 60から30へ
11. 決着

#### デュエル -Duel- (1v1 ランク)
1. エントリールームへテレポート
2. 全員が準備完了になり次第5秒カウント開始
3. 透明化を付与
4. アリーナのチーム地点へテレポート
5. 初期アイテムを配布
6. プリセットからアビリティをセット
7. 10秒の透明化後に矢を配布
8. 範囲を縮める 110から60へ
9. ゲームスタート 3分
10. 2分後に範囲を縮める 60から30へ
11. 決着

#### ウォーズ -Wars- (チーム戦)
1. エントリールームへテレポート
2. 全員が準備完了になり次第5秒カウント開始
3. 透明化を付与
4. アリーナのチーム地点へテレポート
5. 初期アイテムを配布
6. プリセットからアビリティをセット
7. 10秒の透明化後に矢を配布
8. ゲームスタート 5分
9. 2分後に範囲を縮める 110から60へ
10. 4分後に範囲を縮める 60から30へ
11. 決着


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
- [x] 最終攻撃者が死ぬと、その人の最終攻撃者のフラグが外れる
- [x] 最終攻撃者のフラグは時間経過で消えない
- [x] 撃破されると所持してたハチミツ入り瓶のみドロップ。
- [x] 安地外ダメージはプロテクターを削る
- [x] 肉体に一発喰らうと消滅する（消滅原因: 壊疽）


## キャラコン
- [x] 壁蹴り
  - [x] 後方即跳ね
  - [x] 壁登り
- [x] 登り越え
  - [x] 屈折
- [x] 鎖リフト
  - [x] 鎖の当たり判定削除
  - [x] 離脱時の上向き慣性
  - [x] 離脱時の下向き慣性


## アビリティ
ソフトアビリティはスロット8に配置したアイテムにより発動が可能。  
ハードアビリティはスロット9に配置したアイテムにより発動が可能。  
各々で好きにカスタマイズさせ、両方同じものに設定することもできる。  
なお、そうした場合はクールダウンが共通する為に、リスキーなカスタムとなる。  

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


## 初動アイテム
- [x] ハチミツ入り瓶
  - [x] プロテクター（鎧）を一段階上位の物へ回復させる
  - [x] 初動で2つ
- [x] 鉄のプロテクター（鎧）
  - [x] 初動で1つ

## ランク
※イロレーティングシステムで実装予定
|名称|下限レート|上限レート|
|---|:---:|:---:|
|ZERO|0|999|
|ONE|1000|1999|
|TWO|2000|2999|
|THREE|3000|3999|
|FOUR|4000|4999|
|FIVE|5000|-|

## データベース
### マスタ
#### game_rank
|論理カラム名|物理カラム名|型|PK|FK|NN|UK|AI|DEF|備考|
|---|---|---|:---:|:---:|:---:|:---:|:---:|:---:|---|
|ID|id|INTEGER UNSIGNED|〇||||〇|||
|ランク名称|name|VARCHAR(8)|||〇|〇||||
|最小レート|minimum|INTEGER UNSIGNED|||〇|||||
|最大レート|maximum|INTEGER UNSIGNED||||||||

#### season
|論理カラム名|物理カラム名|型|PK|FK|NN|UK|AI|DEF|備考|
|---|---|---|:---:|:---:|:---:|:---:|:---:|:---:|---|
|ID|id|INTEGER UNSIGNED|〇||||〇|||
|シーズン名|name|VARCHAR(16)|||〇|〇||||

#### ability
|論理カラム名|物理カラム名|型|PK|FK|NN|UK|AI|DEF|備考|
|---|---|---|:---:|:---:|:---:|:---:|:---:|:---:|---|
|ID|id|INTEGER UNSIGNED|〇||||〇|||
|アビリティ名|name|VARCHAR(16)|||〇|〇||||

#### kill_particle
|論理カラム名|物理カラム名|型|PK|FK|NN|UK|AI|DEF|備考|
|---|---|---|:---:|:---:|:---:|:---:|:---:|:---:|---|
|ID|id|INTEGER UNSIGNED|〇||||〇|||
|キルパーティクル名|name|VARCHAR(16)|||〇|〇||||

#### emerge_particle
|論理カラム名|物理カラム名|型|PK|FK|NN|UK|AI|DEF|備考|
|---|---|---|:---:|:---:|:---:|:---:|:---:|:---:|---|
|ID|id|INTEGER UNSIGNED|〇||||〇|||
|出現パーティクル名|name|VARCHAR(16)|||〇|〇||||
|シーズン|season_id|INTEGER UNSIGNED||season.id|〇|||||

### トランザクション
#### player_account
|論理カラム名|物理カラム名|型|PK|FK|NN|UK|AI|DEF|備考|
|---|---|---|:---:|:---:|:---:|:---:|:---:|:---:|---|
|ID|id|INTEGER UNSIGNED|〇||||〇|||
|UUID|uuid|CHAR(36)|||〇|〇||||
|お金|karma|INTEGER UNSIGNED||||||0||
|プレイ時間|play_times|DOUBLE|||〇|||0.0||
|最終プレイ日時|last_play_at|DATETIME|||〇|||CURRENT_TIMESTAMP||
|作成日|created_at|DATETIME|||〇|||CURRENT_TIMESTAMP||

#### player_battle_record
|論理カラム名|物理カラム名|型|PK|FK|NN|UK|AI|DEF|備考|
|---|---|---|:---:|:---:|:---:|:---:|:---:|:---:|---|
|ID|id|INTEGER UNSIGNED|〇||||〇|||
|プレイヤー|player_id|INTEGER UNSIGNED||player_account.id|〇|||||
|シーズン|season_id|INTEGER UNSIGNED||season.id|〇|||||
|ランク|rank_id|INTEGER UNSIGNED||game_rank.id|〇|||||
|レート|rating|INTEGER UNSIGNED|||〇|||0||
|プレイ数|play_count|INTEGER UNSIGNED|||〇|||0||
|勝利数|win_count|INTEGER UNSIGNED|||〇|||0||
|キル数|kill_count|INTEGER UNSIGNED|||〇|||0||
|デス数|death_count|INTEGER UNSIGNED|||〇|||0||
|ヒット数|hit_count|INTEGER UNSIGNED|||〇|||0||
|ショット数|shot_count|INTEGER UNSIGNED|||〇|||0||
|ヘッドショット数|headshot_count|INTEGER UNSIGNED|||〇|||0||
|プロテクター破壊回数|break_count|INTEGER UNSIGNED|||〇|||0||
|プロテクター回復回数|recovery_count|INTEGER UNSIGNED|||〇|||0||
|プロテクター強化回数|enchanted_count|INTEGER UNSIGNED|||〇|||0||
|最長射撃距離|longest_shot_distance|DOUBLE|||〇|||0.0||

#### player_game_settings
|論理カラム名|物理カラム名|型|PK|FK|NN|UK|AI|DEF|備考|
|---|---|---|:---:|:---:|:---:|:---:|:---:|:---:|---|
|ID|id|INTEGER UNSIGNED|〇||||〇|||
|プレイヤー|player_id|INTEGER UNSIGNED||player_account.id|〇|〇||||
|ソフトアビリティ|soft_ability_id|INTEGER UNSIGNED||ability.id||||NULL||
|ハードアビリティ|hard_ability_id|INTEGER UNSIGNED||ability.id||||NULL||
|キルパーティクル|kill_particle_id|INTEGER UNSIGNED||kill_particle.id||||NULL||
|出現パーティクル|emerge_particle_id|INTEGER UNSIGNED||emerge_particle.id||||NULL||

#### player_kill_particle
|論理カラム名|物理カラム名|型|PK|FK|NN|UK|AI|DEF|備考|
|---|---|---|:---:|:---:|:---:|:---:|:---:|:---:|---|
|ID|id|INTEGER UNSIGNED|〇||||〇|||
|プレイヤー|player_id|INTEGER UNSIGNED||player_account.id|〇|||||
|キルパーティクル|kill_particle_id|INTEGER UNSIGNED||kill_particle.id|〇|||||
|獲得日|created_at|DATETIME|||〇|||CURRENT_TIMESTAMP||

#### player_emerge_particle
|論理カラム名|物理カラム名|型|PK|FK|NN|UK|AI|DEF|備考|
|---|---|---|:---:|:---:|:---:|:---:|:---:|:---:|---|
|ID|id|INTEGER UNSIGNED|〇||||〇|||
|プレイヤー|player_id|INTEGER UNSIGNED||player_account.id|〇|||||
|出現パーティクル|emerge_particle_id|INTEGER UNSIGNED||emerge_particle.id|〇|||||
|獲得日|created_at|DATETIME|||〇|||CURRENT_TIMESTAMP||

#### player_ability
|論理カラム名|物理カラム名|型|PK|FK|NN|UK|AI|DEF|備考|
|---|---|---|:---:|:---:|:---:|:---:|:---:|:---:|---|
|ID|id|INTEGER UNSIGNED|〇||||〇|||
|プレイヤー|player_id|INTEGER UNSIGNED||player_account.id|〇|||||
|アビリティ|ability_id|INTEGER UNSIGNED||ability.id|〇|||||
|ソフトアビリティとして使った回数|count_as_soft_ability|INTEGER UNSIGNED|||〇||0||
|ハードアビリティとして使った回数|count_as_hard_ability|INTEGER UNSIGNED|||〇||0||
|獲得日|created_at|DATETIME|||〇|||CURRENT_TIMESTAMP||

...
