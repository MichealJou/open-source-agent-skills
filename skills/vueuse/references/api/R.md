# VueUse R

版本：@vueuse/core 14.3.0；包括 core 对外重导出的 shared 可调用项。

## `rand`

```ts
rand(min: number, max: number): number
```

## `reactify`

```ts
reactify<T extends AnyFn, K extends boolean = true>(fn: T, options?: ReactifyOptions<K>): ReactifyReturn<T, K>
```

## `reactifyObject`

```ts
reactifyObject<T extends object, Keys extends keyof T>(obj: T, keys?: (keyof T)[]): ReactifyObjectReturn<T, Keys, true>
reactifyObject<T extends object, S extends boolean = true>(obj: T, options?: ReactifyObjectOptions<S>): ReactifyObjectReturn<T, keyof T, S>
```

## `reactiveComputed`

```ts
reactiveComputed<T extends object>(fn: ComputedGetter<T>): ReactiveComputedReturn<T>
```

## `reactiveOmit`

```ts
reactiveOmit<T extends object, K extends keyof T>(obj: T, ...keys: (K | K[])[]): ReactiveOmitReturn<T, K>
reactiveOmit<T extends object>(obj: T, predicate: ReactiveOmitPredicate<T>): ReactiveOmitReturn<T>
```

## `reactivePick`

```ts
reactivePick<T extends object, K extends keyof T>(obj: T, ...keys: (K | K[])[]): ReactivePickReturn<T, K>
reactivePick<T extends object>(obj: T, predicate: ReactivePickPredicate<T>): ReactivePickReturn<T, keyof T>
```

## `refAutoReset`

```ts
refAutoReset<T>(defaultValue: MaybeRefOrGetter<T>, afterMs?: MaybeRefOrGetter<number>): RefAutoResetReturn<T>
```

## `refDebounced`

```ts
refDebounced<T>(value: Ref<T>, ms?: MaybeRefOrGetter<number>, options?: DebounceFilterOptions): RefDebouncedReturn<T>
```

## `refDefault`

```ts
refDefault<T>(source: Ref<T | undefined | null>, defaultValue: T): Ref<T>
```

## `refManualReset`

```ts
refManualReset<T>(defaultValue: MaybeRefOrGetter<T>): ManualResetRefReturn<T>
```

## `refThrottled`

```ts
refThrottled<T = any>(value: Ref<T>, delay?: number, trailing?: boolean, leading?: boolean): RefThrottledReturn<T>
```

## `refWithControl`

```ts
refWithControl<T>(initial: T, options?: ControlledRefOptions<T>): { get: (tracking?: boolean) => T; set: (value: T, triggering?: boolean) => void; untrackedGet: () => T; silentSet: (v: T) => void; peek: () => T; lay: (v: T) => void; } & _$vue.Ref<T, T>
```
