- [documents](https://github.com/angular/angularfire2/blob/master/docs/firestore/documents.md)
- `FirebaseError: Missing or insufficient permissions.` というエラーが出てデータの読み込みができない
    - ルールで何も許可しない設定になっていた `allow read, write: if false;`
- Collection : RDB のテーブルっぽいやつ
- Document : RDB のレコードっぽいやつ