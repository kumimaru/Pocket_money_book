# お小遣い残高管理システム

## 入力

Google Home

## 出力

LINE

## Google App Scriptsの処理内容

本システムは　Google App Scripts　で実装する。
ここでは毎月10000円追加する処理がある。

## その他の処理

入力　から　出力まではIFTTTを用いて管理する。
流れは以下の通り。

1. Google Home　で使用した金額を入力
2. IFTTTで受け取った金額をGASに渡す
3. GASでは残高 - 受け取った金額　を計算し、保持
4. 計算結果が入ったセルが更新されたら、IFTTTを起動
5. IFTTT　からLINEに更新結果の値を通知
