橋梁CSV列の説明
===============


列の説明
--------

読みやすさのため、パートごとに説明します。
「必須」「取り得る値」については次項以降で説明します。

#### 基本情報

|物理名|論理名|必須|取り得る値|備考|
|------|------|----|----------|----|
|id                |連番            |〇|整数          |重複しない連番を指定し、以後、変更しないでください|
|bridge_name       |橋梁名          |△|文字列        ||
|bridge_name_kana  |橋梁名カナ      |  |文字列（カナ）||
|address           |所在地          |△|文字列        ||
|address_kana      |所在地カナ      |  |文字列（カナ）||
|location_latitude |起点位置（緯度）|△|少数          |両方入力されているとGoogleMapsへのリンクが表示されます|
|location_longitude|起点位置（経度）|△|少数          |両方入力されているとGoogleMapsへのリンクが表示されます|

#### 周辺環境

|物理名|論理名|必須|取り得る値|備考|
|------|------|----|----------|----|
|route_name              |路線名      ||文字列      |     |
|road_condition          |路下条件    ||文字列      |     |
|alternative_road        |代替路の有無||真偽値      |有無 |
|road_division_cd        |道路区分    ||道路区分    |1（一般道）、2（高速道路）、0（その他）|
|emergency_transport_road|緊急輸送道路||真偽値      |○× |
|traffic_volume          |交通量      ||整数        |台/日|
|occupied_property       |占有物件    ||真偽値      |有無 |
|occupied_property_name  |占有物件名  ||文字列      |     |

#### 橋梁仕様

|物理名|論理名|必須|取り得る値|備考|
|------|------|----|----------|----|
|construction_year|設置年次  |  |整数|年           |
|bridge_length    |橋長      |  |少数|m（メートル）|
|bridge_width     |幅員      |  |少数|m（メートル）|
|load_limit       |荷重制限  |  |少数|kg           |
|number_of_piers  |橋脚数    |△|整数|点検データのひな型自動作成に影響します（未指定は0扱い）|
|number_of_spans  |径間数    |  |整数|             |
|number_of_griders|主桁数    |△|整数|点検データのひな型自動作成に影響します（未指定は0扱い）|
|number_of_beams  |横桁数    |△|整数|点検データのひな型自動作成に影響します（未指定は0扱い）|


「必須」列の説明
----------------

|値|説明|
|--|----|
|〇|必須です。必ず指定してください|
|△|利便性のため指定推奨です      |
|（空）||

必須でない項目は後からでも追記・変更できます。

「取り得る値」列の説明
----------------------

|値|説明|
|--|----|
|整数          ||
|少数          ||
|真偽値        |`true`か`false`、未指定は`false`扱い|
|文字列        |任意の文字列                        |
|文字列（カナ）|カナで入力されることを想定した文字列|
|道路区分      |備考欄参照                          |