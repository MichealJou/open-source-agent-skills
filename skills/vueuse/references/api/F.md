# VueUse F

版本：@vueuse/core 14.3.0；包括 core 对外重导出的 shared 可调用项。

## `formatDate`

```ts
formatDate(date: Date, formatStr: string, options?: UseDateFormatOptions): string
```

## `formatTimeAgo`

```ts
formatTimeAgo<UnitNames extends string = UseTimeAgoUnitNamesDefault>(from: Date, options?: FormatTimeAgoOptions<UnitNames>, now?: Date | number): string
```

## `formatTimeAgoIntl`

```ts
formatTimeAgoIntl(from: Date, options?: FormatTimeAgoIntlOptions, now?: Date | number): string
```

## `formatTimeAgoIntlParts`

```ts
formatTimeAgoIntlParts(parts: Intl.RelativeTimeFormatPart[], options?: FormatTimeAgoIntlOptions): string
```
