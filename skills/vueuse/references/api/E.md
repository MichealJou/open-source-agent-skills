# VueUse E

版本：@vueuse/core 14.3.0；包括 core 对外重导出的 shared 可调用项。

## `eagerComputed`

```ts
eagerComputed<T>(fn: () => T, options?: ComputedEagerOptions): ComputedEagerReturn<T>
```

## `executeTransition`

```ts
executeTransition<T>(source: Ref<T>, from: MaybeRefOrGetter<T>, to: MaybeRefOrGetter<T>, options?: TransitionOptions<T>): PromiseLike<void>
```

## `extendRef`

```ts
extendRef<R extends Ref<any>, Extend extends object, Options extends ExtendRefOptions<false>>(ref: R, extend: Extend, options?: Options): ShallowUnwrapRef$1<Extend> & R
extendRef<R extends Ref<any>, Extend extends object, Options extends ExtendRefOptions>(ref: R, extend: Extend, options?: Options): Extend & R
```
