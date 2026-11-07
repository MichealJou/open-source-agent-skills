# cn.hutool.json.serialize

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.json.serialize.GlobalSerializeMapping` | `JSONDeserializer<?> getDeserializer(Type type)` | 获取自定义的反序列化器，如果未定义返回null |
| `cn.hutool.json.serialize.GlobalSerializeMapping` | `JSONSerializer<? extends JSON, ?> getSerializer(Type type)` | 获取自定义的序列化器，如果未定义返回null |
| `cn.hutool.json.serialize.GlobalSerializeMapping` | `void put(Type type,JSONArraySerializer<?> serializer)` | 加入自定义的序列化器 |
| `cn.hutool.json.serialize.GlobalSerializeMapping` | `void put(Type type,JSONDeserializer<?> deserializer)` | 加入自定义的反序列化器 |
| `cn.hutool.json.serialize.GlobalSerializeMapping` | `void put(Type type,JSONObjectSerializer<?> serializer)` | 加入自定义的序列化器 |
| `cn.hutool.json.serialize.JSONDeserializer` | `T deserialize(JSON json)` | 反序列化，通过实现此方法，自定义实现JSON转换为指定类型的逻辑 |
| `cn.hutool.json.serialize.JSONSerializer` | `void serialize(T json,V bean)` | 序列化实现，通过实现此方法，将指定类型的对象转换为JSON对象 转换后的对象可以为JSONObject也可以为JSONArray，首先new一个空的JSON，然后将需要的数据字段put到JSON对象中去即可。 |
| `cn.hutool.json.serialize.JSONWriter` | `JSONWriter beginArray()` | JSONArray写出开始，默认写出"[" |
| `cn.hutool.json.serialize.JSONWriter` | `JSONWriter beginObj()` | JSONObject写出开始，默认写出"{" |
| `cn.hutool.json.serialize.JSONWriter` | `JSONWriter end()` | 结束，默认根据开始的类型，补充"}"或"]" |
| `cn.hutool.json.serialize.JSONWriter` | `JSONWriter of(Writer writer,int indentFactor,int indent,JSONConfig config)` | 创建JSONWriter |
| `cn.hutool.json.serialize.JSONWriter` | `JSONWriter writeField(MutablePair<Object, Object> pair,Filter<MutablePair<Object, Object>> filter)` | 写出字段名及字段值，如果字段值是null且忽略null值，则不写出任何内容 |
| `cn.hutool.json.serialize.JSONWriter` | `JSONWriter writeField(String key,Object value)` | 写出字段名及字段值，如果字段值是null且忽略null值，则不写出任何内容 |
| `cn.hutool.json.serialize.JSONWriter` | `JSONWriter writeKey(String key)` | 写出键，自动处理分隔符和缩进，并包装键名 |
| `cn.hutool.json.serialize.JSONWriter` | `JSONWriter writeValue(Object value)` | 写出值，自动处理分隔符和缩进，自动判断类型，并根据不同类型写出特定格式的值 如果写出的值为null或者JSONNull，且配置忽略null，则跳过。 |
| `cn.hutool.json.serialize.JSONWriter` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.serialize.JSONWriter` | `void flush()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.serialize.JSONWriter` | `void write(char[] cbuf,int off,int len)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.serialize.TemporalAccessorSerializer` | `TemporalAccessor deserialize(JSON json)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.serialize.TemporalAccessorSerializer` | `void serialize(JSONObject json,TemporalAccessor bean)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
