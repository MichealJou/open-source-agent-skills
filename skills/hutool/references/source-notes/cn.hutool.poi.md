# cn.hutool.poi

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.poi.GlobalPoiConfig` | `void setMaxEntrySize(final long maxEntrySize)` | 设置单个Zip文件中最大文件大小，默认为4GB，即32位zip格式的最大值。 |
| `cn.hutool.poi.GlobalPoiConfig` | `void setMaxTextSize(final long maxTextSize)` | 设置解压前文本的最大字符数，超过抛出异常。 |
| `cn.hutool.poi.GlobalPoiConfig` | `void setMinInflateRatio(final double ratio)` | 设置解压时的最小压缩比例 为了避免'Zip Bomb'，POI中设置了最小压缩比例，这个比例为： |
| `cn.hutool.poi.PoiChecker` | `void checkPoiImport()` | 检查POI包的引入情况 |
