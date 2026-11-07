# VueUse I

版本：@vueuse/core 14.3.0；包括 core 对外重导出的 shared 可调用项。

## `identity`

```ts
identity<T>(arg: T): T
```

## `ignorableWatch`

```ts
ignorableWatch<T, Immediate extends Readonly<boolean> = false>(source: WatchSource<T>, cb: WatchCallback<T, Immediate extends true ? T | undefined : T>, options?: WatchWithFilterOptions<Immediate>): WatchIgnorableReturn
ignorableWatch<T extends Readonly<MultiWatchSources$1>, Immediate extends Readonly<boolean> = false>(sources: [...T], cb: WatchCallback<MapSources<T>, MapOldSources<T, Immediate>>, options?: WatchWithFilterOptions<Immediate>): WatchIgnorableReturn
ignorableWatch<T extends object, Immediate extends Readonly<boolean> = false>(source: T, cb: WatchCallback<T, Immediate extends true ? T | undefined : T>, options?: WatchWithFilterOptions<Immediate>): WatchIgnorableReturn
```

## `increaseWithUnit`

```ts
increaseWithUnit(target: number, delta: number): number
increaseWithUnit(target: string, delta: number): string
increaseWithUnit(target: string | number, delta: number): string | number
```

## `injectLocal`

```ts
injectLocal<T>(key: InjectionKey<T> | string): T | undefined
injectLocal<T>(key: InjectionKey<T> | string, defaultValue: T, treatDefaultAsFactory?: false): T
injectLocal<T>(key: InjectionKey<T> | string, defaultValue: T | (() => T), treatDefaultAsFactory: true): T
```

## `invoke`

```ts
invoke<T>(fn: () => T): T
```

## `isDef`

```ts
isDef<T = any>(val?: T): val is T
```

## `isDefined`

```ts
isDefined<T>(v: ComputedRef<T>): v is ComputedRef<Exclude<T, null | undefined>>
isDefined<T>(v: Ref<T>): v is Ref<Exclude<T, null | undefined>>
isDefined<T>(v: T): v is Exclude<T, null | undefined>
```

## `isObject`

```ts
isObject(val: any): val is object
```
