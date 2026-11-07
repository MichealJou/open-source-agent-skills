# VueUse G

版本：@vueuse/core 14.3.0；包括 core 对外重导出的 shared 可调用项。

## `get`

```ts
get<T>(ref: MaybeRef<T>): T
get<T, K extends keyof T>(ref: MaybeRef<T>, key: K): T[K]
```

## `getLifeCycleTarget`

```ts
getLifeCycleTarget(target?: ComponentInternalInstance | null): ComponentInternalInstance | null
```

## `getSSRHandler`

```ts
getSSRHandler<T extends keyof SSRHandlersMap>(key: T, fallback: SSRHandlersMap[T]): SSRHandlersMap[T]
getSSRHandler<T extends keyof SSRHandlersMap>(key: T, fallback: SSRHandlersMap[T] | undefined): SSRHandlersMap[T] | undefined
```
