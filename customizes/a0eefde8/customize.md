# チケット閲覧画面で編集を行う際にコメント欄へのフォーカスとスクロールをやめる

チケット閲覧画面で編集を行う際に、コメント欄へのフォーカスとスクロールをやめて表示します。  
コメント欄に自動でフォーカスとスクロールすることを防ぎ、スマホなどでアクセスした時、チケット項目を閲覧しやすくしたい際などに利用できます。

対応バージョン：RedMica 2.4.1

## 注意事項

* チケットのコメントを引用してコメントする場合など、未対応の操作があります。
* 表示のカスタマイズの項目「プライベート」がOFFの場合は全てのユーザーに影響します。
* パスのパターンを間違えるとフォーラムなどの機能もコメント欄へのフォーカスとスクロールができなくなります。

## 設定

パスのパターン: `/issues/[0-9]+`

挿入位置: 全ページの末尾

種別: CSS

コード:

``` javascript
function showAndScrollTo(id, focus) {
  $('#'+id).show();
}
```
コメント: チケット閲覧画面で編集を行う際にコメント欄へのフォーカスとスクロールをやめる