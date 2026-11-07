# cn.hutool.json.xml

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.json.xml.JSONXMLParser` | `void parseJSONObject(JSONObject jo,String xmlStr,boolean keepStrings)` | 转换XML为JSONObject 转换过程中一些信息可能会丢失，JSON中无法区分节点和属性，相同的节点将被处理为JSONArray。 |
| `cn.hutool.json.xml.JSONXMLParser` | `void parseJSONObject(final JSONObject jo,final String xmlStr,final ParseConfig parseConfig)` | 转换XML为JSONObject 转换过程中一些信息可能会丢失，JSON中无法区分节点和属性，相同的节点将被处理为JSONArray。 |
| `cn.hutool.json.xml.JSONXMLSerializer` | `String toXml(Object object)` | 转换JSONObject为XML Convert a JSONObject into a well-formed, element-normal XML string. |
| `cn.hutool.json.xml.JSONXMLSerializer` | `String toXml(Object object,String tagName)` | 转换JSONObject为XML |
| `cn.hutool.json.xml.JSONXMLSerializer` | `String toXml(Object object,String tagName,String... contentKeys)` | 转换JSONObject为XML |
| `cn.hutool.json.xml.ParseConfig` | `ParseConfig of()` | 创建ParseConfig |
| `cn.hutool.json.xml.ParseConfig` | `ParseConfig setKeepStrings(final boolean keepStrings)` | 设置是否保持值为String类型，如果为false，则尝试转换为对应类型(numeric, boolean, string) |
| `cn.hutool.json.xml.ParseConfig` | `ParseConfig setMaxNestingDepth(final int maxNestingDepth)` | 设置最大嵌套深度，用于解析时限制解析层级，当大于这个层级时抛出异常，-1表示无限制 |
| `cn.hutool.json.xml.ParseConfig` | `boolean isKeepStrings()` | 是否保持值为String类型，如果为false，则尝试转换为对应类型(numeric, boolean, string) |
| `cn.hutool.json.xml.ParseConfig` | `int getMaxNestingDepth()` | 获取最大嵌套深度，用于解析时限制解析层级，当大于这个层级时抛出异常，-1表示无限制 |
