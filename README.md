**コマンド集**
---
**【minecraft.gamer-iris.com】**<br>
![ワールド選択画面](world-selection-menu-page.png)<br>
Java版：minecraft.gamer-iris.com<br>
統合版：be.minecraft.gamer-iris.com<br>
<details><summary>サーバーコントロール操作</summary>

- サーバー1移動<br>
    ```
    /server server1
    ```
- サーバー2移動<br>
    ```
    /server server2
    ```
- 時間変更<br>
    ```
    /time set day
    ```
- 天気変更<br>
    ```
    /weather clear
    ```
- ゲームモード変更<br>
    ```
    /gamemode survival @p
    /gamemode creative @p
    /gamemode spectator @p
    ```
- ホワイトリスト操作<br>
    - ホワイトリスト有効化（サーバーの再起動要）<br>
        ```
        /whitelist on
        ```
    - ホワイトリスト無効化（サーバーの再起動要）<br>
        ```
        /whitelist off
        ```
    - ホワイトリスト取得<br>
        ```
        /whitelist list
        ```
    - プレイヤー追加<br>
        ```
        /whitelist add プレイヤー名
        ```
    - プレイヤー削除<br>
        ```
        /whitelist remove プレイヤー名
        ```
    - リロード<br>
        ```
        /whitelist reload
        ```
- BAN操作<br>
    - BANリスト取得<br>
        ```
        /banlist
        ```
    - プレイヤー追加<br>
        ```
        /ban-ip プレイヤー名 理由
        ```
    - プレイヤー削除<br>
        ```
        /pardon-ip プレイヤー名
        ```
- <a href="https://www.spigotmc.org/resources/coreprotect.8631/">CoreProtect</a>操作<br>
    - ログ調査コマンド<br>
        ```
        /co inspect
        ```
    - ログ詳細調査コマンド<br>
        ```
        /co lookup <パラメーター>
        ```
    - ロールバックコマンド<br>
        ```
        /co rollback <パラメーター>
        ```
    - 各パラメータ内容<br>
        ```
        action:<行動>
          ∟action:block - ブロックの破壊 / 設置
          ∟action:＋block - ブロックの設置
          ∟action:－block - ブロックの破壊
          ∟action:container - チェストやかまどなどへのアイテムを追加 / 取る
          ∟action:＋container - チェストやかまどなどへのアイテムの追加
          ∟action:－container - チェストやかまどからアイテムを取る
          ∟action:item - アイテムの取得 / ドロップ等
          ∟action:＋item - アイテムの取得
          ∟action:－item - アイテムのドロップ等
          ∟action:inventory - インベントリへのアイテムの追加 / 取り出し
          ∟action:＋inventory - インベントリへのアイテムの追加
          ∟action:－inventory - インベントリからのアイテムの取り出し
          ∟action:session - サーバーへの参加 / 退出
          ∟action:＋session - サーバーへの参加
          ∟action:－session - サーバーの退出
          ∟action:chat - チャット
          ∟action:command - コマンド
          ∟action:kill - エンティティの殺害
          ∟action:sign - 看板への記入
          ∟action:username - ユーザーネームの変更
          ∟action:click - ドアやボタンなどの操作
        block:<ブロック / エンティティ>
        exclude:<ブロック / アイテム / エンティティ / ユーザー>
        include:<ブロック / エンティティ>
        radius:<範囲 or ワールド>
        time:<時間>
        user:<ユーザーネーム>
        ```
- <a href="https://github.com/Gamer-Iris/Linux/releases">Greetmate</a>操作<br>
    - greetbanコマンド<br>
        ```
        /greetban プレイヤー名 BAN理由
        ```
    - greetroleコマンド<br>
        ```
        /greetrole set プレイヤー名 ロール番号
        /greetrole register プレイヤー名 ロール番号
        /greetrole del プレイヤー名 ロール番号
        ```
    - greetunbanコマンド<br>
        ```
        /greetunban プレイヤー名
        ```
- <a href="https://www.spigotmc.org/resources/plugmanx.88135/">PlugManX</a>操作<br>
    - プラグイン有効コマンド<br>
        ```
        /plugman enable プラグイン名
        ```
    - プラグイン無効コマンド<br>
        ```
        /plugman disable プラグイン名
        ```
    - プラグインリロードコマンド<br>
        ```
        /plugman reload プラグイン名
        ```
</details>
<details><summary><a href="https://minecraft-blog.net/?s=%E3%82%A8%E3%83%B3%E3%83%81%E3%83%A3%E3%83%B3%E3%83%88%E3%82%B3%E3%83%9E%E3%83%B3%E3%83%89">装備一式取得</a>操作</summary>

- ネザライトの剣<br>
    |エンチャント①|エンチャント②|エンチャント③|エンチャント④|エンチャント⑤|エンチャント⑥|
    |:---:|:---:|:---:|:---:|:---:|:---:|
    |アンデッド特効（5）|ノックバック（1）|火属性（2）|ドロップ増加（3）|範囲ダメージ増加（3）|修繕（1）|
    ```
    /minecraft:give @p netherite_sword[enchantments={levels:{smite:5,knockback:1,fire_aspect:2,looting:3,sweeping_edge:3,mending:1}}]
    ```
- 弓<br>
    |エンチャント①|エンチャント②|エンチャント③|エンチャント④|
    |:---:|:---:|:---:|:---:|
    |耐久力（3）|射撃ダメージ増加（5）|フレイム（1）|無限（1）|
    ```
    /minecraft:give @p bow[enchantments={levels:{unbreaking:3,power:5,flame:1,infinity:1}}]
    ```
- メイス<br>
    |エンチャント①|エンチャント②|エンチャント③|エンチャント④|
    |:---:|:---:|:---:|:---:|
    |耐久力（3）|修繕（1）|重撃（5）|ウィンドバースト（3）|
    ```
    /minecraft:give @p mace[enchantments={levels:{unbreaking:3,mending:1,density:5,wind_burst:3}}]
    ```
- 盾<br>
    |エンチャント①|エンチャント②|
    |:---:|:---:|
    |耐久力（3）|修繕（1）|
    ```
    /minecraft:give @p shield[enchantments={levels:{unbreaking:3,mending:1}}]
    ```
- ネザライトのヘルメット<br>
    |エンチャント①|エンチャント②|エンチャント③|エンチャント④|エンチャント⑤|
    |:---:|:---:|:---:|:---:|:---:|
    |ダメージ軽減（4）|水中呼吸（3）|水中採掘（1）|耐久力（3）|修繕（1）|
    ```
    /minecraft:give @p netherite_helmet[enchantments={levels:{protection:4,respiration:3,aqua_affinity:1,unbreaking:3,mending:1}}]
    ```
- ネザライトのチェストプレート<br>
    |エンチャント①|エンチャント②|エンチャント③|
    |:---:|:---:|:---:|
    |ダメージ軽減（4）|耐久力（3）|修繕（1）|
    ```
    /minecraft:give @p netherite_chestplate[enchantments={levels:{protection:4,unbreaking:3,mending:1}}]
    ```
- ネザライトのレギンス<br>
    |エンチャント①|エンチャント②|エンチャント③|
    |:---:|:---:|:---:|
    |ダメージ軽減（4）|耐久力（3）|修繕（1）|
    ```
    /minecraft:give @p netherite_leggings[enchantments={levels:{protection:4,unbreaking:3,mending:1}}]
    ```
- ネザライトのブーツ<br>
    |エンチャント①|エンチャント②|エンチャント③|エンチャント④|エンチャント⑤|
    |:---:|:---:|:---:|:---:|:---:|
    |ダメージ軽減（4）|落下耐性（4）|水中歩行（3）|耐久力（3）|修繕（1）|
    ```
    /minecraft:give @p netherite_boots[enchantments={levels:{protection:4,feather_falling:4,depth_strider:3,unbreaking:3,mending:1}}]
    ```
- エリトラ<br>
    |エンチャント①|エンチャント②|
    |:---:|:---:|
    |耐久力（3）|修繕（1）|
    ```
    /minecraft:give @p elytra[enchantments={levels:{unbreaking:3,mending:1}}]
    ```
- ネザライトのツルハシ①<br>
    |エンチャント①|エンチャント②|エンチャント③|エンチャント④|
    |:---:|:---:|:---:|:---:|
    |効率強化（5）|シルクタッチ（1）|耐久力（3）|修繕（1）|
    ```
    /minecraft:give @p netherite_pickaxe[enchantments={levels:{efficiency:5,silk_touch:1,unbreaking:3,mending:1}}]
    ```
- ネザライトのツルハシ②<br>
    |エンチャント①|エンチャント②|エンチャント③|エンチャント④|
    |:---:|:---:|:---:|:---:|
    |効率強化（5）|耐久力（3）|幸運（3）|修繕（1）|
    ```
    /minecraft:give @p netherite_pickaxe[enchantments={levels:{efficiency:5,unbreaking:3,fortune:3,mending:1}}]
    ```
- ネザライトのシャベル<br>
    |エンチャント①|エンチャント②|エンチャント③|
    |:---:|:---:|:---:|
    |効率強化（5）|耐久力（3）|修繕（1）|
    ```
    /minecraft:give @p netherite_shovel[enchantments={levels:{efficiency:5,unbreaking:3,mending:1}}]
    ```
- ネザライトの斧<br>
    |エンチャント①|エンチャント②|エンチャント③|エンチャント④|
    |:---:|:---:|:---:|:---:|
    |ダメージ増加（5）|効率強化（5）|耐久力（3）|修繕（1）|
    ```
    /minecraft:give @p netherite_axe[enchantments={levels:{sharpness:5,efficiency:5,unbreaking:3,mending:1}}]
    ```
- ネザライトのクワ<br>
    |エンチャント①|エンチャント②|エンチャント③|エンチャント④|
    |:---:|:---:|:---:|:---:|
    |効率強化（5）|耐久力（3）|幸運（3）|修繕（1）|
    ```
    /minecraft:give @p netherite_hoe[enchantments={levels:{efficiency:5,unbreaking:3,fortune:3,mending:1}}]
    ```
</details>
<details><summary>環境設定操作</summary>

- <a href="https://luckperms.net/">LuckPerms</a>操作<br>
    - 権限追加
        ```
        /lp editor
        ゲーム内で生成されたURLを開く
        以下を設定
        +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
        （グループ_サーバー所有者）
        greetmate.command.*
        plugmanx.*
        （グループ_default）
        bungeecord.command.server
        multiverse.portal.access.*
        +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
        ```
- <a href="https://dev.bukkit.org/projects/multiverse-core/">Multiverse</a>操作<br>
    - ワールド作成
        ```
        /mv list
        /mv create resource normal
        /mv create resource_nether nether
        /mv create resource_the_end the_end
        /mv create spawn normal -t flat
        サーバー停止
        バックアップの「X.XX.X」「X.XX.X_nether」「X.XX.X_the_end」「resource」「resource_nether」「resource_the_end」「spawn」から「XXXXX-world.yml」を除き、復元を実行
        バックアップの「plugins」から各プラグインフォルダの復元を実行
        サーバー起動
        /mv list
        /mv tp resource
        /mv tp resource_nether
        /mv tp resource_the_end
        /mv tp spawn
        /mv tp バージョン番号
        /mv tp バージョン番号_nether
        /mv tp バージョン番号_the_end
        /mvnp link nether resource resource_nether
        /mvnp link nether resource_nether resource
        /mvnp link end resource resource_the_end
        /mvnp link end resource_the_end resource
        /mvinv group
        edit
        default
        Worlds
        以下を追加
        +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
        resource
        resource_nether
        resource_the_end
        +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
        @
        ##
        ```
    - ワールド編集
        ```
        【spawnワールドで作業】
        /mv modify set difficulty peaceful
        /mv modify set animals false
        /mv modify set monsters false
        /mv modify set hunger false
        /mv modify set gameMode adventure
        /mv modify set bed-respawn false
        /mv modify set allowflight false
        /mv setspawn
        /setworldspawn

        【resourceワールドで作業】
        /mv modify set bed-respawn true
        /mv modify set pvp false
        /mv modify set respawn-world resource
        /mv setspawn

        【resource_netherワールドで作業】
        /mv modify set bed-respawn false
        /mv modify set pvp false
        /mv modify set respawn-world resource

        【resource_the_endワールドで作業】
        /mv modify set bed-respawn false
        /mv modify set pvp false
        /mv modify set respawn-world resource

        【X.XX.Xワールドで作業】
        /mv modify set bed-respawn true
        /mv modify set respawn-world X.XX.X
        /mv setspawn

        【X.XX.X_netherワールドで作業】
        /mv modify set bed-respawn false
        /mv modify set respawn-world X.XX.X

        【X.XX.X_the_endワールドで作業】
        /mv modify set bed-respawn false
        /mv modify set respawn-world X.XX.X
        ```
    - ポータル設定
        ```
        【spawnワールドで作業】
        //wand
        ポータルの範囲を決める
        /mvpc spawn-original
        /mvpc spawn-resource

        【originalワールドで作業】
        //wand
        ポータルの範囲を決める
        /mvpc original-spawn（任意のポータル名）
        /mvps spawn-original
        /mvpm dest p:original-spawn
        /mvps original-spawn
        /mvpm dest p:spawn-original

        【resourceワールドで作業】
        //wand
        ポータルの範囲を決める
        /mvpc resource-spawn（任意のポータル名）
        /mvps spawn-resource
        /mvpm dest p:resource-spawn
        /mvps resource-spawn
        /mvpm dest p:spawn-resource
        ```
- <a href="https://dev.bukkit.org/projects/worldguard/">WorldGuard</a>操作<br>
    - 地域保護
        ```
        【spawn、各original、各resourceワールドで作業】
        //wand
        保護したい範囲を決める
        /rg define リージョン名（任意のリージョン名）
        /rg addmember リージョン名 ユーザー名
        /rg flags リージョン名
        ```
- <a href="https://www.spigotmc.org/resources/chunky.81534/">Chunky</a>操作<br>
    - チャンク更新
        ```
        【spawn、各original、各resourceワールドで作業】
        /worldborder center ~ ~
        /worldborder set 5000 0
        /chunky worldborder チャンクを生成したいワールド
        /chunky start
        /chunky progress
        ```
- <a href="https://github.com/PlaceholderAPI/PlaceholderAPI">PlaceholderAPI</a>操作<br>
    - 変数設定
        ```
        /papi ecloud download player
        /papi ecloud download server
        /papi ecloud download Bungee
        /papi reload
        ```
</details>
