# VueUse S

版本：@vueuse/core 14.3.0；包括 core 对外重导出的 shared 可调用项。

## `set`

```ts
set<T>(ref: Ref<T>, value: T): void
set<O extends object, K extends keyof O>(target: O, key: K, value: O[K]): void
```

## `setSSRHandler`

```ts
setSSRHandler<T extends keyof SSRHandlersMap>(key: T, fn: SSRHandlersMap[T]): void
```

## `syncRef`

```ts
syncRef<L, R, D extends Direction = "both">(left: Ref<L>, right: Ref<R>, ...[options]: Equal<L, R> extends true ? [options?: SyncRefOptions<L, R, D>] : [options: SyncRefOptions<L, R, D>]): () => void
```

## `syncRefs`

```ts
syncRefs<T>(source: WatchSource<T>, targets: Ref<T> | Ref<T>[], options?: SyncRefsOptions): _$vue.WatchHandle
```
