# com.feilong.taglib.common

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.taglib.common.AbstractContainsSupport` | `boolean condition()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.taglib.common.AbstractContainsSupport` | `boolean containsByStringValue(Iterator<?> iterator,Object value)` | 迭代Iterator,判断元素的字符串格式是否和传入的值 value 的字符串格式相等. 注意,比较的是java.util.Objects#toString(Object, String),常用于自定义标签或者el function |
| `com.feilong.taglib.common.AbstractContainsSupport` | `void setCollection(Object collection)` | Sets the 一个集合,将会被转成Iterator,可以为逗号隔开的字符串,会被分隔成Iterator. |
| `com.feilong.taglib.common.AbstractContainsSupport` | `void setValue(Object value)` | Sets the 一个值. |
| `com.feilong.taglib.common.IsInTimeTag` | `boolean condition()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.taglib.common.IsInTimeTag` | `void setBeginDate(Date beginDate)` | Sets the 开始时间,beginDate和 beginDateString 二者只能选择其一. |
| `com.feilong.taglib.common.IsInTimeTag` | `void setBeginDateString(String beginDateString)` | Sets the 开始时间,beginDate和 beginDateString 二者只能选择其一. |
| `com.feilong.taglib.common.IsInTimeTag` | `void setDate(Date date)` | Sets the 一个时间,如果为null,则使用当前时间. |
| `com.feilong.taglib.common.IsInTimeTag` | `void setEndDate(Date endDate)` | Sets the 结束时间,endDate和 endDateString 二者只能选择其一. |
| `com.feilong.taglib.common.IsInTimeTag` | `void setEndDateString(String endDateString)` | Sets the 结束时间,endDate和 endDateString 二者只能选择其一. |
| `com.feilong.taglib.common.IsInTimeTag` | `void setPattern(String pattern)` | Sets the 如果 使用的 beginDateString 和 endDateString ,其format模式. |
| `com.feilong.taglib.common.IsNotContainsTag` | `boolean condition()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.taglib.common.SwitchCaseTag` | `int doStartTag()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.taglib.common.SwitchCaseTag` | `void setValue(String value)` | Sets the 值. |
| `com.feilong.taglib.common.SwitchDefaultTag` | `int doStartTag()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.taglib.common.SwitchTag` | `String getValue()` | 此处不可少 子标签调用. |
| `com.feilong.taglib.common.SwitchTag` | `boolean isExecuteTag()` | 该方法有子标签调用,表示是否可以执行自身的标签.. |
| `com.feilong.taglib.common.SwitchTag` | `int doStartTag()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.taglib.common.SwitchTag` | `void release()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.taglib.common.SwitchTag` | `void setExecuteTag()` | 标记执行了. |
| `com.feilong.taglib.common.SwitchTag` | `void setValue(String value)` | switch的值. |
