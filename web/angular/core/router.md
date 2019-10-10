## Router の event のテストをする場合
- Router には NavigationStart などの event が存在するがこの条件のテストをする場合はインスタンス化して `router.events.next()` に渡せばよい

```ts
const event = new NavigationStart(1, '/');
TestBed.get(Router).events.next(event);
```
