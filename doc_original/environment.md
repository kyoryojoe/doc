動作環境
========

KyoRyoJoeは点検現場ではAndroid端末を利用して橋梁点検を行います。

報告書の作成は、PC(Windows, Mac, Linux)で行うことを想定しています。
点検権結果データを閲覧のために、PCにもKyoRyoJoeがインストールされていると便利です。

GitHub
----

点検データは[Git](https://git-scm.com/)で管理することを想定しています。
[GitHub](https://github.com/)アカウントを作成してください。

他のGit（サービス）でも動くはずですが、開発・確認はGitHubにて行っています。


PC
----

* [PC上に構築する | 動作環境](environment_pc.md)
* 現場サーバ化するならルータ化が必要
  * 【参考】[Windowsをルータにする方法 | 俺の技術メモ](http://xn--u9j0md1592aqmt715c.net/windows-router/)
  * 【注意】同じ点検データを同時に変更できません！お互いにデータを壊しあいます


Android（Termux利用）
--------------------

* [Termux on Android上に構築する | 動作環境](environment_android_termux.md)


Webサーバ（インターネット公開）
--------------------------------------

* 非推奨なのでドキュメント作らない

