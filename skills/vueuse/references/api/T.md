# VueUse T

版本：@vueuse/core 14.3.0；包括 core 对外重导出的 shared 可调用项。

## `templateRef`

```ts
templateRef<T extends HTMLElement | SVGElement | Component | null, Keys extends string = string>(key: Keys, initialValue?: T | null): Readonly<Ref<T>>
```

## `throttledRef`

```ts
throttledRef<T = any>(value: Ref<T>, delay?: number, trailing?: boolean, leading?: boolean): RefThrottledReturn<T>
```

## `throttledWatch`

```ts
throttledWatch<T, Immediate extends Readonly<boolean> = false>(source: WatchSource<T>, cb: WatchCallback<T, Immediate extends true ? T | undefined : T>, options?: WatchThrottledOptions<Immediate>): WatchHandle
throttledWatch<T extends Readonly<MultiWatchSources$1>, Immediate extends Readonly<boolean> = false>(sources: [...T], cb: WatchCallback<MapSources<T>, MapOldSources<T, Immediate>>, options?: WatchThrottledOptions<Immediate>): WatchHandle
throttledWatch<T extends object, Immediate extends Readonly<boolean> = false>(source: T, cb: WatchCallback<T, Immediate extends true ? T | undefined : T>, options?: WatchThrottledOptions<Immediate>): WatchHandle
```

## `throttleFilter`

```ts
throttleFilter(ms: MaybeRefOrGetter<number>, trailing?: boolean, leading?: boolean, rejectOnCancel?: boolean): EventFilter
throttleFilter(options: ThrottleFilterOptions): EventFilter
```

## `timestamp`

```ts
timestamp(): number
```

## `toArray`

```ts
toArray<T>(value: T | readonly T[]): readonly T[]
toArray<T>(value: T | T[]): T[]
```

## `toReactive`

```ts
toReactive<T extends object>(objectRef: MaybeRef<T>): UnwrapNestedRefs<T>
```

## `toRef`

```ts
toRef<T>(r: () => T): Readonly<Ref<T>>
toRef<T>(r: ComputedRef<T>): ComputedRef<T>
toRef<T>(r: MaybeRefOrGetter<T>): Ref<T>
toRef<T>(r: T): Ref<T>
toRef<T extends object, K extends keyof T>(object: T, key: K): ToRef<T[K]>
toRef<T extends object, K extends keyof T>(object: T, key: K, defaultValue: T[K]): ToRef<Exclude<T[K], undefined>>
```

## `toRefs`

```ts
toRefs<T extends object>(objectRef: MaybeRef<T>, options?: ToRefsOptions): ToRefs<T>
```

## `transition`

```ts
transition<T>(source: Ref<T>, from: MaybeRefOrGetter<T>, to: MaybeRefOrGetter<T>, options?: TransitionOptions<T>): PromiseLike<void>
```

## `tryOnBeforeMount`

```ts
tryOnBeforeMount(fn: Fn, sync?: boolean, target?: ComponentInternalInstance | null): void
```

## `tryOnBeforeUnmount`

```ts
tryOnBeforeUnmount(fn: Fn, target?: ComponentInternalInstance | null): void
```

## `tryOnMounted`

```ts
tryOnMounted(fn: Fn, sync?: boolean, target?: ComponentInternalInstance | null): void
```

## `tryOnScopeDispose`

```ts
tryOnScopeDispose(fn: Fn, failSilently?: boolean): boolean
```

## `tryOnUnmounted`

```ts
tryOnUnmounted(fn: Fn, target?: ComponentInternalInstance | null): void
```
