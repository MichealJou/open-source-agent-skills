# VueUse A

版本：@vueuse/core 14.3.0；包括 core 对外重导出的 shared 可调用项。

## `assert`

```ts
assert(condition: boolean, ...infos: any[]): void
```

## `asyncComputed`

```ts
asyncComputed<T>(evaluationCallback: (onCancel: AsyncComputedOnCancel) => T | Promise<T>, initialState: T, optionsOrRef: AsyncComputedOptions<true>): ComputedRef<T>
asyncComputed<T>(evaluationCallback: (onCancel: AsyncComputedOnCancel) => T | Promise<T>, initialState: undefined, optionsOrRef: AsyncComputedOptions<true>): ComputedRef<T | undefined>
asyncComputed<T>(evaluationCallback: (onCancel: AsyncComputedOnCancel) => T | Promise<T>, initialState: T, optionsOrRef?: Ref<boolean> | AsyncComputedOptions): Ref<T>
asyncComputed<T>(evaluationCallback: (onCancel: AsyncComputedOnCancel) => T | Promise<T>, initialState?: undefined, optionsOrRef?: Ref<boolean> | AsyncComputedOptions): Ref<T | undefined>
```

## `autoResetRef`

```ts
autoResetRef<T>(defaultValue: MaybeRefOrGetter<T>, afterMs?: MaybeRefOrGetter<number>): RefAutoResetReturn<T>
```
