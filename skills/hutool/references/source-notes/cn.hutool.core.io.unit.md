# cn.hutool.core.io.unit

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.io.unit.DataSize` | `DataSize of(BigDecimal amount,DataUnit unit)` | 获得指定DataUnit对应的DataSize |
| `cn.hutool.core.io.unit.DataSize` | `DataSize of(long amount,DataUnit unit)` | 获得指定DataUnit对应的DataSize |
| `cn.hutool.core.io.unit.DataSize` | `DataSize ofBytes(long bytes)` | 获得对应bytes的DataSize |
| `cn.hutool.core.io.unit.DataSize` | `DataSize ofGigabytes(long gigabytes)` | 获得对应gigabytes的DataSize |
| `cn.hutool.core.io.unit.DataSize` | `DataSize ofKilobytes(long kilobytes)` | 获得对应kilobytes的DataSize |
| `cn.hutool.core.io.unit.DataSize` | `DataSize ofMegabytes(long megabytes)` | 获得对应megabytes的DataSize |
| `cn.hutool.core.io.unit.DataSize` | `DataSize ofTerabytes(long terabytes)` | 获得对应terabytes的DataSize |
| `cn.hutool.core.io.unit.DataSize` | `DataSize parse(CharSequence text)` | 获取指定数据大小文本对应的DataSize对象，如果无单位指定，默认获取DataUnit#BYTES 例如： |
| `cn.hutool.core.io.unit.DataSize` | `DataSize parse(CharSequence text,DataUnit defaultUnit)` | 【原文待译】Obtain a DataSize from a text string such as 12MB using the specified default DataUnit if no unit is specified. The string starts with a number followed optionally by a unit matching one of the supported {@linkplain DataUnit suffixes}. Examples: |
| `cn.hutool.core.io.unit.DataSize` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.unit.DataSize` | `boolean equals(Object other)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.unit.DataSize` | `boolean isNegative()` | 是否为负数，不包括0 |
| `cn.hutool.core.io.unit.DataSize` | `int compareTo(DataSize other)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.unit.DataSize` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.unit.DataSize` | `long toBytes()` | 返回bytes大小 |
| `cn.hutool.core.io.unit.DataSize` | `long toGigabytes()` | 返回GB大小 |
| `cn.hutool.core.io.unit.DataSize` | `long toKilobytes()` | 返回KB大小 |
| `cn.hutool.core.io.unit.DataSize` | `long toMegabytes()` | 返回MB大小 |
| `cn.hutool.core.io.unit.DataSize` | `long toTerabytes()` | 返回TB大小 |
| `cn.hutool.core.io.unit.DataSizeUtil` | `String format(Long size,DataUnit fileDataUnit)` | 根据单位，将文件大小转换为对应单位的大小 |
| `cn.hutool.core.io.unit.DataSizeUtil` | `String format(long size)` | 可读的文件大小 参考 http://stackoverflow.com/questions/3263892/format-file-size-as-mb-gb-etc |
| `cn.hutool.core.io.unit.DataSizeUtil` | `long parse(String text)` | 解析数据大小字符串，转换为bytes大小 |
| `cn.hutool.core.io.unit.DataUnit` | `DataUnit fromSuffix(String suffix)` | 通过后缀返回对应的 DataUnit |
| `cn.hutool.core.io.unit.DataUnit` | `String getSuffix()` | 单位后缀 |
