## styleguide について
https://google.github.io/styleguide/tsguide.html

## TypeScript exercises
https://typescript-exercises.github.io/

## Advanced types
https://www.typescriptlang.org/docs/handbook/advanced-types.html

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
