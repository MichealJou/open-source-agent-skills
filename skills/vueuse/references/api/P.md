# VueUse P

版本：@vueuse/core 14.3.0；包括 core 对外重导出的 shared 可调用项。

## `pausableFilter`

```ts
pausableFilter(extendFilter?: EventFilter, options?: PausableFilterOptions): Pausable & { eventFilter: EventFilter; }
```

## `pausableWatch`

```ts
pausableWatch<T, Immediate extends Readonly<boolean> = false>(source: WatchSource<T>, cb: WatchCallback<T, Immediate extends true ? T | undefined : T>, options?: WatchPausableOptions<Immediate>): WatchPausableReturn
pausableWatch<T extends Readonly<MultiWatchSources$1>, Immediate extends Readonly<boolean> = false>(sources: [...T], cb: WatchCallback<MapSources<T>, MapOldSources<T, Immediate>>, options?: WatchPausableOptions<Immediate>): WatchPausableReturn
pausableWatch<T extends object, Immediate extends Readonly<boolean> = false>(source: T, cb: WatchCallback<T, Immediate extends true ? T | undefined : T>, options?: WatchPausableOptions<Immediate>): WatchPausableReturn
```

## `promiseTimeout`

```ts
promiseTimeout(ms: number, throwOnTimeout?: boolean, reason?: string): Promise<void>
```

## `provideLocal`

```ts
provideLocal<T, K = LocalProvidedKey<T>>(key: K, value: K extends InjectionKey<infer V> ? V : T): ProvideLocalReturn
```

## `provideSSRWidth`

```ts
provideSSRWidth(width: number | null, app?: App<unknown>): void
```

## `pxValue`

```ts
pxValue(px: string): number
```
