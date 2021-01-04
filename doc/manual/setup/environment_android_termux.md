Android(Termux)上にKyoRyoJoeを構築する
======================================


Android端末と周辺機器の準備
---------------------------

* [Androidの内部ストレージをSDカードで拡張する](../tips/expand_android_storade.md)
  * 橋梁点検データ（写真）はAndroidストレージを圧迫するため、拡張することをお勧めします。
* [動作実績のあるAndroid端末](../tips/confirmed_devices.md)
  * Androidは機種の差が大きいので、ご参考までに動作確認が取れた機種を紹介しています。
* Bluetoothキーボード
  * Termuxのコマンド操作は物理キーボードがあると便利です。

Termuxインストール
-------------

1. Google PlayストからTermuxをインストールします。
   * [Termux | Google Play](https://play.google.com/store/apps/details?id=com.termux)
1. インストールしたTermuxを起動します。
   * Termux上で以下のコマンドを実行します
   * `pkg update -y`
     * Termuxを最新化するコマンドです。時々応答を求められますので、何も入力せずに`[Enter]`入力してください
   * `termux-setup-storage`
     * Termuxのファイルシステムを初期化するコマンド？みたいです。Androidからストレージアクセスの許可を求められた場合は許可してください


セットアップスクリプトの実行
-----------------

1. Termux上で以下のコマンドを実行します
   * `eval "$(curl https://raw.githubusercontent.com/kyoryojoe/app/main/bin/setup_termux.sh)"`
     * GitHubアカウントのメールアドレス入力が求められます
     * それ以外にも時々応答を求められますので、何も入力せずに`[Enter]`入力してください
   * ↑の入力が面倒な場合は↓のQRコードを読取って、Termux上に貼り付けます
   * ![セットアップスクリプト](qrcode_setup_termux.png)
1. 5分ほどで「セットアップが完了しました」と表示されます
   * 失敗した場合はもう一度実行してください
1. Termuxを再起動します
   * 一般的なAndroid同様、落としてください
     * `[CTRL-D]`入力でも落とせます
   * Termuxを起動します
     * 「KyoRyoJoeが起動しました」と表示されます
     * ブラウザで以下のURLにアクセスしてください
       *  http://localhost:4567/


その後の操作
------------

Android(Termux)でのKyoRyoJoe構築はここまでです。
点検データの配置は別項で説明します。



その他（TODO:
-----

* Termuxを自動起動させる方法
* Termuxを常駐（起動しっぱなし）させる方法
* Androidで音声入力を行う
* Androidで手書き入力を行う
