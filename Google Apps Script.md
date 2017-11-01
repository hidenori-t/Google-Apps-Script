『Google Apps Script クイックリファレンス』
http://www.shuwasystem.co.jp/support/7980html/3675.html
(p.12 par.1 l.)  

```gas:
function myFunction() {
  Logger.log("Hello World");
}
```

(p.22 par.1 l.)  
* 単語補完 Mac: option+/
* コンテンツアシスト Ctrl+Space

(p.26 par.1 l.)  
# 開発したプロジェクトのスナップショットを取るには
「ファイル」→「版を管理」
(p.28 par.1 l.)  
# 作成したプロジェクトのプログラムをライブラリとして利用するには
「リソース」→「ライブラリを管理」


(p.30 par.1 l.)  
# 関数のドキュメント

```gas:
/**
* ?
* @param {型名} 引数名 引数の説明
* @return {型名} 戻り値の説明
*/
function myFunction() {
  Logger.log("Hello World");
}

/**
* 本日の日付オブジェクトを返す。
* @return {date} 本日の日付オブジェクト
*/
function today() {
  return new Date();
}

/**
* 日付を任意のフォーマットの文字列に変換する。
* ただし、変換後の文字列は日本時間で表現される。
*
* @param {date} date 日付オブジェクト
* @param {string} format 変換する書式
* @return {string} 変換後の文字列
*/
function formatJST(date, format) {
  return Utilities.formatDate(date, "JST", format);
}
```

