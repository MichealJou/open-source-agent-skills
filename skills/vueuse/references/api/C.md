# VueUse C

版本：@vueuse/core 14.3.0；包括 core 对外重导出的 shared 可调用项。

## `camelize`

```ts
camelize(str: string): string
```

## `clamp`

```ts
clamp(n: number, min: number, max: number): number
```

## `cloneFnJSON`

```ts
cloneFnJSON<T>(source: T): T
```

## `computedAsync`

```ts
computedAsync<T>(evaluationCallback: (onCancel: AsyncComputedOnCancel) => T | Promise<T>, initialState: T, optionsOrRef: AsyncComputedOptions<true>): ComputedRef<T>
computedAsync<T>(evaluationCallback: (onCancel: AsyncComputedOnCancel) => T | Promise<T>, initialState: undefined, optionsOrRef: AsyncComputedOptions<true>): ComputedRef<T | undefined>
computedAsync<T>(evaluationCallback: (onCancel: AsyncComputedOnCancel) => T | Promise<T>, initialState: T, optionsOrRef?: Ref<boolean> | AsyncComputedOptions): Ref<T>
computedAsync<T>(evaluationCallback: (onCancel: AsyncComputedOnCancel) => T | Promise<T>, initialState?: undefined, optionsOrRef?: Ref<boolean> | AsyncComputedOptions): Ref<T | undefined>
```

## `computedEager`

```ts
computedEager<T>(fn: () => T, options?: ComputedEagerOptions): ComputedEagerReturn<T>
```

## `computedInject`

```ts
computedInject<T, K = any>(key: InjectionKey<T> | string, getter: ComputedInjectGetter<T, K>): ComputedRef<K | undefined>
computedInject<T, K = any>(key: InjectionKey<T> | string, options: WritableComputedInjectOptions<T, K>): ComputedRef<K | undefined>
computedInject<T, K = any>(key: InjectionKey<T> | string, getter: ComputedInjectGetterWithDefault<T, K>, defaultSource: T, treatDefaultAsFactory?: false): ComputedRef<K>
computedInject<T, K = any>(key: InjectionKey<T> | string, options: WritableComputedInjectOptionsWithDefault<T, K>, defaultSource: T | (() => T), treatDefaultAsFactory: true): ComputedRef<K>
```

## `computedWithControl`

```ts
computedWithControl<T>(source: WatchSource | MultiWatchSources$1, fn: ComputedGetter<T>, options?: WatchOptions): ComputedRefWithControl<T>
computedWithControl<T>(source: WatchSource | MultiWatchSources$1, fn: WritableComputedOptions<T>, options?: WatchOptions): WritableComputedRefWithControl<T>
```

## `containsProp`

```ts
containsProp(obj: object, ...props: string[]): boolean
```

## `controlledComputed`

```ts
controlledComputed<T>(source: WatchSource | MultiWatchSources$1, fn: ComputedGetter<T>, options?: WatchOptions): ComputedRefWithControl<T>
controlledComputed<T>(source: WatchSource | MultiWatchSources$1, fn: WritableComputedOptions<T>, options?: WatchOptions): WritableComputedRefWithControl<T>
```

## `controlledRef`

```ts
controlledRef<T>(initial: T, options?: ControlledRefOptions<T>): { get: (tracking?: boolean) => T; set: (value: T, triggering?: boolean) => void; untrackedGet: () => T; silentSet: (v: T) => void; peek: () => T; lay: (v: T) => void; } & _$vue.Ref<T, T>
```

## `createDisposableDirective`

```ts
createDisposableDirective<H extends HTMLElement, V, A = any>(origin?: originDirective<H, V, A>): originDirective<H, V, A>
```

## `createEventHook`

```ts
createEventHook<T = any>(): EventHookReturn<T>
```

## `createFetch`

```ts
createFetch(config?: CreateFetchOptions): typeof useFetch
```

## `createFilterWrapper`

```ts
createFilterWrapper<T extends AnyFn>(filter: EventFilter, fn: T): (this: any, ...args: ArgumentsType<T>) => Promise<Awaited<ReturnType<T>>>
```

## `createGlobalState`

```ts
createGlobalState<Fn extends AnyFn>(stateFactory: Fn): CreateGlobalStateReturn<Fn>
```

## `createInjectionState`

```ts
createInjectionState<Arguments extends Array<any>, Return>(composable: (...args: Arguments) => Return, options: { defaultValue: Return; } & CreateInjectionStateOptions<Return>): CreateInjectionStateReturn<Arguments, Return, Return>
createInjectionState<Arguments extends Array<any>, Return>(composable: (...args: Arguments) => Return, options?: CreateInjectionStateOptions<Return>): CreateInjectionStateReturn<Arguments, Return, Return | undefined>
```

## `createReactiveFn`

```ts
createReactiveFn<T extends AnyFn, K extends boolean = true>(fn: T, options?: ReactifyOptions<K>): ReactifyReturn<T, K>
```

## `createRef`

```ts
createRef<T = any, D extends boolean = false>(value: T, deep?: D): CreateRefReturn<T, D>
```

## `createReusableTemplate`

```ts
createReusableTemplate<Bindings extends Record<string, any>, MapSlotNameToSlotProps extends ObjectLiteralWithPotentialObjectLiterals = Record<"default", undefined>>(options?: CreateReusableTemplateOptions<Bindings>): ReusableTemplatePair<Bindings, MapSlotNameToSlotProps>
```

## `createSharedComposable`

```ts
createSharedComposable<Fn extends AnyFn>(composable: Fn): SharedComposableReturn<Fn>
```

## `createSingletonPromise`

```ts
createSingletonPromise<T>(fn: () => Promise<T>): SingletonPromiseReturn<T>
```

## `createTemplatePromise`

```ts
createTemplatePromise<Return, Args extends any[] = []>(options?: TemplatePromiseOptions): TemplatePromise<Return, Args>
```

## `createUnrefFn`

```ts
createUnrefFn<T extends Function>(fn: T): UnrefFn<T>
```
