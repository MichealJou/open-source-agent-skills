# cn.hutool.core.date.format

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.date.format.AbstractDateBasic` | `Locale getLocale()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.AbstractDateBasic` | `String getPattern()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.AbstractDateBasic` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.AbstractDateBasic` | `TimeZone getTimeZone()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.AbstractDateBasic` | `boolean equals(final Object obj)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.AbstractDateBasic` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.DateBasic` | `Locale getLocale()` | 获得 日期地理位置 |
| `cn.hutool.core.date.format.DateBasic` | `String getPattern()` | 获得日期格式化或者转换的格式 |
| `cn.hutool.core.date.format.DateBasic` | `TimeZone getTimeZone()` | 获得时区 |
| `cn.hutool.core.date.format.DateParser` | `Date parse(String source)` | 将日期字符串解析并转换为 Date 对象 等价于 java.text.DateFormat#parse(String) |
| `cn.hutool.core.date.format.DateParser` | `Date parse(String source,ParsePosition pos)` | 将日期字符串解析并转换为 Date 对象 等价于 java.text.DateFormat#parse(String, ParsePosition) |
| `cn.hutool.core.date.format.DateParser` | `Object parseObject(String source)` | 将日期字符串解析并转换为 Date 对象 |
| `cn.hutool.core.date.format.DateParser` | `Object parseObject(String source,ParsePosition pos)` | 根据 ParsePosition 给定将日期字符串解析并转换为 Date 对象 |
| `cn.hutool.core.date.format.DateParser` | `boolean parse(String source,ParsePosition pos,Calendar calendar)` | 根据给定格式更新Calendar Upon success, the ParsePosition index is updated to indicate how much of the source text was consumed. Not all source text needs to be consumed. Upon parse failure, ParsePosition error index is updated to the offset of the source text which does not match the supplied format. |
| `cn.hutool.core.date.format.DatePrinter` | `B format(Calendar calendar,B buf)` | 【原文待译】Formats a Calendar object into the supplied Appendable. The TimeZone set on the Calendar is only used to adjust the time offset. The TimeZone specified during the construction of the Parser will determine the TimeZone used in the formatted string. |
| `cn.hutool.core.date.format.DatePrinter` | `B format(Date date,B buf)` | 【原文待译】Formats a Date object into the supplied Appendable using a GregorianCalendar. |
| `cn.hutool.core.date.format.DatePrinter` | `B format(long millis,B buf)` | 【原文待译】Formats a millisecond long value into the supplied Appendable. |
| `cn.hutool.core.date.format.DatePrinter` | `String format(Calendar calendar)` | Formats a Calendar object. 格式化 Calendar |
| `cn.hutool.core.date.format.DatePrinter` | `String format(Date date)` | 使用 GregorianCalendar 格式化 Date |
| `cn.hutool.core.date.format.DatePrinter` | `String format(long millis)` | 格式化日期表示的毫秒数 |
| `cn.hutool.core.date.format.FastDateFormat` | `B format(final Calendar calendar,final B buf)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDateFormat` | `B format(final Date date,final B buf)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDateFormat` | `B format(final long millis,final B buf)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDateFormat` | `Date parse(final String source)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDateFormat` | `Date parse(final String source,final ParsePosition pos)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDateFormat` | `DateTimeFormatter getDateTimeFormatter()` | 便捷获取 DateTimeFormatter 由于 DatePattern 很大一部分的格式没有提供 DateTimeFormatter,因此这里提供快捷获取方式 |
| `cn.hutool.core.date.format.FastDateFormat` | `FastDateFormat getDateInstance(final int style)` | 获得 FastDateFormat 实例 支持缓存 |
| `cn.hutool.core.date.format.FastDateFormat` | `FastDateFormat getDateInstance(final int style,final Locale locale)` | 获得 FastDateFormat 实例 支持缓存 |
| `cn.hutool.core.date.format.FastDateFormat` | `FastDateFormat getDateInstance(final int style,final TimeZone timeZone)` | 获得 FastDateFormat 实例 支持缓存 |
| `cn.hutool.core.date.format.FastDateFormat` | `FastDateFormat getDateInstance(final int style,final TimeZone timeZone,final Locale locale)` | 获得 FastDateFormat 实例 支持缓存 |
| `cn.hutool.core.date.format.FastDateFormat` | `FastDateFormat getDateTimeInstance(final int dateStyle,final int timeStyle)` | 获得 FastDateFormat 实例 支持缓存 |
| `cn.hutool.core.date.format.FastDateFormat` | `FastDateFormat getDateTimeInstance(final int dateStyle,final int timeStyle,final Locale locale)` | 获得 FastDateFormat 实例 支持缓存 |
| `cn.hutool.core.date.format.FastDateFormat` | `FastDateFormat getDateTimeInstance(final int dateStyle,final int timeStyle,final TimeZone timeZone)` | 获得 FastDateFormat 实例 支持缓存 |
| `cn.hutool.core.date.format.FastDateFormat` | `FastDateFormat getDateTimeInstance(final int dateStyle,final int timeStyle,final TimeZone timeZone,final Locale locale)` | 获得 FastDateFormat 实例 支持缓存 |
| `cn.hutool.core.date.format.FastDateFormat` | `FastDateFormat getInstance()` | 获得 FastDateFormat实例，使用默认格式和地区 |
| `cn.hutool.core.date.format.FastDateFormat` | `FastDateFormat getInstance(final String pattern)` | 获得 FastDateFormat 实例，使用默认地区 支持缓存 |
| `cn.hutool.core.date.format.FastDateFormat` | `FastDateFormat getInstance(final String pattern,final Locale locale)` | 获得 FastDateFormat 实例 支持缓存 |
| `cn.hutool.core.date.format.FastDateFormat` | `FastDateFormat getInstance(final String pattern,final TimeZone timeZone)` | 获得 FastDateFormat 实例 支持缓存 |
| `cn.hutool.core.date.format.FastDateFormat` | `FastDateFormat getInstance(final String pattern,final TimeZone timeZone,final Locale locale)` | 获得 FastDateFormat 实例 支持缓存 |
| `cn.hutool.core.date.format.FastDateFormat` | `FastDateFormat getTimeInstance(final int style)` | 获得 FastDateFormat 实例 支持缓存 |
| `cn.hutool.core.date.format.FastDateFormat` | `FastDateFormat getTimeInstance(final int style,final Locale locale)` | 获得 FastDateFormat 实例 支持缓存 |
| `cn.hutool.core.date.format.FastDateFormat` | `FastDateFormat getTimeInstance(final int style,final TimeZone timeZone)` | 获得 FastDateFormat 实例 支持缓存 |
| `cn.hutool.core.date.format.FastDateFormat` | `FastDateFormat getTimeInstance(final int style,final TimeZone timeZone,final Locale locale)` | 获得 FastDateFormat 实例 支持缓存 |
| `cn.hutool.core.date.format.FastDateFormat` | `Locale getLocale()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDateFormat` | `Object parseObject(final String source,final ParsePosition pos)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDateFormat` | `String format(final Calendar calendar)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDateFormat` | `String format(final Date date)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDateFormat` | `String format(final long millis)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDateFormat` | `String getPattern()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDateFormat` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDateFormat` | `StringBuffer format(final Object obj,final StringBuffer toAppendTo,final FieldPosition pos)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDateFormat` | `TimeZone getTimeZone()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDateFormat` | `boolean equals(final Object obj)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDateFormat` | `boolean parse(final String source,final ParsePosition pos,final Calendar calendar)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDateFormat` | `int getMaxLengthEstimate()` | 估算生成的日期字符串长度 实际生成的字符串长度小于或等于此值 |
| `cn.hutool.core.date.format.FastDateFormat` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDateParser` | `Date parse(String source)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDateParser` | `Date parse(String source,ParsePosition pos)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDateParser` | `boolean parse(String source,ParsePosition pos,Calendar calendar)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDatePrinter` | `B format(Calendar calendar,B buf)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDatePrinter` | `B format(Date date,B buf)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDatePrinter` | `B format(long millis,B buf)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDatePrinter` | `String format(Calendar calendar)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDatePrinter` | `String format(Date date)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDatePrinter` | `String format(long millis)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.format.FastDatePrinter` | `int getMaxLengthEstimate()` | 估算生成的日期字符串长度 实际生成的字符串长度小于或等于此值 |
| `cn.hutool.core.date.format.GlobalCustomFormat` | `Date parse(CharSequence dateStr,String format)` | 使用自定义格式解析日期 |
| `cn.hutool.core.date.format.GlobalCustomFormat` | `String format(Date date,CharSequence format)` | 使用自定义格式格式化日期 |
| `cn.hutool.core.date.format.GlobalCustomFormat` | `String format(TemporalAccessor temporalAccessor,CharSequence format)` | 使用自定义格式格式化日期 |
| `cn.hutool.core.date.format.GlobalCustomFormat` | `boolean isCustomFormat(String format)` | 检查指定格式是否为自定义格式 |
| `cn.hutool.core.date.format.GlobalCustomFormat` | `void putFormatter(String format,Function<Date, String> func)` | 加入日期格式化规则 |
| `cn.hutool.core.date.format.GlobalCustomFormat` | `void putParser(String format,Function<CharSequence, Date> func)` | 加入日期解析规则 |
