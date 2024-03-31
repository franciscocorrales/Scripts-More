```js
type Immutable<T> = {
    readonly [K in keyof T]:
         keyof T[K] extends undefined ?
              T[K] :
              Immutable<T[K]>;
}
```
