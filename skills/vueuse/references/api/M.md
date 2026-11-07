# VueUse M

版本：@vueuse/core 14.3.0；包括 core 对外重导出的 shared 可调用项。

## `makeDestructurable`

```ts
makeDestructurable<T extends Record<string, unknown>, A extends readonly any[]>(obj: T, arr: A): T & A
```

## `mapGamepadToXbox360Controller`

```ts
mapGamepadToXbox360Controller(gamepad: Ref<Gamepad | undefined>): _$vue.ComputedRef<{ buttons: { a: GamepadButton; b: GamepadButton; x: GamepadButton; y: GamepadButton; }; bumper: { left: GamepadButton; right: GamepadButton; }; triggers: { left: GamepadButton; right: GamepadButton; }; stick: { left: { horizontal: number; vertical: number; button: GamepadButton; }; right: { horizontal: number; vertical: number; button: GamepadButton; }; }; dpad: { up: GamepadButton; down: GamepadButton; left: GamepadButton; right: GamepadButton; }; back: GamepadButton; start: GamepadButton; } | null>
```
