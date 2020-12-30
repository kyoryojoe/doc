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

鍵の生成
--------

* 鍵を生成する
  * `ssh-keygen -t rsa`
* コマンド`ssh-keygen`は、OpenSSHがインストールされている必要があります。
  * Windowsの場合、Gitインストール時にGitBash共々入ります
  * mac、Linuxの場合、最初から入ってる？（要調査


その後の操作
------------

PCでのKyoRyoJoe構築はここまでです。
点検データの配置は別項で説明します。
