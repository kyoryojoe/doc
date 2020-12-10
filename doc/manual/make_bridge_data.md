橋梁データの作成
================

簡単に説明すると、以下の3ステップです。

1. 橋梁一覧データ（CSV）を作成します
1. YAMLに変換します
1. リポジトリに追加します

橋梁一覧データ（CSV）の作成
--------------------------

### CSVヘッダのダウンロード

編集を簡単にするため、CSVヘッダを準備しました。
* [CSVヘッダダウンロード](https://raw.githubusercontent.com/kyoryojoe/app/main/public/bridges_header.csv)

### 橋一覧CSVの作成

CSVヘッダを元に橋梁データの一覧を作成してください。
* [橋梁CSV列の説明](bridge_csv_layout.md)

※CSVファイルの文字コードはUTF-8にしてください

橋梁一覧データを変換する（CSV → YAML）
-------------------------------------

KyoRyoJoe内部で利用するため、CSVをYAMLに変換する必要があります。

* [CSV | Wikipedia](https://ja.wikipedia.org/wiki/Comma-Separated_Values)
* [YAML | Wikipedia](https://ja.wikipedia.org/wiki/YAML)

以下の変換サービスを利用すると、簡単にCSVをYAMLに変換できます。

* [Convert CSV to YAML](https://www.convertcsv.com/csv-to-yaml.htm)

橋梁一覧データをリポジトリに追加する
-----------------------------------

橋梁データ作成の作業はここまでです。
リポジトリ操作は別項で説明します。
