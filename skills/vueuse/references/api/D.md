# VueUse D

版本：@vueuse/core 14.3.0；包括 core 对外重导出的 shared 可调用项。

## `debouncedRef`

```ts
debouncedRef<T>(value: Ref<T>, ms?: MaybeRefOrGetter<number>, options?: DebounceFilterOptions): RefDebouncedReturn<T>
```

## `debouncedWatch`

```ts
debouncedWatch<T, Immediate extends Readonly<boolean> = false>(source: WatchSource<T>, cb: WatchCallback<T, Immediate extends true ? T | undefined : T>, options?: WatchDebouncedOptions<Immediate>): WatchHandle
debouncedWatch<T extends Readonly<MultiWatchSources$1>, Immediate extends Readonly<boolean> = false>(sources: [...T], cb: WatchCallback<MapSources<T>, MapOldSources<T, Immediate>>, options?: WatchDebouncedOptions<Immediate>): WatchHandle
debouncedWatch<T extends object, Immediate extends Readonly<boolean> = false>(source: T, cb: WatchCallback<T, Immediate extends true ? T | undefined : T>, options?: WatchDebouncedOptions<Immediate>): WatchHandle
```

## `debounceFilter`

```ts
debounceFilter(ms: MaybeRefOrGetter<number>, options?: DebounceFilterOptions): EventFilter<any[], any, AnyFn>
```
