業務選択/ツール画面
===============

<img src="capture_work_page.png" width="256" />

業務選択
--------

* 配置されている巡目の点検データ一覧が表示されます。
  リンクをクリックすると、選択した巡目で[橋梁一覧画面](list_page.md)に遷移します。
* <img src="capture_work_empty_list.png" width="128" />
  まだ点検データを配置していない場合「リポジトリがありません。」と表示されます。
* <img src="capture_work_need_sync.png" width="128" />
  点検データがサーバに同期されていない巡目には「[同期してください]」と表示されます。

【注意】
現在、ステージングされた状態（PUSH失敗）と競合した状態を検出できません。
ステージングされていても点検は続行できますが、競合しているファイルはエラーとなり、点検が行えません。


ツール
------

これらツールは手操作では面倒な作業を補助する目的で提供しますが、あくまで簡易なツールです。

### 橋梁

[橋梁データの作成](../setup/make_bridge_data.md)で利用するリンクです。

* CSVヘッダダウンロード
* 変換（CSV → YAML） 


### データ

#### 点検データ同期

点検したローカルリポジトリ変更をコミットします。
（PULL→COMMIT→PUSH）

Git認証は認証情報付きのURLで行う前提です。
次項の「巡目リポジトリ配置」を使ってCLONEしていれば認証情報付きのURLが保存されるので気にしなくて良いです。

鍵認証も行えるはずですが未確認です。

#### 巡目リポジトリ配置

![配置](capture_work_clone.png)

* 巡目：
  * 何巡目のデータかを数値で指定します
* URL：
  * 点検データリポジトリのクローンURLを指定します
* ユーザID：
  * Git認証のユーザID（GitHubのログインユーザID）を指定します
* パスワード：
  * Git認証のパスワード（GitHubのログインパスワード）を指定します

【注意】ブランチを使った複数端末の運用はここからは行えません。
配置（CLONE）後、手操作でブランチを切り替えてください。