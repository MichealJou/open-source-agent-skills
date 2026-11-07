# com.feilong.taglib.functions

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.taglib.functions.ELFunctions` | `String toJsonString(Object obj)` | 将对象format成json字符串(不会有pretty输出,会连在一起). 使用 indentFactor=0, indent=0 来格式化 |
| `com.feilong.taglib.functions.ELFunctions` | `boolean contains(Object collection,Object value)` | 用于 自定义标签/ 自定义el. 注意,比较的是 java.lang.Object#toString() |
