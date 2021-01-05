巡目リポジトリの作成
====================

簡単に説明すると、以下の3ステップです。

1. GitHubアカウントの作成（最初の一回）
1. 新規リポジトリの作成
1. 橋一覧データのコミット


GitHubアカウントの作成（最初の一回）
------------------------------------

点検データは[Git](https://git-scm.com/)で管理します。
[GitHub](https://github.com/)アカウントを作成してください。

開発・確認はGitHubにて行っており、ドキュメントもGitHub利用を前提として書いています。
他のGit（サービス）でも動作すると思われますが、未確認です。


### SSH公開鍵の登録
KyoRyoJoeインストール後、SSH公開鍵を登録してください。
鍵は[ツール/SSH公開鍵確認](../operation/work_page.md#SSH公開鍵確認)から確認できます。
* 【参考】[GitHub アカウントへの新しい SSH キーの追加 | GitHub Docs](https://docs.github.com/ja/free-pro-team@latest/github/authenticating-to-github/adding-a-new-ssh-key-to-your-github-account)
* 【注意】鍵の登録は、PC/Androidに関わらず、KyoRyoJoeをインストールしたすべての端末で行う必要があります。

新規リポジトリの作成
--------------------

KyoRyoJoeは巡目ごとにリポジトリを作成してデータを管理します。
つまり、5年に1回この作業を行います。

以下のドキュメントを参照して、空のリポジトリを作成してください。

* [新しいリポジトリの作成 | GitHub Docs](https://docs.github.com/ja/free-pro-team@latest/github/creating-cloning-and-archiving-repositories/creating-a-new-repository)

### Git管理についての補足

複数の端末を利用する場合、ブランチの運用がおすすめです
* Android端末上で競合すると解決に手間取ります
* データのマージは常にPC上で行う運用が安全です
* 【参考】[GITブランチの作成と運用](../tips/git_branch.md)



橋一覧データのコミット
----------------------

「[橋梁データの作成](make_bridge_data.md)」で作成した橋梁一覧データ（YAML）をリポジトリに追加します。
ブラウザ上で操作できます。
以下のドキュメントを参照して、 **リポジトリの直下に** ファイルを追加してください。

* [ファイルをリポジトリに追加する | GitHub Docs](https://docs.github.com/ja/free-pro-team@latest/github/managing-files-in-a-repository/adding-a-file-to-a-repository)
* 【注意】ドキュメントにも記載されていますが、コミット操作が必要です。

### 橋一覧データについての補足

橋一覧データはいつでも変更できます
* Git管理なので、変更履歴が残ります
* 点検時点の状態は点検データ内にも保存されます
