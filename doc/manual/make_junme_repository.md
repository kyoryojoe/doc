巡目リポジトリの作成
====================

簡単に説明すると、以下の3ステップです。

1. GitHubアカウントの作成（最初の一回）
1. 新規リポジトリの作成
1. 橋一覧データのコミット


GitHubアカウントの作成（最初の一回）
------------------------------------

点検データは[Git](https://git-scm.com/)で管理することを想定しています。
[GitHub](https://github.com/)アカウントを作成してください。

開発・確認はGitHubにて行っており、ドキュメントもGitHub利用を前提として書いています。
他のGit（サービス）でも動作すると思われますが、未確認です。

GitHubは無料アカウントでも無条件と言ってよいほど緩い制限でリポジトリ（データ）を管理できますが、この状況が変更される可能性はゼロではありません。

* [私のディスク容量はいくつですか？ | GitHub Docs](https://docs.github.com/ja/free-pro-team@latest/github/managing-large-files/what-is-my-disk-quota)


新規リポジトリの作成
--------------------

KyoRyoJoeは巡目ごとにリポジトリを作成してデータを管理します。
（つまり、5年に1回この作業を行います）

以下のドキュメントを参照して、リポジトリを作成してください。

* [新しいリポジトリの作成 | GitHub Docs](https://docs.github.com/ja/free-pro-team@latest/github/creating-cloning-and-archiving-repositories/creating-a-new-repository)

### Git管理についての補足

* リポジトリ名は「junme1（1は何巡目かを表す数字）」とするのが無難です
  * 1巡目のリポジトリを2巡目として読み込むことはできません
  * 厳密にはできますが、エラーになり使えません
* リポジトリはPublicでもPrivateでも構いません。
  * Publicは誰でも参照できます（変更はできません）
  * Privateは許可されたユーザのみ参照、更新できます
  * Public/Privateは後から変更できます

橋一覧データのコミット
----------------------

「[橋梁データの作成](make_bridge_data.md)」で作成した橋梁一覧データ（YAML）をリポジトリに追加します。
ブラウザ上で操作できます。
以下のドキュメントを参照して、 **リポジトリの直下に** ファイルを追加してください。

* [ファイルをリポジトリに追加する | GitHub Docs](https://docs.github.com/ja/free-pro-team@latest/github/managing-files-in-a-repository/adding-a-file-to-a-repository)

ドキュメントにも記載されていますが、コミット操作が必要です。
