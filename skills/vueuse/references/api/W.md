# VueUse W

版本：@vueuse/core 14.3.0；包括 core 对外重导出的 shared 可调用项。

## `watchArray`

```ts
watchArray<T, Immediate extends Readonly<boolean> = false>(source: WatchSource<T[]> | T[], cb: WatchArrayCallback<T[], Immediate extends true ? T[] | undefined : T[]>, options?: WatchOptions<Immediate>): _$vue.WatchHandle
```

## `watchAtMost`

```ts
watchAtMost<T, Immediate extends Readonly<boolean> = false>(sources: WatchSource<T>, cb: WatchCallback<T, Immediate extends true ? T | undefined : T>, options: WatchAtMostOptions<Immediate>): WatchAtMostReturn
watchAtMost<T extends Readonly<MultiWatchSources$1>, Immediate extends Readonly<boolean> = false>(sources: [...T], cb: WatchCallback<MapSources<T>, MapOldSources<T, Immediate>>, options: WatchAtMostOptions<Immediate>): WatchAtMostReturn
watchAtMost<T extends object, Immediate extends Readonly<boolean> = false>(sources: T, cb: WatchCallback<MapSources<T>, MapOldSources<T, Immediate>>, options: WatchAtMostOptions<Immediate>): WatchAtMostReturn
```

## `watchDebounced`

```ts
watchDebounced<T, Immediate extends Readonly<boolean> = false>(source: WatchSource<T>, cb: WatchCallback<T, Immediate extends true ? T | undefined : T>, options?: WatchDebouncedOptions<Immediate>): WatchHandle
watchDebounced<T extends Readonly<MultiWatchSources$1>, Immediate extends Readonly<boolean> = false>(sources: [...T], cb: WatchCallback<MapSources<T>, MapOldSources<T, Immediate>>, options?: WatchDebouncedOptions<Immediate>): WatchHandle
watchDebounced<T extends object, Immediate extends Readonly<boolean> = false>(source: T, cb: WatchCallback<T, Immediate extends true ? T | undefined : T>, options?: WatchDebouncedOptions<Immediate>): WatchHandle
```

## `watchDeep`

```ts
watchDeep<T, Immediate extends Readonly<boolean> = false>(source: WatchSource<T>, cb: WatchCallback<T, Immediate extends true ? T | undefined : T>, options?: Omit<WatchOptions<Immediate>, "deep">): WatchHandle
watchDeep<T extends Readonly<MultiWatchSources$1>, Immediate extends Readonly<boolean> = false>(source: [...T], cb: WatchCallback<MapSources<T>, MapOldSources<T, Immediate>>, options?: Omit<WatchOptions<Immediate>, "deep">): WatchHandle
watchDeep<T extends object, Immediate extends Readonly<boolean> = false>(source: T, cb: WatchCallback<T, Immediate extends true ? T | undefined : T>, options?: Omit<WatchOptions<Immediate>, "deep">): WatchHandle
```

## `watchIgnorable`

```ts
watchIgnorable<T, Immediate extends Readonly<boolean> = false>(source: WatchSource<T>, cb: WatchCallback<T, Immediate extends true ? T | undefined : T>, options?: WatchWithFilterOptions<Immediate>): WatchIgnorableReturn
watchIgnorable<T extends Readonly<MultiWatchSources$1>, Immediate extends Readonly<boolean> = false>(sources: [...T], cb: WatchCallback<MapSources<T>, MapOldSources<T, Immediate>>, options?: WatchWithFilterOptions<Immediate>): WatchIgnorableReturn
watchIgnorable<T extends object, Immediate extends Readonly<boolean> = false>(source: T, cb: WatchCallback<T, Immediate extends true ? T | undefined : T>, options?: WatchWithFilterOptions<Immediate>): WatchIgnorableReturn
```

## `watchImmediate`

```ts
watchImmediate<T>(source: WatchSource<T>, cb: WatchCallback<T, T | undefined>, options?: Omit<WatchOptions<true>, "immediate">): WatchHandle
watchImmediate<T extends Readonly<MultiWatchSources$1>>(source: [...T], cb: WatchCallback<MapSources<T>, MapOldSources<T, true>>, options?: Omit<WatchOptions<true>, "immediate">): WatchHandle
watchImmediate<T extends object>(source: T, cb: WatchCallback<T, T | undefined>, options?: Omit<WatchOptions<true>, "immediate">): WatchHandle
```

## `watchOnce`

```ts
watchOnce<T>(source: WatchSource<T>, cb: WatchCallback<T, T | undefined>, options?: Omit<WatchOptions<true>, "once">): WatchHandle
watchOnce<T extends Readonly<MultiWatchSources$1>>(source: [...T], cb: WatchCallback<MapSources<T>, MapOldSources<T, true>>, options?: Omit<WatchOptions<true>, "once">): WatchHandle
watchOnce<T extends object>(source: T, cb: WatchCallback<T, T | undefined>, options?: Omit<WatchOptions<true>, "once">): WatchHandle
```

## `watchPausable`

```ts
watchPausable<T, Immediate extends Readonly<boolean> = false>(source: WatchSource<T>, cb: WatchCallback<T, Immediate extends true ? T | undefined : T>, options?: WatchPausableOptions<Immediate>): WatchPausableReturn
watchPausable<T extends Readonly<MultiWatchSources$1>, Immediate extends Readonly<boolean> = false>(sources: [...T], cb: WatchCallback<MapSources<T>, MapOldSources<T, Immediate>>, options?: WatchPausableOptions<Immediate>): WatchPausableReturn
watchPausable<T extends object, Immediate extends Readonly<boolean> = false>(source: T, cb: WatchCallback<T, Immediate extends true ? T | undefined : T>, options?: WatchPausableOptions<Immediate>): WatchPausableReturn
```

## `watchThrottled`

```ts
watchThrottled<T, Immediate extends Readonly<boolean> = false>(source: WatchSource<T>, cb: WatchCallback<T, Immediate extends true ? T | undefined : T>, options?: WatchThrottledOptions<Immediate>): WatchHandle
watchThrottled<T extends Readonly<MultiWatchSources$1>, Immediate extends Readonly<boolean> = false>(sources: [...T], cb: WatchCallback<MapSources<T>, MapOldSources<T, Immediate>>, options?: WatchThrottledOptions<Immediate>): WatchHandle
watchThrottled<T extends object, Immediate extends Readonly<boolean> = false>(source: T, cb: WatchCallback<T, Immediate extends true ? T | undefined : T>, options?: WatchThrottledOptions<Immediate>): WatchHandle
```

## `watchTriggerable`

```ts
watchTriggerable<T, FnReturnT>(source: WatchSource<T>, cb: WatchTriggerableCallback<T, T | undefined, FnReturnT>, options?: WatchWithFilterOptions<boolean>): WatchTriggerableReturn<FnReturnT>
watchTriggerable<T extends Readonly<MultiWatchSources$1>, FnReturnT>(sources: [...T], cb: WatchTriggerableCallback<MapSources<T>, MapOldSources<T, true>, FnReturnT>, options?: WatchWithFilterOptions<boolean>): WatchTriggerableReturn<FnReturnT>
watchTriggerable<T extends object, FnReturnT>(source: T, cb: WatchTriggerableCallback<T, T | undefined, FnReturnT>, options?: WatchWithFilterOptions<boolean>): WatchTriggerableReturn<FnReturnT>
```

## `watchWithFilter`

```ts
watchWithFilter<T, Immediate extends Readonly<boolean> = false>(source: WatchSource<T>, cb: WatchCallback<T, Immediate extends true ? T | undefined : T>, options?: WatchWithFilterOptions<Immediate>): WatchHandle
watchWithFilter<T extends Readonly<MultiWatchSources$1>, Immediate extends Readonly<boolean> = false>(sources: [...T], cb: WatchCallback<MapSources<T>, MapOldSources<T, Immediate>>, options?: WatchWithFilterOptions<Immediate>): WatchHandle
watchWithFilter<T extends object, Immediate extends Readonly<boolean> = false>(source: T, cb: WatchCallback<T, Immediate extends true ? T | undefined : T>, options?: WatchWithFilterOptions<Immediate>): WatchHandle
```

## `whenever`

```ts
whenever<T>(source: WatchSource<T>, cb: WatchCallback<Truthy<T>, T | undefined>, options?: WheneverOptions<true>): WatchHandle
whenever<T>(source: WatchSource<T>, cb: WatchCallback<Truthy<T>, T>, options?: WheneverOptions<false>): WatchHandle
```
