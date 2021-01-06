巡目リポジトリのクローン
========================

KyoRyoJoeをインストールした端末に、必要な巡目リポジトリをクローンしてください。

* 今巡目、前巡目のリポジトリが配置されていると、比較しながら点検が行えて便利です。


画面からクローン操作を行う
--------------------------

業務選択/ツール画面から[巡目リポジトリ配置](../operation/work_page.md#巡目リポジトリ配置)を行えます。

コマンドラインからクローン操作を行う
------------------------------------

1. リポジトリ管理ディレクトリに移動します
   * `cd //kyoryojoe/public/inspects/repositories`
     * KyoRyoJoeルートディレクトリを`//kyoryojoe`と記載しています。
     環境に合わせて変更してください。
     * Android(Termux)の場合は`~/kyoryojoe/public/inspects/repositories`です。
1. 巡目リポジトリをクローンします(コマンド例は2巡目)
   * `git clone git@github.com:USERNAME/REPOSITORY.git junme2`
   * リポジトリのURLはご自身のリポジトリに合わせて変更してください
     * [リポジトリをクローンする | GitHub Docs](https://docs.github.com/ja/free-pro-team@latest/github/creating-cloning-and-archiving-repositories/cloning-a-repository)


【補足】巡目リポジトリの削除
----------------------------

この操作は主に、ストレージの容量の制限が厳しいAndroid端末で行われることを想定しています。
端末内の（ローカル）リポジトリを削除しても、Gitの（リモート）リポジトリは削除されません。

リポジトリの削除ツールは提供していません。
コマンドラインから操作してください。

1. リポジトリ管理ディレクトリに移動します
   * `cd //kyoryojoe-app/public/inspects/repositories`
     * KyoRyoJoeルートディレクトリを`//kyoryojoe-app`と記載しています。
     環境に合わせて変更してください。
     * Android(Termux)の場合は`~/kyoryojoe/public/inspects/repositories`です。
1. 巡目リポジトリを削除します(コマンド例は2巡目)
   * `rm -r -d -f junme2`

