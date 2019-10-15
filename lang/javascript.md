## console.table
- 配列やオブジェクトを渡した時 Devtools 上にテーブル形式で表現される

## [Object.entries()](https://developer.mozilla.org/ja/docs/Web/JavaScript/Reference/Global_Objects/Object/entries)
- オブジェクトを key と value の組みからなる配列を返す
```js
Object.entries(obj).forEach(([key, value]) => {
    console.log(`${key} ${value}`);
});
```
