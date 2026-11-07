# VueUse O

版本：@vueuse/core 14.3.0；包括 core 对外重导出的 shared 可调用项。

## `objectEntries`

```ts
objectEntries<T extends object>(obj: T): Array<[keyof T, T[keyof T]]>
```

## `objectOmit`

```ts
objectOmit<O extends object, T extends keyof O>(obj: O, keys: T[], omitUndefined?: boolean): Omit<O, T>
```

## `objectPick`

```ts
objectPick<O extends object, T extends keyof O>(obj: O, keys: T[], omitUndefined?: boolean): Pick<O, T>
```

## `onClickOutside`

```ts
onClickOutside<T extends OnClickOutsideOptions>(target: MaybeComputedElementRef, handler: OnClickOutsideHandler<T>, options?: T): Fn
onClickOutside<T extends OnClickOutsideOptions<true>>(target: MaybeComputedElementRef, handler: OnClickOutsideHandler<T>, options: T): { stop: Fn; cancel: Fn; trigger: (event: Event) => void; }
```

## `onElementRemoval`

```ts
onElementRemoval(target: MaybeElementRef, callback: (mutationRecords: MutationRecord[]) => void, options?: OnElementRemovalOptions): Fn
```

## `onKeyDown`

```ts
onKeyDown(key: KeyFilter, handler: (event: KeyboardEvent) => void, options?: Omit<OnKeyStrokeOptions, "eventName">): () => void
```

## `onKeyPressed`

```ts
onKeyPressed(key: KeyFilter, handler: (event: KeyboardEvent) => void, options?: Omit<OnKeyStrokeOptions, "eventName">): () => void
```

## `onKeyStroke`

```ts
onKeyStroke(key: KeyFilter, handler: (event: KeyboardEvent) => void, options?: OnKeyStrokeOptions): () => void
onKeyStroke(handler: (event: KeyboardEvent) => void, options?: OnKeyStrokeOptions): () => void
```

## `onKeyUp`

```ts
onKeyUp(key: KeyFilter, handler: (event: KeyboardEvent) => void, options?: Omit<OnKeyStrokeOptions, "eventName">): () => void
```

## `onLongPress`

```ts
onLongPress(target: MaybeElementRef, handler: (evt: PointerEvent) => void, options?: OnLongPressOptions): OnLongPressReturn
```

## `onStartTyping`

```ts
onStartTyping(callback: (event: KeyboardEvent) => void, options?: ConfigurableDocument): void
```
