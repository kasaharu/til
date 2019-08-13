## toBeTruthy() と toBe(true) の違い
- boolean の値のテストをするときは `toBe(true)` を使う
    - `toBeTruthy()` は true かどうかの確認ではなく truthy かどうかの確認をする
    - 下記も成立する
    ```
    expect('false').toBeTruthy()
    ```

## jasmine.createSpy()
- 実装のない object を生成する。
- [createSpy](https://github.com/jasmine/jasmine.github.io/blob/8c1f66e3a1f02c40a15eaeb6b77cb71d8d0186bb/_versions/2.9/lib/jasmine.js#L322-L324) を見ると中身は function
