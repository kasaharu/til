## Collection Group Queries
- `where` を使って SQL のように絞り込みができる
    - ref. [Collection Group Queries](https://github.com/angular/angularfire2/blob/992b15882c157d19f7779233e1d5e3da79cf0f03/docs/firestore/querying-collections.md#collection-group-queries)

## Random
- [documents](https://github.com/angular/angularfire2/blob/master/docs/firestore/documents.md)
- `FirebaseError: Missing or insufficient permissions.` というエラーが出てデータの読み込みができない
    - ルールで何も許可しない設定になっていた `allow read, write: if false;`
- Collection : RDB のテーブルっぽいやつ
- Document : RDB のレコードっぽいやつ
