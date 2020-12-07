PC上にKyoRyoJoeを構築する
==========================================

Windows・Mac・LinuxにKyoRyoJoeを構築する手順です。

必要なツールのインストール
--------------------------

1. [Git](https://git-scm.com/)
1. [Ruby](https://www.ruby-lang.org/ja/)(>=2.5)
1. Bundler(>=2.1.4)
   * Rubyインストール後に↓のコマンドを実行する
   * `gem install bundler`

ソースコードの取得と実行
------------------------

1. GitHubからソースコードを`clone`する
   * `git clone https://github.com/kyoryojoe/app.git kyoryojoe`
1. インストール
   * `cd kyoryojoe/`
   * `bundle install`
1. 実行（起動）
   * `bundle exec ruby app.rb`
   * ブラウザから`http://localhost:4567/`にアクセスする

その後の操作
------------

1. GitHub上に巡目点検データリポジトリを作成する
   * TODO: →使い方にリンクする
1. 巡目点検データを配置する
   * TODO: →使い方にリンクする

