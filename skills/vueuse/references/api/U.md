# VueUse U

版本：@vueuse/core 14.3.0；包括 core 对外重导出的 shared 可调用项。

## `unrefElement`

```ts
unrefElement<T extends MaybeElement>(elRef: MaybeComputedElementRef<T>): UnRefElementReturn<T>
```

## `until`

```ts
until<T extends unknown[]>(r: WatchSource<T> | MaybeRefOrGetter<T>): UntilArrayInstance<T>
until<T>(r: WatchSource<T> | MaybeRefOrGetter<T>): UntilValueInstance<T>
```

## `useActiveElement`

```ts
useActiveElement<T extends HTMLElement>(options?: UseActiveElementOptions): UseActiveElementReturn<T>
```

## `useAnimate`

```ts
useAnimate(target: MaybeComputedElementRef, keyframes: UseAnimateKeyframes, options?: number | UseAnimateOptions): UseAnimateReturn
```

## `useArrayDifference`

```ts
useArrayDifference<T>(list: MaybeRefOrGetter<T[]>, values: MaybeRefOrGetter<T[]>, key?: keyof T, options?: UseArrayDifferenceOptions): UseArrayDifferenceReturn<T>
useArrayDifference<T>(list: MaybeRefOrGetter<T[]>, values: MaybeRefOrGetter<T[]>, compareFn?: (value: T, othVal: T) => boolean, options?: UseArrayDifferenceOptions): UseArrayDifferenceReturn<T>
```

## `useArrayEvery`

```ts
useArrayEvery<T>(list: MaybeRefOrGetter<MaybeRefOrGetter<T>[]>, fn: (element: T, index: number, array: MaybeRefOrGetter<T>[]) => unknown): UseArrayEveryReturn
```

## `useArrayFilter`

```ts
useArrayFilter<T, S extends T>(list: MaybeRefOrGetter<MaybeRefOrGetter<T>[]>, fn: (element: T, index: number, array: T[]) => element is S): UseArrayFilterReturn<S>
useArrayFilter<T>(list: MaybeRefOrGetter<MaybeRefOrGetter<T>[]>, fn: (element: T, index: number, array: T[]) => unknown): UseArrayFilterReturn<T>
```

## `useArrayFind`

```ts
useArrayFind<T>(list: MaybeRefOrGetter<MaybeRefOrGetter<T>[]>, fn: (element: T, index: number, array: MaybeRefOrGetter<T>[]) => boolean): UseArrayFindReturn<T>
```

## `useArrayFindIndex`

```ts
useArrayFindIndex<T>(list: MaybeRefOrGetter<MaybeRefOrGetter<T>[]>, fn: (element: T, index: number, array: MaybeRefOrGetter<T>[]) => unknown): UseArrayFindIndexReturn
```

## `useArrayFindLast`

```ts
useArrayFindLast<T>(list: MaybeRefOrGetter<MaybeRefOrGetter<T>[]>, fn: (element: T, index: number, array: MaybeRefOrGetter<T>[]) => boolean): UseArrayFindLastReturn<T>
```

## `useArrayIncludes`

```ts
useArrayIncludes<T, V = any>(list: MaybeRefOrGetter<MaybeRefOrGetter<T>[]>, value: MaybeRefOrGetter<V>, comparator?: UseArrayIncludesComparatorFn<T, V>): UseArrayIncludesReturn
useArrayIncludes<T, V = any>(list: MaybeRefOrGetter<MaybeRefOrGetter<T>[]>, value: MaybeRefOrGetter<V>, comparator?: keyof T): UseArrayIncludesReturn
useArrayIncludes<T, V = any>(list: MaybeRefOrGetter<MaybeRefOrGetter<T>[]>, value: MaybeRefOrGetter<V>, options?: UseArrayIncludesOptions<T, V>): UseArrayIncludesReturn
```

## `useArrayJoin`

```ts
useArrayJoin(list: MaybeRefOrGetter<MaybeRefOrGetter<any>[]>, separator?: MaybeRefOrGetter<string>): UseArrayJoinReturn
```

## `useArrayMap`

```ts
useArrayMap<T, U = T>(list: MaybeRefOrGetter<MaybeRefOrGetter<T>[]>, fn: (element: T, index: number, array: T[]) => U): UseArrayMapReturn<U>
```

## `useArrayReduce`

```ts
useArrayReduce<T>(list: MaybeRefOrGetter<MaybeRefOrGetter<T>[]>, reducer: UseArrayReducer<T, T, T>): UseArrayReduceReturn<T>
useArrayReduce<T, U>(list: MaybeRefOrGetter<MaybeRefOrGetter<T>[]>, reducer: UseArrayReducer<U, T, U>, initialValue: MaybeRefOrGetter<U>): UseArrayReduceReturn<U>
```

## `useArraySome`

```ts
useArraySome<T>(list: MaybeRefOrGetter<MaybeRefOrGetter<T>[]>, fn: (element: T, index: number, array: MaybeRefOrGetter<T>[]) => unknown): UseArraySomeReturn
```

## `useArrayUnique`

```ts
useArrayUnique<T>(list: MaybeRefOrGetter<MaybeRefOrGetter<T>[]>, compareFn?: (a: T, b: T, array: T[]) => boolean): UseArrayUniqueReturn<T>
```

## `useAsyncQueue`

```ts
useAsyncQueue<T extends any[], S = MapQueueTask<T>>(tasks: S & Array<UseAsyncQueueTask<any>>, options?: UseAsyncQueueOptions): UseAsyncQueueReturn<{ [P in keyof T]: UseAsyncQueueResult<T[P]>; }>
```

## `useAsyncState`

```ts
useAsyncState<Data, Params extends any[] = any[], Shallow extends boolean = true>(promise: Promise<Data> | ((...args: Params) => Promise<Data>), initialState: MaybeRef<Data>, options?: UseAsyncStateOptions<Shallow, Data>): UseAsyncStateReturn<Data, Params, Shallow>
```

## `useBase64`

```ts
useBase64(target: MaybeRefOrGetter<string | undefined>, options?: UseBase64Options): UseBase64Return
useBase64(target: MaybeRefOrGetter<Blob | undefined>, options?: UseBase64Options): UseBase64Return
useBase64(target: MaybeRefOrGetter<ArrayBuffer | undefined>, options?: UseBase64Options): UseBase64Return
useBase64(target: MaybeRefOrGetter<HTMLCanvasElement | undefined>, options?: ToDataURLOptions): UseBase64Return
useBase64(target: MaybeRefOrGetter<HTMLImageElement | undefined>, options?: ToDataURLOptions): UseBase64Return
useBase64<T extends Record<string, unknown>>(target: MaybeRefOrGetter<T>, options?: UseBase64ObjectOptions<T>): UseBase64Return
useBase64<T extends Map<string, unknown>>(target: MaybeRefOrGetter<T>, options?: UseBase64ObjectOptions<T>): UseBase64Return
useBase64<T extends Set<unknown>>(target: MaybeRefOrGetter<T>, options?: UseBase64ObjectOptions<T>): UseBase64Return
useBase64<T>(target: MaybeRefOrGetter<T[]>, options?: UseBase64ObjectOptions<T[]>): UseBase64Return
```

## `useBattery`

```ts
useBattery(options?: UseBatteryOptions): UseBatteryReturn
```

## `useBluetooth`

```ts
useBluetooth(options?: UseBluetoothOptions): UseBluetoothReturn
```

## `useBreakpoints`

```ts
useBreakpoints<K extends string>(breakpoints: Breakpoints<K>, options?: UseBreakpointsOptions): UseBreakpointReturn<K>
```

## `useBroadcastChannel`

```ts
useBroadcastChannel<D, P>(options: UseBroadcastChannelOptions): UseBroadcastChannelReturn<D, P>
```

## `useBrowserLocation`

```ts
useBrowserLocation(options?: UseBrowserLocationOptions): UseBrowserLocationReturn
```

## `useCached`

```ts
useCached<T, D extends boolean = true>(refValue: Ref<T>, comparator?: (newSourceValue: T, cachedValue: T) => boolean, options?: UseCachedOptions<D>): UseCachedReturn<T, D>
```

## `useClipboard`

```ts
useClipboard(options?: UseClipboardOptions<undefined>): UseClipboardReturn<false>
useClipboard(options: UseClipboardOptions<MaybeRefOrGetter<string>>): UseClipboardReturn<true>
```

## `useClipboardItems`

```ts
useClipboardItems(options?: UseClipboardItemsOptions<undefined>): UseClipboardItemsReturn<false>
useClipboardItems(options: UseClipboardItemsOptions<MaybeRefOrGetter<ClipboardItems>>): UseClipboardItemsReturn<true>
```

## `useCloned`

```ts
useCloned<T>(source: MaybeRefOrGetter<T>, options?: UseClonedOptions): UseClonedReturn<T>
```

## `useColorMode`

```ts
useColorMode<T extends string = BasicColorMode>(options?: UseColorModeOptions<T>): UseColorModeReturn<T>
```

## `useConfirmDialog`

```ts
useConfirmDialog<RevealData = any, ConfirmData = any, CancelData = any>(revealed?: ShallowRef<boolean>): UseConfirmDialogReturn<RevealData, ConfirmData, CancelData>
```

## `useCountdown`

```ts
useCountdown(initialCountdown: MaybeRefOrGetter<number>, options?: UseCountdownOptions): UseCountdownReturn
```

## `useCounter`

```ts
useCounter(initialValue?: MaybeRef<number>, options?: UseCounterOptions): { count: Readonly<Ref<number, number> | _$vue.ShallowRef<number, number> | _$vue.WritableComputedRef<number, number>>; inc: (delta?: number) => number; dec: (delta?: number) => number; get: () => number; set: (val: number) => number; reset: (val?: number) => number; }
```

## `useCssSupports`

```ts
useCssSupports(property: MaybeRefOrGetter<string>, value: MaybeRefOrGetter<string>, options?: UseCssSupportsOptions): UseCssSupportsReturn
useCssSupports(conditionText: MaybeRefOrGetter<string>, options?: UseCssSupportsOptions): UseCssSupportsReturn
```

## `useCssVar`

```ts
useCssVar(prop: MaybeRefOrGetter<string | null | undefined>, target?: MaybeElementRef, options?: UseCssVarOptions): _$vue.ShallowRef<string | undefined, string | undefined>
```

## `useCurrentElement`

```ts
useCurrentElement<T extends MaybeElement = MaybeElement, R extends VueInstance = VueInstance, E extends MaybeElement = MaybeElement extends T ? _$_vueuse_shared0.IsAny<R["$el"]> extends false ? R["$el"] : T : T>(rootComponent?: MaybeElementRef<R>): _$_vueuse_shared0.ComputedRefWithControl<E>
```

## `useCycleList`

```ts
useCycleList<T>(list: MaybeRefOrGetter<T[]>, options?: UseCycleListOptions<T>): UseCycleListReturn<T>
```

## `useDark`

```ts
useDark(options?: UseDarkOptions): UseDarkReturn
```

## `useDateFormat`

```ts
useDateFormat(date: MaybeRefOrGetter<DateLike>, formatStr?: MaybeRefOrGetter<string>, options?: UseDateFormatOptions): UseDateFormatReturn
```

## `useDebounce`

```ts
useDebounce<T>(value: Ref<T>, ms?: MaybeRefOrGetter<number>, options?: DebounceFilterOptions): RefDebouncedReturn<T>
```

## `useDebouncedRefHistory`

```ts
useDebouncedRefHistory<Raw, Serialized = Raw>(source: Ref<Raw>, options?: Omit<UseRefHistoryOptions<Raw, Serialized>, "eventFilter"> & { debounce?: MaybeRefOrGetter<number>; }): UseRefHistoryReturn<Raw, Serialized>
```

## `useDebounceFn`

```ts
useDebounceFn<T extends FunctionArgs>(fn: T, ms?: MaybeRefOrGetter<number>, options?: DebounceFilterOptions): UseDebounceFnReturn<T>
```

## `useDeviceMotion`

```ts
useDeviceMotion(options?: UseDeviceMotionOptions): UseDeviceMotionReturn
```

## `useDeviceOrientation`

```ts
useDeviceOrientation(options?: UseDeviceOrientationOptions): UseDeviceOrientationReturn
```

## `useDevicePixelRatio`

```ts
useDevicePixelRatio(options?: UseDevicePixelRatioOptions): UseDevicePixelRatioReturn
```

## `useDevicesList`

```ts
useDevicesList(options?: UseDevicesListOptions): UseDevicesListReturn
```

## `useDisplayMedia`

```ts
useDisplayMedia(options?: UseDisplayMediaOptions): UseDisplayMediaReturn
```

## `useDocumentVisibility`

```ts
useDocumentVisibility(options?: UseDocumentVisibilityOptions): UseDocumentVisibilityReturn
```

## `useDraggable`

```ts
useDraggable(target: MaybeRefOrGetter<HTMLElement | SVGElement | null | undefined>, options?: UseDraggableOptions): UseDraggableReturn
```

## `useDropZone`

```ts
useDropZone(target: MaybeRefOrGetter<HTMLElement | Document | null | undefined>, options?: UseDropZoneOptions | UseDropZoneOptions["onDrop"]): UseDropZoneReturn
```

## `useElementBounding`

```ts
useElementBounding(target: MaybeComputedElementRef, options?: UseElementBoundingOptions): UseElementBoundingReturn
```

## `useElementByPoint`

```ts
useElementByPoint<M extends boolean = false>(options: UseElementByPointOptions<M>): UseElementByPointReturn<M>
```

## `useElementHover`

```ts
useElementHover(el: MaybeRefOrGetter<EventTarget | null | undefined>, options?: UseElementHoverOptions): ShallowRef<boolean>
```

## `useElementSize`

```ts
useElementSize(target: MaybeComputedElementRef, initialSize?: ElementSize, options?: UseElementSizeOptions): UseElementSizeReturn
```

## `useElementVisibility`

```ts
useElementVisibility(element: MaybeComputedElementRef, options?: UseElementVisibilityOptions<false>): UseElementVisibilityReturn<false>
useElementVisibility(element: MaybeComputedElementRef, options?: UseElementVisibilityOptions<true>): UseElementVisibilityReturn<true>
```

## `useEventBus`

```ts
useEventBus<T = unknown, P = any>(key: EventBusIdentifier<T>): UseEventBusReturn<T, P>
```

## `useEventListener`

```ts
useEventListener<E extends keyof WindowEventMap>(event: MaybeRefOrGetter<Arrayable<E>>, listener: MaybeRef<Arrayable<(this: Window, ev: WindowEventMap[E]) => any>>, options?: MaybeRefOrGetter<boolean | AddEventListenerOptions>): Fn
useEventListener<E extends keyof WindowEventMap>(target: Window, event: MaybeRefOrGetter<Arrayable<E>>, listener: MaybeRef<Arrayable<(this: Window, ev: WindowEventMap[E]) => any>>, options?: MaybeRefOrGetter<boolean | AddEventListenerOptions>): Fn
useEventListener<E extends keyof DocumentEventMap>(target: Document, event: MaybeRefOrGetter<Arrayable<E>>, listener: MaybeRef<Arrayable<(this: Document, ev: DocumentEventMap[E]) => any>>, options?: MaybeRefOrGetter<boolean | AddEventListenerOptions>): Fn
useEventListener<E extends keyof ShadowRootEventMap>(target: MaybeRefOrGetter<Arrayable<ShadowRoot> | null | undefined>, event: MaybeRefOrGetter<Arrayable<E>>, listener: MaybeRef<Arrayable<(this: ShadowRoot, ev: ShadowRootEventMap[E]) => any>>, options?: MaybeRefOrGetter<boolean | AddEventListenerOptions>): Fn
useEventListener<E extends keyof HTMLElementEventMap>(target: MaybeRefOrGetter<Arrayable<HTMLElement> | null | undefined>, event: MaybeRefOrGetter<Arrayable<E>>, listener: MaybeRef<(this: HTMLElement, ev: HTMLElementEventMap[E]) => any>, options?: MaybeRefOrGetter<boolean | AddEventListenerOptions>): Fn
useEventListener<Names extends string, EventType = Event>(target: MaybeRefOrGetter<Arrayable<InferEventTarget<Names>> | null | undefined>, event: MaybeRefOrGetter<Arrayable<Names>>, listener: MaybeRef<Arrayable<GeneralEventListener<EventType>>>, options?: MaybeRefOrGetter<boolean | AddEventListenerOptions>): Fn
useEventListener<EventType = Event>(target: MaybeRefOrGetter<Arrayable<EventTarget> | null | undefined>, event: MaybeRefOrGetter<Arrayable<string>>, listener: MaybeRef<Arrayable<GeneralEventListener<EventType>>>, options?: MaybeRefOrGetter<boolean | AddEventListenerOptions>): Fn
```

## `useEventSource`

```ts
useEventSource<Events extends string[], Data = any>(url: MaybeRefOrGetter<string | URL | undefined>, events?: Events, options?: UseEventSourceOptions<Data>): UseEventSourceReturn<Events, Data>
```

## `useEyeDropper`

```ts
useEyeDropper(options?: UseEyeDropperOptions): UseEyeDropperReturn
```

## `useFavicon`

```ts
useFavicon(newIcon: ReadonlyRefOrGetter<string | null | undefined>, options?: UseFaviconOptions): ComputedRef<string | null | undefined>
useFavicon(newIcon?: MaybeRef<string | null | undefined>, options?: UseFaviconOptions): Ref<string | null | undefined>
```

## `useFetch`

```ts
useFetch<T>(url: MaybeRefOrGetter<string>): UseFetchReturn<T> & PromiseLike<UseFetchReturn<T>>
useFetch<T>(url: MaybeRefOrGetter<string>, useFetchOptions: UseFetchOptions): UseFetchReturn<T> & PromiseLike<UseFetchReturn<T>>
useFetch<T>(url: MaybeRefOrGetter<string>, options: RequestInit, useFetchOptions?: UseFetchOptions): UseFetchReturn<T> & PromiseLike<UseFetchReturn<T>>
```

## `useFileDialog`

```ts
useFileDialog(options?: UseFileDialogOptions): UseFileDialogReturn
```

## `useFileSystemAccess`

```ts
useFileSystemAccess(): UseFileSystemAccessReturn<string | ArrayBuffer | Blob>
useFileSystemAccess(options: UseFileSystemAccessOptions & { dataType: "Text"; }): UseFileSystemAccessReturn<string>
useFileSystemAccess(options: UseFileSystemAccessOptions & { dataType: "ArrayBuffer"; }): UseFileSystemAccessReturn<ArrayBuffer>
useFileSystemAccess(options: UseFileSystemAccessOptions & { dataType: "Blob"; }): UseFileSystemAccessReturn<Blob>
useFileSystemAccess(options: UseFileSystemAccessOptions): UseFileSystemAccessReturn<string | ArrayBuffer | Blob>
```

## `useFocus`

```ts
useFocus(target: MaybeElementRef, options?: UseFocusOptions): UseFocusReturn
```

## `useFocusWithin`

```ts
useFocusWithin(target: MaybeElementRef, options?: ConfigurableWindow): UseFocusWithinReturn
```

## `useFps`

```ts
useFps(options?: UseFpsOptions): ShallowRef<number>
```

## `useFullscreen`

```ts
useFullscreen(target?: MaybeElementRef, options?: UseFullscreenOptions): UseFullscreenReturn
```

## `useGamepad`

```ts
useGamepad(options?: UseGamepadOptions): UseGamepadReturn
```

## `useGeolocation`

```ts
useGeolocation(options?: UseGeolocationOptions): UseGeolocationReturn
```

## `useIdle`

```ts
useIdle(timeout?: number, options?: UseIdleOptions): UseIdleReturn
```

## `useImage`

```ts
useImage<Shallow extends true>(options: MaybeRefOrGetter<UseImageOptions>, asyncStateOptions?: UseAsyncStateOptions<Shallow>): UseImageReturn
```

## `useInfiniteScroll`

```ts
useInfiniteScroll<T extends InfiniteScrollElement>(element: MaybeRefOrGetter<T>, onLoadMore: (state: UnwrapNestedRefs<UseScrollReturn>) => Awaitable<void>, options?: UseInfiniteScrollOptions<T>): UseInfiniteScrollReturn
```

## `useIntersectionObserver`

```ts
useIntersectionObserver(target: MaybeComputedElementRef | MaybeRefOrGetter<MaybeElement[]> | MaybeComputedElementRef[], callback: IntersectionObserverCallback, options?: UseIntersectionObserverOptions): UseIntersectionObserverReturn
```

## `useInterval`

```ts
useInterval(interval?: MaybeRefOrGetter<number>, options?: UseIntervalOptions<false>): Readonly<ShallowRef<number>>
useInterval(interval: MaybeRefOrGetter<number>, options: UseIntervalOptions<true>): Readonly<UseIntervalControls & Pausable>
```

## `useIntervalFn`

```ts
useIntervalFn(cb: Fn, interval?: MaybeRefOrGetter<number>, options?: UseIntervalFnOptions): UseIntervalFnReturn
```

## `useKeyModifier`

```ts
useKeyModifier<Initial extends boolean | null>(modifier: KeyModifier, options?: UseModifierOptions<Initial>): UseKeyModifierReturn<Initial>
```

## `useLastChanged`

```ts
useLastChanged(source: WatchSource, options?: UseLastChangedOptions<false>): Readonly<ShallowRef<number | null>>
useLastChanged(source: WatchSource, options: UseLastChangedOptions<true> | UseLastChangedOptions<boolean, number>): Readonly<ShallowRef<number>>
```

## `useLocalStorage`

```ts
useLocalStorage(key: MaybeRefOrGetter<string>, initialValue: MaybeRefOrGetter<string>, options?: UseStorageOptions<string>): RemovableRef<string>
useLocalStorage(key: MaybeRefOrGetter<string>, initialValue: MaybeRefOrGetter<boolean>, options?: UseStorageOptions<boolean>): RemovableRef<boolean>
useLocalStorage(key: MaybeRefOrGetter<string>, initialValue: MaybeRefOrGetter<number>, options?: UseStorageOptions<number>): RemovableRef<number>
useLocalStorage<T>(key: MaybeRefOrGetter<string>, initialValue: MaybeRefOrGetter<T>, options?: UseStorageOptions<T>): RemovableRef<T>
useLocalStorage<T = unknown>(key: MaybeRefOrGetter<string>, initialValue: MaybeRefOrGetter<null>, options?: UseStorageOptions<T>): RemovableRef<T>
```

## `useMagicKeys`

```ts
useMagicKeys<T extends boolean = false>(options?: UseMagicKeysOptions<T>): UseMagicKeysReturn<T>
```

## `useManualRefHistory`

```ts
useManualRefHistory<Raw, Serialized = Raw>(source: Ref<Raw>, options?: UseManualRefHistoryOptions<Raw, Serialized>): UseManualRefHistoryReturn<Raw, Serialized>
```

## `useMediaControls`

```ts
useMediaControls(target: MaybeRef<HTMLMediaElement | null | undefined>, options?: UseMediaControlsOptions): UseMediaControlsReturn
```

## `useMediaQuery`

```ts
useMediaQuery(query: MaybeRefOrGetter<string>, options?: ConfigurableWindow & { ssrWidth?: number; }): _$vue.ComputedRef<boolean>
```

## `useMemoize`

```ts
useMemoize<Result, Args extends unknown[]>(resolver: (...args: Args) => Result, options?: UseMemoizeOptions<Result, Args>): UseMemoizeReturn<Result, Args>
```

## `useMemory`

```ts
useMemory(options?: UseMemoryOptions): UseMemoryReturn
```

## `useMounted`

```ts
useMounted(): _$vue.ShallowRef<boolean, boolean>
```

## `useMouse`

```ts
useMouse(options?: UseMouseOptions): UseMouseReturn
```

## `useMouseInElement`

```ts
useMouseInElement(target?: MaybeElementRef, options?: MouseInElementOptions): { x: ShallowRef<number>; y: ShallowRef<number>; sourceType: ShallowRef<UseMouseSourceType>; elementX: ShallowRef<number, number>; elementY: ShallowRef<number, number>; elementPositionX: ShallowRef<number, number>; elementPositionY: ShallowRef<number, number>; elementHeight: ShallowRef<number, number>; elementWidth: ShallowRef<number, number>; isOutside: ShallowRef<boolean, boolean>; stop: () => void; }
```

## `useMousePressed`

```ts
useMousePressed(options?: UseMousePressedOptions): UseMousePressedReturn
```

## `useMutationObserver`

```ts
useMutationObserver(target: MaybeComputedElementRef | MaybeComputedElementRef[] | MaybeRefOrGetter<MaybeElement[]>, callback: MutationCallback, options?: UseMutationObserverOptions): UseMutationObserverReturn
```

## `useNavigatorLanguage`

```ts
useNavigatorLanguage(options?: UseNavigatorLanguageOptions): UseNavigatorLanguageReturn
```

## `useNetwork`

```ts
useNetwork(options?: UseNetworkOptions): UseNetworkReturn
```

## `useNow`

```ts
useNow(options?: UseNowOptions<false>): ShallowRef<Date>
useNow(options: UseNowOptions<true>): { now: ShallowRef<Date>; } & Pausable
```

## `useObjectUrl`

```ts
useObjectUrl(object: MaybeRefOrGetter<Blob | MediaSource | null | undefined>): Readonly<_$vue.ShallowRef<string | undefined, string | undefined>>
```

## `useOffsetPagination`

```ts
useOffsetPagination(options: Omit<UseOffsetPaginationOptions, "total">): UseOffsetPaginationInfinityPageReturn
useOffsetPagination(options: UseOffsetPaginationOptions): UseOffsetPaginationReturn
```

## `useOnline`

```ts
useOnline(options?: ConfigurableWindow): Readonly<_$vue.ShallowRef<boolean>>
```

## `usePageLeave`

```ts
usePageLeave(options?: UsePageLeaveOptions): UsePageLeaveReturn
```

## `useParallax`

```ts
useParallax(target: MaybeElementRef, options?: UseParallaxOptions): UseParallaxReturn
```

## `useParentElement`

```ts
useParentElement(element?: MaybeRefOrGetter<HTMLElement | SVGElement | null | undefined>): Readonly<ShallowRef<HTMLElement | SVGElement | null | undefined>>
```

## `usePerformanceObserver`

```ts
usePerformanceObserver(options: UsePerformanceObserverOptions, callback: PerformanceObserverCallback): { isSupported: UseSupportedReturn; start: () => void; stop: () => void; }
```

## `usePermission`

```ts
usePermission(permissionDesc: GeneralPermissionDescriptor | GeneralPermissionDescriptor["name"], options?: UsePermissionOptions<false>): UsePermissionReturn
usePermission(permissionDesc: GeneralPermissionDescriptor | GeneralPermissionDescriptor["name"], options: UsePermissionOptions<true>): UsePermissionReturnWithControls
```

## `usePointer`

```ts
usePointer(options?: UsePointerOptions): UsePointerReturn
```

## `usePointerLock`

```ts
usePointerLock(target?: MaybeElementRef, options?: UsePointerLockOptions): UsePointerLockReturn
```

## `usePointerSwipe`

```ts
usePointerSwipe(target: MaybeRefOrGetter<HTMLElement | null | undefined>, options?: UsePointerSwipeOptions): UsePointerSwipeReturn
```

## `usePreferredColorScheme`

```ts
usePreferredColorScheme(options?: ConfigurableWindow): _$vue.ComputedRef<ColorSchemeType>
```

## `usePreferredContrast`

```ts
usePreferredContrast(options?: ConfigurableWindow): _$vue.ComputedRef<ContrastType>
```

## `usePreferredDark`

```ts
usePreferredDark(options?: ConfigurableWindow): _$vue.ComputedRef<boolean>
```

## `usePreferredLanguages`

```ts
usePreferredLanguages(options?: ConfigurableWindow): ShallowRef<readonly string[]>
```

## `usePreferredReducedMotion`

```ts
usePreferredReducedMotion(options?: ConfigurableWindow): _$vue.ComputedRef<ReducedMotionType>
```

## `usePreferredReducedTransparency`

```ts
usePreferredReducedTransparency(options?: ConfigurableWindow): _$vue.ComputedRef<ReducedTransparencyType>
```

## `usePrevious`

```ts
usePrevious<T>(value: MaybeRefOrGetter<T>): Readonly<ShallowRef<T | undefined>>
usePrevious<T>(value: MaybeRefOrGetter<T>, initialValue: T): Readonly<ShallowRef<T>>
```

## `useRafFn`

```ts
useRafFn(fn: (args: UseRafFnCallbackArguments) => void, options?: UseRafFnOptions): Pausable
```

## `useRefHistory`

```ts
useRefHistory<Raw, Serialized = Raw>(source: Ref<Raw>, options?: UseRefHistoryOptions<Raw, Serialized>): UseRefHistoryReturn<Raw, Serialized>
```

## `useResizeObserver`

```ts
useResizeObserver(target: MaybeComputedElementRef | MaybeComputedElementRef[] | MaybeRefOrGetter<MaybeElement[]>, callback: globalThis.ResizeObserverCallback, options?: UseResizeObserverOptions): UseResizeObserverReturn
```

## `useScreenOrientation`

```ts
useScreenOrientation(options?: UseScreenOrientationOptions): UseScreenOrientationReturn
```

## `useScreenSafeArea`

```ts
useScreenSafeArea(): UseScreenSafeAreaReturn
```

## `useScriptTag`

```ts
useScriptTag(src: MaybeRefOrGetter<string>, onLoaded?: (el: HTMLScriptElement) => void, options?: UseScriptTagOptions): UseScriptTagReturn
```

## `useScroll`

```ts
useScroll(element: MaybeRefOrGetter<HTMLElement | SVGElement | Window | Document | null | undefined>, options?: UseScrollOptions): UseScrollReturn
```

## `useScrollLock`

```ts
useScrollLock(element: MaybeRefOrGetter<HTMLElement | SVGElement | Window | Document | null | undefined>, initialState?: boolean): _$vue.WritableComputedRef<boolean, boolean>
```

## `useSessionStorage`

```ts
useSessionStorage(key: MaybeRefOrGetter<string>, initialValue: MaybeRefOrGetter<string>, options?: UseStorageOptions<string>): RemovableRef<string>
useSessionStorage(key: MaybeRefOrGetter<string>, initialValue: MaybeRefOrGetter<boolean>, options?: UseStorageOptions<boolean>): RemovableRef<boolean>
useSessionStorage(key: MaybeRefOrGetter<string>, initialValue: MaybeRefOrGetter<number>, options?: UseStorageOptions<number>): RemovableRef<number>
useSessionStorage<T>(key: MaybeRefOrGetter<string>, initialValue: MaybeRefOrGetter<T>, options?: UseStorageOptions<T>): RemovableRef<T>
useSessionStorage<T = unknown>(key: MaybeRefOrGetter<string>, initialValue: MaybeRefOrGetter<null>, options?: UseStorageOptions<T>): RemovableRef<T>
```

## `useShare`

```ts
useShare(shareOptions?: MaybeRefOrGetter<UseShareOptions>, options?: ConfigurableNavigator): UseShareReturn
```

## `useSorted`

```ts
useSorted<T = any>(source: MaybeRefOrGetter<T[]>, compareFn?: UseSortedCompareFn<T>): Ref<T[]>
useSorted<T = any>(source: MaybeRefOrGetter<T[]>, options?: UseSortedOptions<T>): Ref<T[]>
useSorted<T = any>(source: MaybeRefOrGetter<T[]>, compareFn?: UseSortedCompareFn<T>, options?: Omit<UseSortedOptions<T>, "compareFn">): Ref<T[]>
```

## `useSpeechRecognition`

```ts
useSpeechRecognition(options?: UseSpeechRecognitionOptions): UseSpeechRecognitionReturn
```

## `useSpeechSynthesis`

```ts
useSpeechSynthesis(text: MaybeRefOrGetter<string>, options?: UseSpeechSynthesisOptions): UseSpeechSynthesisReturn
```

## `useSSRWidth`

```ts
useSSRWidth(): number | undefined
```

## `useStepper`

```ts
useStepper<T extends string | number>(steps: MaybeRef<T[]>, initialStep?: T): UseStepperReturn<T, T[], T>
useStepper<T extends Record<string, any>>(steps: MaybeRef<T>, initialStep?: keyof T): UseStepperReturn<Exclude<keyof T, symbol>, T, T[keyof T]>
```

## `useStorage`

```ts
useStorage(key: MaybeRefOrGetter<string>, defaults: MaybeRefOrGetter<string>, storage?: StorageLike, options?: UseStorageOptions<string>): RemovableRef<string>
useStorage(key: MaybeRefOrGetter<string>, defaults: MaybeRefOrGetter<boolean>, storage?: StorageLike, options?: UseStorageOptions<boolean>): RemovableRef<boolean>
useStorage(key: MaybeRefOrGetter<string>, defaults: MaybeRefOrGetter<number>, storage?: StorageLike, options?: UseStorageOptions<number>): RemovableRef<number>
useStorage<T>(key: MaybeRefOrGetter<string>, defaults: MaybeRefOrGetter<T>, storage?: StorageLike, options?: UseStorageOptions<T>): RemovableRef<T>
useStorage<T = unknown>(key: MaybeRefOrGetter<string>, defaults: MaybeRefOrGetter<null>, storage?: StorageLike, options?: UseStorageOptions<T>): RemovableRef<T>
```

## `useStorageAsync`

```ts
useStorageAsync(key: string, initialValue: MaybeRefOrGetter<string>, storage?: StorageLikeAsync, options?: UseStorageAsyncOptions<string>): RemovableRef<string> & Promise<RemovableRef<string>>
useStorageAsync(key: string, initialValue: MaybeRefOrGetter<boolean>, storage?: StorageLikeAsync, options?: UseStorageAsyncOptions<boolean>): RemovableRef<boolean> & Promise<RemovableRef<boolean>>
useStorageAsync(key: string, initialValue: MaybeRefOrGetter<number>, storage?: StorageLikeAsync, options?: UseStorageAsyncOptions<number>): RemovableRef<number> & Promise<RemovableRef<number>>
useStorageAsync<T>(key: string, initialValue: MaybeRefOrGetter<T>, storage?: StorageLikeAsync, options?: UseStorageAsyncOptions<T>): RemovableRef<T> & Promise<RemovableRef<T>>
useStorageAsync<T = unknown>(key: string, initialValue: MaybeRefOrGetter<null>, storage?: StorageLikeAsync, options?: UseStorageAsyncOptions<T>): RemovableRef<T> & Promise<RemovableRef<T>>
```

## `useStyleTag`

```ts
useStyleTag(css: MaybeRef<string>, options?: UseStyleTagOptions): UseStyleTagReturn
```

## `useSupported`

```ts
useSupported(callback: () => unknown): UseSupportedReturn
```

## `useSwipe`

```ts
useSwipe(target: MaybeRefOrGetter<EventTarget | null | undefined>, options?: UseSwipeOptions): UseSwipeReturn
```

## `useTemplateRefsList`

```ts
useTemplateRefsList<T = Element>(): Readonly<Ref<Readonly<TemplateRefsList<T>>>>
```

## `useTextareaAutosize`

```ts
useTextareaAutosize(options?: UseTextareaAutosizeOptions): UseTextareaAutosizeReturn
```

## `useTextDirection`

```ts
useTextDirection(options?: UseTextDirectionOptions): _$vue.WritableComputedRef<UseTextDirectionValue, UseTextDirectionValue>
```

## `useTextSelection`

```ts
useTextSelection(options?: UseTextSelectionOptions): UseTextSelectionReturn
```

## `useThrottle`

```ts
useThrottle<T = any>(value: Ref<T>, delay?: number, trailing?: boolean, leading?: boolean): RefThrottledReturn<T>
```

## `useThrottledRefHistory`

```ts
useThrottledRefHistory<Raw, Serialized = Raw>(source: Ref<Raw>, options?: UseThrottledRefHistoryOptions<Raw, Serialized>): UseThrottledRefHistoryReturn<Raw, Serialized>
```

## `useThrottleFn`

```ts
useThrottleFn<T extends FunctionArgs>(fn: T, ms?: MaybeRefOrGetter<number>, trailing?: boolean, leading?: boolean, rejectOnCancel?: boolean): PromisifyFn<T>
```

## `useTimeAgo`

```ts
useTimeAgo<UnitNames extends string = UseTimeAgoUnitNamesDefault>(time: MaybeRefOrGetter<Date | number | string>, options?: UseTimeAgoOptions<false, UnitNames>): UseTimeAgoReturn<false>
useTimeAgo<UnitNames extends string = UseTimeAgoUnitNamesDefault>(time: MaybeRefOrGetter<Date | number | string>, options: UseTimeAgoOptions<true, UnitNames>): UseTimeAgoReturn<true>
```

## `useTimeAgoIntl`

```ts
useTimeAgoIntl(time: MaybeRefOrGetter<Date | number | string>, options?: UseTimeAgoIntlOptions<false>): UseTimeAgoReturn$1<false>
useTimeAgoIntl(time: MaybeRefOrGetter<Date | number | string>, options: UseTimeAgoIntlOptions<true>): UseTimeAgoReturn$1<true>
```

## `useTimeout`

```ts
useTimeout(interval?: MaybeRefOrGetter<number>, options?: UseTimeoutOptions<false>): ComputedRef<boolean>
useTimeout(interval: MaybeRefOrGetter<number>, options: UseTimeoutOptions<true>): { ready: ComputedRef<boolean>; } & Stoppable
```

## `useTimeoutFn`

```ts
useTimeoutFn<CallbackFn extends AnyFn>(cb: CallbackFn, interval: MaybeRefOrGetter<number>, options?: UseTimeoutFnOptions): UseTimeoutFnReturn<CallbackFn>
```

## `useTimeoutPoll`

```ts
useTimeoutPoll(fn: () => Awaitable<void>, interval: MaybeRefOrGetter<number>, options?: UseTimeoutFnOptions): Pausable
```

## `useTimestamp`

```ts
useTimestamp(options?: UseTimestampOptions<false>): ShallowRef<number>
useTimestamp(options: UseTimestampOptions<true>): { timestamp: ShallowRef<number>; } & Pausable
```

## `useTitle`

```ts
useTitle(newTitle: ReadonlyRefOrGetter<string | null | undefined>, options?: UseTitleOptions): ComputedRef<string | null | undefined>
useTitle(newTitle?: MaybeRef<string | null | undefined>, options?: UseTitleOptions): Ref<string | null | undefined>
```

## `useToggle`

```ts
useToggle<Truthy, Falsy, T = Truthy | Falsy>(initialValue: Ref<T>, options?: UseToggleOptions<Truthy, Falsy>): (value?: T) => T
useToggle<Truthy = true, Falsy = false, T = Truthy | Falsy>(initialValue?: T, options?: UseToggleOptions<Truthy, Falsy>): [ShallowRef<T>, (value?: T) => T]
```

## `useToNumber`

```ts
useToNumber(value: MaybeRefOrGetter<number | string>, options?: UseToNumberOptions): ComputedRef<number>
```

## `useToString`

```ts
useToString(value: MaybeRefOrGetter<unknown>): ComputedRef<string>
```

## `useTransition`

```ts
useTransition<T extends MaybeRefOrGetter<number>[]>(source: [...T], options?: UseTransitionOptions<T>): ComputedRef<{ [K in keyof T]: number; }>
useTransition<T extends MaybeRefOrGetter<number[]>>(source: T, options?: UseTransitionOptions<T>): ComputedRef<number[]>
useTransition<T>(source: MaybeRefOrGetter<T>, options?: UseTransitionOptions<T>): ComputedRef<T>
```

## `useUrlSearchParams`

```ts
useUrlSearchParams<T extends Record<string, any> = UrlParams>(mode?: "history" | "hash" | "hash-params", options?: UseUrlSearchParamsOptions<T>): T
```

## `useUserMedia`

```ts
useUserMedia(options?: UseUserMediaOptions): UseUserMediaReturn
```

## `useVibrate`

```ts
useVibrate(options?: UseVibrateOptions): UseVibrateReturn
```

## `useVirtualList`

```ts
useVirtualList<T = any>(list: MaybeRef<readonly T[]>, options: UseVirtualListOptions): UseVirtualListReturn<T>
```

## `useVModel`

```ts
useVModel<P extends object, K extends keyof P, Name extends string>(props: P, key?: K, emit?: (name: Name, ...args: any[]) => void, options?: UseVModelOptions<P[K], false>): WritableComputedRef<P[K]>
useVModel<P extends object, K extends keyof P, Name extends string>(props: P, key?: K, emit?: (name: Name, ...args: any[]) => void, options?: UseVModelOptions<P[K], true>): Ref<UnwrapRef<P[K]>>
```

## `useVModels`

```ts
useVModels<P extends object, Name extends string>(props: P, emit?: (name: Name, ...args: any[]) => void, options?: UseVModelOptions<any, true>): ToRefs<P>
useVModels<P extends object, Name extends string>(props: P, emit?: (name: Name, ...args: any[]) => void, options?: UseVModelOptions<any, false>): ToRefs<P>
```

## `useWakeLock`

```ts
useWakeLock(options?: UseWakeLockOptions): UseWakeLockReturn
```

## `useWebNotification`

```ts
useWebNotification(options?: UseWebNotificationOptions): UseWebNotificationReturn
```

## `useWebSocket`

```ts
useWebSocket<Data = any>(url: MaybeRefOrGetter<string | URL | undefined>, options?: UseWebSocketOptions): UseWebSocketReturn<Data>
```

## `useWebWorker`

```ts
useWebWorker<T = any>(url: string, workerOptions?: WorkerOptions, options?: ConfigurableWindow): UseWebWorkerReturn<T>
useWebWorker<T = any>(worker: Worker | WorkerFn): UseWebWorkerReturn<T>
```

## `useWebWorkerFn`

```ts
useWebWorkerFn<T extends (...fnArgs: any[]) => any>(fn: T, options?: UseWebWorkerOptions): UseWebWorkerFnReturn<T>
```

## `useWindowFocus`

```ts
useWindowFocus(options?: ConfigurableWindow): ShallowRef<boolean>
```

## `useWindowScroll`

```ts
useWindowScroll(options?: UseWindowScrollOptions): UseWindowScrollReturn
```

## `useWindowSize`

```ts
useWindowSize(options?: UseWindowSizeOptions): UseWindowSizeReturn
```
