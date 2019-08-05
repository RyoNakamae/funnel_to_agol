# 概要
SORACOMのFunnel のPartner Hosted AdapterにてArcGIS Onlineへ送信するための設定がEsri Japanのサイトに不足しているので、備忘録を兼ねて保存しておく

## Config_sigfox
Sigfoxの検証用デバイスである[Sens'it](https://soracom.jp/products/sigfox/sensit/)用の設定
+ d_id：device：デバイスID(IMSI)を使用して既存の位置情報に紐づける
+ D_TIME：time：センサーの情報取得時間
+ v_dbl_1：tempC：気温
+ v_dbl_2：humidity：湿度
+ v_dbl_3：battery：バッテリー残量
+ v_dbl_4：rssi：照度
+ v_int_1：mode：現在のセンシングモード
+ v_str_1：station：
+ v_str_2：modeText：現在のセンシングモード

## Config_LTM-Button
SORACOMの「あのボタン」こと[LTM-Mボタン](https://soracom.jp/products/gadgets/)用の設定
+ d_id：IMSIを設定
+ lat/lng：簡易測位機能にて取得する位置情報を設定
+ v_dbl_1：バッテリー残量
+ v_int_1：クリック種別(1/2)
+ v_str_1：クリック種別(Single/Double)
+ v_str_2：簡易測位機能にて位置情報取得に成功したかどうか


