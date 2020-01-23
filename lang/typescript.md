## 交差型(Intersection Types)
- 2 つの型を統合して作る

```ts
const interfece Name {
  firstName: string,
  lastName: string,
}

const type User = Name & { age: number };
```

## Generics
- method

```ts
identity<T>(arg: T): T {
  return arg;
}
```
