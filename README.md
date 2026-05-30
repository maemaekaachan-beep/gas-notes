# gas-notes# GAS メモ

## PropertiesService（機密情報の管理）

トークンやIDをコードに直書きせず、スクリプトプロパティで管理する方法。

### 設定手順
1. GASの歯車アイコン（プロジェクトの設定）を開く
2. 「スクリプトプロパティを追加」でキーと値を登録して保存

### コードの書き方
```js
const LINE_ACCESS_TOKEN = PropertiesService.getScriptProperties().getProperty("LINE_ACCESS_TOKEN");
const SPREADSHEET_ID = PropertiesService.getScriptProperties().getProperty("SPREADSHEET_ID");
```
