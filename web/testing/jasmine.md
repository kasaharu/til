## toBeTruthy() と toBe(true) の違い
- boolean の値のテストをするときは `toBe(true)` を使う
    - `toBeTruthy()` は true かどうかの確認ではなく truthy かどうかの確認をする
    - 下記も成立する
    ```
    expect('false').toBeTruthy()
    ```
