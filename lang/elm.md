## 匿名関数
- 名前を持たない関数
```elm
isNegative = \n -> n < 0
```

## if 式
- Elm の if は式 → 値を返せる → そのまま関数に渡すことが可能
- `then` と `else` で同じ型の値を返す必要がある
- `else` は省略不可
