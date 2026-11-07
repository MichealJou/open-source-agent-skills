# cn.hutool.json

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.json.InternalJSONUtil` | `Object stringToValue(String string)` | 尝试转换字符串为number, boolean, or null，无法转换返回String |
| `cn.hutool.json.JSON` | `JSONConfig getConfig()` | 获取JSON配置 |
| `cn.hutool.json.JSON` | `Object getByPath(String expression)` | 通过表达式获取JSON中嵌套的对象 .表达式，可以获取Bean对象中的属性（字段）值或者Map中key对应的值 []表达式，可以获取集合等对象中对应index的值 表达式栗子： |
| `cn.hutool.json.JSON` | `String toJSONString(int indentFactor)` | 格式化输出JSON字符串 |
| `cn.hutool.json.JSON` | `String toStringPretty()` | 格式化打印JSON，缩进为4个空格 |
| `cn.hutool.json.JSON` | `T getByPath(String expression,Class<T> resultType)` | 通过表达式获取JSON中嵌套的对象 .表达式，可以获取Bean对象中的属性（字段）值或者Map中key对应的值 []表达式，可以获取集合等对象中对应index的值 表达式栗子： |
| `cn.hutool.json.JSON` | `T getByPath(String expression,TypeReference<T> targetType)` | 通过表达式获取JSON中嵌套的对象 .表达式，可以获取Bean对象中的属性（字段）值或者Map中key对应的值 []表达式，可以获取集合等对象中对应index的值 表达式栗子： |
| `cn.hutool.json.JSON` | `T toBean(Class<T> clazz)` | 转为实体类对象，转换异常将被抛出 |
| `cn.hutool.json.JSON` | `T toBean(Type type)` | 转为实体类对象 |
| `cn.hutool.json.JSON` | `T toBean(Type type,boolean ignoreError)` | 转为实体类对象 |
| `cn.hutool.json.JSON` | `T toBean(TypeReference<T> reference)` | 转为实体类对象，转换异常将被抛出 |
| `cn.hutool.json.JSON` | `Writer write(Writer writer)` | 将JSON内容写入Writer，无缩进 Warning: This method assumes that the data structure is acyclical. |
| `cn.hutool.json.JSON` | `Writer write(Writer writer,int indentFactor,int indent)` | 将JSON内容写入Writer Warning: This method assumes that the data structure is acyclical. |
| `cn.hutool.json.JSON` | `void putByPath(String expression,Object value)` | 设置表达式指定位置（或filed对应）的值 若表达式指向一个JSONArray则设置其坐标对应位置的值，若指向JSONObject则put对应key的值 注意：如果为JSONArray，设置值下标小于其长度，将替换原有值，否则追加新值 .表达式，可以获取Bean对象中的属性（字段）值或者Map中key对应的值 []表达式，可以获取集合等对象中对应index的值 表达式栗子： |
| `cn.hutool.json.JSONArray` | `Iterable<JSONObject> jsonIter()` | 当此JSON列表的每个元素都是一个JSONObject时，可以调用此方法返回一个Iterable，便于使用foreach语法遍历 |
| `cn.hutool.json.JSONArray` | `Iterator<Object> iterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `JSONArray put(Object value)` | Append an object value. This increases the array's length by one. 加入元素，数组长度+1，等同于 JSONArray#add(Object) |
| `cn.hutool.json.JSONArray` | `JSONArray put(int index,Object value)` | 加入或者替换JSONArray中指定Index的值，如果index大于JSONArray的长度，将在指定index设置值，之前的位置填充JSONNull.Null |
| `cn.hutool.json.JSONArray` | `JSONArray set(Object value)` | Append an object value. This increases the array's length by one. 加入元素，数组长度+1，等同于 JSONArray#add(Object) |
| `cn.hutool.json.JSONArray` | `JSONArray setDateFormat(String format)` | 设置转为字符串时的日期格式，默认为时间戳（null值） |
| `cn.hutool.json.JSONArray` | `JSONConfig getConfig()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `JSONObject toJSONObject(JSONArray names)` | 根据给定名列表，与其位置对应的值组成JSONObject |
| `cn.hutool.json.JSONArray` | `List<Object> subList(int fromIndex,int toIndex)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `List<T> toList(Class<T> elementType)` | 转为ArrayList |
| `cn.hutool.json.JSONArray` | `ListIterator<Object> listIterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `ListIterator<Object> listIterator(int index)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `Object clone()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `Object get(int index)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `Object getByPath(String expression)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `Object getObj(Integer index,Object defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `Object remove(int index)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `Object set(int index,Object element)` | 加入或者替换JSONArray中指定Index的值，如果index大于JSONArray的长度，将在指定index设置值，之前的位置填充JSONNull.Null |
| `cn.hutool.json.JSONArray` | `Object set(int index,Object element,Filter<MutablePair<Integer, Object>> filter)` | 加入或者替换JSONArray中指定Index的值，如果index大于JSONArray的长度，将在指定index设置值，之前的位置填充JSONNull.Null |
| `cn.hutool.json.JSONArray` | `Object toArray(Class<?> arrayClass)` | 转为Bean数组 |
| `cn.hutool.json.JSONArray` | `Object[] toArray()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `String join(String separator)` | JSONArray转为以separator为分界符的字符串 |
| `cn.hutool.json.JSONArray` | `String toJSONString(int indentFactor,Filter<MutablePair<Object, Object>> filter)` | 返回JSON字符串 支持过滤器，即选择哪些字段或值不写出 |
| `cn.hutool.json.JSONArray` | `String toString()` | 转为JSON字符串，无缩进 |
| `cn.hutool.json.JSONArray` | `T getByPath(String expression,Class<T> resultType)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `T getByPath(String expression,TypeReference<T> targetType)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `T[] toArray(T[] a)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `Writer write(Writer writer,int indentFactor,int indent)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `Writer write(Writer writer,int indentFactor,int indent,Filter<MutablePair<Object, Object>> filter)` | 将JSON内容写入Writer 支持过滤器，即选择哪些字段或值不写出 |
| `cn.hutool.json.JSONArray` | `boolean add(Object e)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `boolean addAll(Collection<?> c)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `boolean addAll(int index,Collection<?> c)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `boolean contains(Object o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `boolean containsAll(Collection<?> c)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `boolean equals(Object obj)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `boolean isEmpty()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `boolean remove(Object o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `boolean removeAll(Collection<?> c)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `boolean retainAll(Collection<?> c)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `int indexOf(Object o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `int lastIndexOf(Object o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `int size()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `void add(int index,Object element)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `void clear()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONArray` | `void putByPath(String expression,Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONBeanParser` | `void parse(T value)` | value转Bean 通过实现此接口，将JSON中的值填充到当前对象的字段值中，即对象自行实现JSON反序列化逻辑 |
| `cn.hutool.json.JSONConfig` | `Comparator<String> getKeyComparator()` | 获取键排序规则 键排序规则，null表示不排序，不排序情况下，按照加入顺序排序 |
| `cn.hutool.json.JSONConfig` | `JSONConfig create()` | 创建默认的配置项 |
| `cn.hutool.json.JSONConfig` | `JSONConfig setCheckDuplicate(boolean checkDuplicate)` | 是否检查多个相同的key |
| `cn.hutool.json.JSONConfig` | `JSONConfig setDateFormat(String dateFormat)` | 设置日期格式，null表示默认的时间戳 此方法设置的日期格式仅对转换为JSON字符串有效，对解析JSON为bean无效。 |
| `cn.hutool.json.JSONConfig` | `JSONConfig setIgnoreCase(boolean ignoreCase)` | 设置是否忽略键的大小写 |
| `cn.hutool.json.JSONConfig` | `JSONConfig setIgnoreError(boolean ignoreError)` | 设置是否忽略转换过程中的异常 |
| `cn.hutool.json.JSONConfig` | `JSONConfig setIgnoreNullValue(boolean ignoreNullValue)` | 设置是否忽略null值 |
| `cn.hutool.json.JSONConfig` | `JSONConfig setKeyComparator(Comparator<String> keyComparator)` | 设置键排序规则 键排序规则，null表示不排序，不排序情况下，按照加入顺序排序 |
| `cn.hutool.json.JSONConfig` | `JSONConfig setNatureKeyComparator()` | 设置自然排序，即按照字母顺序排序 |
| `cn.hutool.json.JSONConfig` | `JSONConfig setOrder(boolean order)` | 设置是否有序，顺序按照加入顺序排序，只针对JSONObject有效 |
| `cn.hutool.json.JSONConfig` | `JSONConfig setStripTrailingZeros(boolean stripTrailingZeros)` | 设置是否去除末尾多余0，例如如果为true,5.0返回5 |
| `cn.hutool.json.JSONConfig` | `JSONConfig setTransientSupport(boolean transientSupport)` | 设置是否支持transient关键字修饰和@Transient注解，如果支持，被修饰的字段或方法对应的字段将被忽略。 |
| `cn.hutool.json.JSONConfig` | `JSONConfig setWriteLongAsString(boolean writeLongAsString)` | 设置是否将Long值写出为字符串类型 |
| `cn.hutool.json.JSONConfig` | `String getDateFormat()` | 日期格式，null表示默认的时间戳 |
| `cn.hutool.json.JSONConfig` | `boolean isCheckDuplicate()` | 是否检查多个相同的key |
| `cn.hutool.json.JSONConfig` | `boolean isIgnoreCase()` | 是否忽略键的大小写 |
| `cn.hutool.json.JSONConfig` | `boolean isIgnoreError()` | 是否忽略转换过程中的异常 |
| `cn.hutool.json.JSONConfig` | `boolean isIgnoreNullValue()` | 是否忽略null值 |
| `cn.hutool.json.JSONConfig` | `boolean isOrder()` | 是否有序，顺序按照加入顺序排序，只针对JSONObject有效 |
| `cn.hutool.json.JSONConfig` | `boolean isStripTrailingZeros()` | 是否去除末尾多余0，例如如果为true,5.0返回5 |
| `cn.hutool.json.JSONConfig` | `boolean isTransientSupport()` | 是否支持transient关键字修饰和@Transient注解，如果支持，被修饰的字段或方法对应的字段将被忽略。 |
| `cn.hutool.json.JSONConfig` | `boolean isWriteLongAsString()` | 是否将Long值写出为字符串类型 |
| `cn.hutool.json.JSONConverter` | `JSON convert(Object value,JSON defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONGetter` | `Date getDate(K key,Date defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONGetter` | `JSONArray getJSONArray(K key)` | 获得JSONArray对象 如果值为其它类型对象，尝试转换为JSONArray返回，否则抛出异常 |
| `cn.hutool.json.JSONGetter` | `JSONConfig getConfig()` | 获取JSON配置 |
| `cn.hutool.json.JSONGetter` | `JSONObject getJSONObject(K key)` | 获得JSONObject对象 如果值为其它类型对象，尝试转换为JSONObject返回，否则抛出异常 |
| `cn.hutool.json.JSONGetter` | `List<T> getBeanList(K key,Class<T> beanType)` | 从JSON中直接获取Bean的List列表 先获取JSONArray对象，然后转为Bean的List |
| `cn.hutool.json.JSONGetter` | `LocalDateTime getLocalDateTime(K key,LocalDateTime defaultValue)` | 获取LocalDateTime类型值 |
| `cn.hutool.json.JSONGetter` | `String getStrEscaped(K key)` | 获取字符串类型值，并转义不可见字符，如'\n'换行符会被转义为字符串"\n" |
| `cn.hutool.json.JSONGetter` | `String getStrEscaped(K key,String defaultValue)` | 获取字符串类型值，并转义不可见字符，如'\n'换行符会被转义为字符串"\n" |
| `cn.hutool.json.JSONGetter` | `T get(K key,Class<T> type)` | 获取指定类型的对象 转换失败或抛出异常 |
| `cn.hutool.json.JSONGetter` | `T get(K key,Class<T> type,boolean ignoreError)` | 获取指定类型的对象 |
| `cn.hutool.json.JSONGetter` | `T getBean(K key,Class<T> beanType)` | 从JSON中直接获取Bean对象 先获取JSONObject对象，然后转为Bean对象 |
| `cn.hutool.json.JSONGetter` | `boolean isNull(K key)` | key对应值是否为null或无此key |
| `cn.hutool.json.JSONGetter` | `byte[] getBytes(K key)` | 获取byte[]数据 |
| `cn.hutool.json.JSONNull` | `String toString()` | Get the "null" string value. 获得“null”字符串 |
| `cn.hutool.json.JSONNull` | `boolean equals(Object object)` | A Null object is equal to the null value and to itself. 对象与其本身和null值相等 |
| `cn.hutool.json.JSONObject` | `JSONArray toJSONArray(Collection<String> names)` | 将指定KEY列表的值组成新的JSONArray |
| `cn.hutool.json.JSONObject` | `JSONConfig getConfig()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONObject` | `JSONObject accumulate(String key,Object value)` | 积累值。类似于set，当key对应value已经存在时，与value组成新的JSONArray. 如果只有一个值，此值就是value，如果多个值，则是添加到新的JSONArray中 |
| `cn.hutool.json.JSONObject` | `JSONObject append(String key,Object value)` | 追加值，如果key无对应值，就添加一个JSONArray，其元素只有value，如果值已经是一个JSONArray，则添加到值JSONArray中。 |
| `cn.hutool.json.JSONObject` | `JSONObject clone()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONObject` | `JSONObject increment(String key)` | 对值加一，如果值不存在，赋值1，如果为数字类型，做加一操作 |
| `cn.hutool.json.JSONObject` | `JSONObject put(String key,Object value)` | PUT 键值对到JSONObject中，在忽略null模式下，如果值为null，将此键移除 |
| `cn.hutool.json.JSONObject` | `JSONObject putOnce(String key,Object value)` | 一次性Put 键值对，如果key已经存在抛出异常，如果键值中有null值，忽略 |
| `cn.hutool.json.JSONObject` | `JSONObject putOpt(String key,Object value)` | 在键和值都为非空的情况下put到JSONObject中 |
| `cn.hutool.json.JSONObject` | `JSONObject set(String key,Object value)` | 设置键值对到JSONObject中，在忽略null模式下，如果值为null，将此键移除 |
| `cn.hutool.json.JSONObject` | `JSONObject set(String key,Object value,Filter<MutablePair<String, Object>> filter,boolean checkDuplicate)` | 设置键值对到JSONObject中，在忽略null模式下，如果值为null，将此键移除 |
| `cn.hutool.json.JSONObject` | `JSONObject setDateFormat(String format)` | 设置转为字符串时的日期格式，默认为时间戳（null值） 此方法设置的日期格式仅对转换为JSON字符串有效，对解析JSON为bean无效。 |
| `cn.hutool.json.JSONObject` | `JSONObject setOnce(String key,Object value,Filter<MutablePair<String, Object>> filter)` | 一次性Put 键值对，如果key已经存在抛出异常，如果键值中有null值，忽略 |
| `cn.hutool.json.JSONObject` | `Object getByPath(String expression)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONObject` | `Object getObj(String key,Object defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONObject` | `String toJSONString(int indentFactor,Filter<MutablePair<Object, Object>> filter)` | 返回JSON字符串 支持过滤器，即选择哪些字段或值不写出 |
| `cn.hutool.json.JSONObject` | `String toString()` | 返回JSON字符串 如果解析错误，返回null |
| `cn.hutool.json.JSONObject` | `T getByPath(String expression,Class<T> resultType)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONObject` | `T getByPath(String expression,TypeReference<T> targetType)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONObject` | `Writer write(Writer writer,int indentFactor,int indent)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONObject` | `Writer write(Writer writer,int indentFactor,int indent,Filter<MutablePair<Object, Object>> filter)` | 将JSON内容写入Writer 支持过滤器，即选择哪些字段或值不写出 |
| `cn.hutool.json.JSONObject` | `void putAll(Map<? extends String, ?> m)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONObject` | `void putByPath(String expression,Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONObjectIter` | `Iterator<JSONObject> iterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONParser` | `JSONParser of(JSONTokener tokener)` | 创建JSONParser |
| `cn.hutool.json.JSONParser` | `void parseTo(JSONArray jsonArray,Filter<Mutable<Object>> filter)` | 解析JSON字符串到JSONArray中 |
| `cn.hutool.json.JSONParser` | `void parseTo(JSONObject jsonObject,Filter<MutablePair<String, Object>> filter)` | 解析JSONTokener中的字符到目标的JSONObject中 |
| `cn.hutool.json.JSONStrFormatter` | `String format(String json)` | 返回格式化JSON字符串。 |
| `cn.hutool.json.JSONString` | `String toJSONString()` | 自定义转JSON字符串的方法 |
| `cn.hutool.json.JSONSupport` | `JSONObject toJSON()` | @return JSON对象 |
| `cn.hutool.json.JSONSupport` | `String toJSONString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONSupport` | `String toPrettyString()` | 美化的JSON（使用回车缩进显示JSON），用于打印输出debug |
| `cn.hutool.json.JSONSupport` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.json.JSONSupport` | `void parse(JSON json)` | JSON转Bean |
| `cn.hutool.json.JSONSupport` | `void parse(String jsonString)` | JSON String转Bean |
| `cn.hutool.json.JSONTokener` | `JSONArray toJSONArray()` | 转为 JSONArray |
| `cn.hutool.json.JSONTokener` | `JSONException syntaxError(String message)` | Make a JSONException to signal a syntax error. 构建 JSONException 用于表示语法错误 |
| `cn.hutool.json.JSONTokener` | `Object nextValue()` | 获得下一个值，值类型可以是Boolean, Double, Integer, JSONArray, JSONObject, Long, or String, or the JSONObject.NULL |
| `cn.hutool.json.JSONTokener` | `String next(int n)` | 获得接下来的n个字符 |
| `cn.hutool.json.JSONTokener` | `String nextString(char quote)` | 返回当前位置到指定引号前的所有字符，反斜杠的转义符也会被处理。 标准的JSON是不允许使用单引号包含字符串的，但是此实现允许。 |
| `cn.hutool.json.JSONTokener` | `String nextStringValue()` | 获取下一个String格式的值，用户获取key |
| `cn.hutool.json.JSONTokener` | `String nextTo(String delimiters)` | 【原文待译】Get the text up but not including one of the specified delimiter characters or the end of line, whichever comes first. |
| `cn.hutool.json.JSONTokener` | `String nextTo(char delimiter)` | Get the text up but not including the specified character or the end of line, whichever comes first. 获得从当前位置直到分隔符（不包括分隔符）或行尾的的所有字符。 |
| `cn.hutool.json.JSONTokener` | `String toString()` | 【原文待译】Make a printable string of this JSONTokener. |
| `cn.hutool.json.JSONTokener` | `boolean end()` | @return 是否进入结尾 |
| `cn.hutool.json.JSONTokener` | `boolean more()` | 源字符串是否有更多的字符 |
| `cn.hutool.json.JSONTokener` | `char next()` | 获得源字符串中的下一个字符 |
| `cn.hutool.json.JSONTokener` | `char next(char c)` | 读取下一个字符，并比对是否和指定字符匹配 |
| `cn.hutool.json.JSONTokener` | `char nextClean()` | 获得下一个字符，跳过空白符 |
| `cn.hutool.json.JSONTokener` | `char skipTo(char to)` | Skip characters until the next character is the requested character. If the requested character is not found, no characters are skipped. 在遇到指定字符前，跳过其它字符。如果字符未找到，则不跳过任何字符。 |
| `cn.hutool.json.JSONTokener` | `void back()` | 将标记回退到第一个字符，重新开始解析新的JSON |
| `cn.hutool.json.JSONUtil` | `JSON parse(Object obj)` | 转换对象为JSON，如果用户不配置JSONConfig，则JSON的有序与否与传入对象有关。 支持的对象： String: 转换为相应的对象 Array、Iterable、Iterator：转换为JSONArray Bean对象：转为JSONObject |
| `cn.hutool.json.JSONUtil` | `JSON parse(Object obj,JSONConfig config)` | 转换对象为JSON，如果用户不配置JSONConfig，则JSON的有序与否与传入对象有关。 支持的对象： String: 转换为相应的对象 Array、Iterable、Iterator：转换为JSONArray Bean对象：转为JSONObject |
| `cn.hutool.json.JSONUtil` | `JSON readJSON(File file,Charset charset)` | 读取JSON |
| `cn.hutool.json.JSONUtil` | `JSONArray createArray()` | 创建 JSONArray |
| `cn.hutool.json.JSONUtil` | `JSONArray createArray(JSONConfig config)` | 创建 JSONArray |
| `cn.hutool.json.JSONUtil` | `JSONArray parseArray(Object arrayOrCollection)` | JSON字符串转JSONArray |
| `cn.hutool.json.JSONUtil` | `JSONArray parseArray(Object arrayOrCollection,JSONConfig config)` | JSON字符串转JSONArray |
| `cn.hutool.json.JSONUtil` | `JSONArray parseArray(Object arrayOrCollection,boolean ignoreNullValue)` | JSON字符串转JSONArray |
| `cn.hutool.json.JSONUtil` | `JSONArray parseArray(String jsonStr)` | JSON字符串转JSONArray |
| `cn.hutool.json.JSONUtil` | `JSONArray readJSONArray(File file,Charset charset)` | 读取JSONArray |
| `cn.hutool.json.JSONUtil` | `JSONObject createObj()` | 创建JSONObject |
| `cn.hutool.json.JSONUtil` | `JSONObject createObj(JSONConfig config)` | 创建JSONObject |
| `cn.hutool.json.JSONUtil` | `JSONObject parseFromXml(String xmlStr)` | XML字符串转为JSONObject |
| `cn.hutool.json.JSONUtil` | `JSONObject parseObj(Object obj)` | JSON字符串转JSONObject对象 此方法会忽略空值，但是对JSON字符串不影响 |
| `cn.hutool.json.JSONUtil` | `JSONObject parseObj(Object obj,JSONConfig config)` | JSON字符串转JSONObject对象 此方法会忽略空值，但是对JSON字符串不影响 |
| `cn.hutool.json.JSONUtil` | `JSONObject parseObj(Object obj,boolean ignoreNullValue)` | JSON字符串转JSONObject对象 |
| `cn.hutool.json.JSONUtil` | `JSONObject parseObj(Object obj,boolean ignoreNullValue,boolean isOrder)` | JSON字符串转JSONObject对象 |
| `cn.hutool.json.JSONUtil` | `JSONObject parseObj(String jsonStr)` | JSON字符串转JSONObject对象 |
| `cn.hutool.json.JSONUtil` | `JSONObject readJSONObject(File file,Charset charset)` | 读取JSONObject |
| `cn.hutool.json.JSONUtil` | `JSONObject xmlToJson(String xml)` | XML转JSONObject 转换过程中一些信息可能会丢失，JSON中无法区分节点和属性，相同的节点将被处理为JSONArray。 |
| `cn.hutool.json.JSONUtil` | `List<T> toList(JSONArray jsonArray,Class<T> elementType)` | 将JSONArray转换为Bean的List，默认为ArrayList |
| `cn.hutool.json.JSONUtil` | `List<T> toList(String jsonArray,Class<T> elementType)` | 将JSONArray字符串转换为Bean的List，默认为ArrayList |
| `cn.hutool.json.JSONUtil` | `Object getByPath(JSON json,String expression)` | 通过表达式获取JSON中嵌套的对象 .表达式，可以获取Bean对象中的属性（字段）值或者Map中key对应的值 []表达式，可以获取集合等对象中对应index的值 表达式栗子： |
| `cn.hutool.json.JSONUtil` | `Object wrap(Object object,JSONConfig jsonConfig)` | 在需要的时候包装对象 包装包括： null =》 JSONNull.NULL array or collection =》 JSONArray map =》 JSONObject standard property (Double, String, et al) =》 原对象 来自于java包 =》 字符串 其它 =》 尝试包装为JSONObject，如果JSONConfig#isIgnoreError()为true时返回null, 否则抛出异常 |
| `cn.hutool.json.JSONUtil` | `String escape(String str)` | 转义显示不可见字符 |
| `cn.hutool.json.JSONUtil` | `String formatJsonStr(String jsonStr)` | 格式化JSON字符串，此方法并不严格检查JSON的格式正确与否 |
| `cn.hutool.json.JSONUtil` | `String quote(String string)` | 对所有双引号做转义处理（使用双反斜杠做转义） 为了能在HTML中较好的显示，会将</转义为<\/ JSON字符串中不能包含控制字符和未经转义的引号和反斜杠 |
| `cn.hutool.json.JSONUtil` | `String quote(String string,boolean isWrap)` | 对所有双引号做转义处理（使用双反斜杠做转义） 为了能在HTML中较好的显示，会将</转义为<\/ JSON字符串中不能包含控制字符和未经转义的引号和反斜杠 |
| `cn.hutool.json.JSONUtil` | `String toJsonPrettyStr(JSON json)` | 转为JSON字符串 |
| `cn.hutool.json.JSONUtil` | `String toJsonPrettyStr(Object obj)` | 转换为格式化后的JSON字符串 |
| `cn.hutool.json.JSONUtil` | `String toJsonStr(JSON json)` | 转为JSON字符串 |
| `cn.hutool.json.JSONUtil` | `String toJsonStr(JSON json,int indentFactor)` | 转为JSON字符串 |
| `cn.hutool.json.JSONUtil` | `String toJsonStr(Object obj)` | 转换为JSON字符串 |
| `cn.hutool.json.JSONUtil` | `String toJsonStr(Object obj,JSONConfig jsonConfig)` | 转换为JSON字符串 |
| `cn.hutool.json.JSONUtil` | `String toXmlStr(JSON json)` | 转换为XML字符串 |
| `cn.hutool.json.JSONUtil` | `T getByPath(JSON json,String expression,T defaultValue)` | 通过表达式获取JSON中嵌套的对象 .表达式，可以获取Bean对象中的属性（字段）值或者Map中key对应的值 []表达式，可以获取集合等对象中对应index的值 表达式栗子： |
| `cn.hutool.json.JSONUtil` | `T toBean(JSON json,Type beanType,boolean ignoreError)` | 转为实体类对象 |
| `cn.hutool.json.JSONUtil` | `T toBean(JSON json,TypeReference<T> typeReference,boolean ignoreError)` | 转为实体类对象 |
| `cn.hutool.json.JSONUtil` | `T toBean(JSONObject json,Class<T> beanClass)` | 转为实体类对象，转换异常将被抛出 |
| `cn.hutool.json.JSONUtil` | `T toBean(String jsonString,Class<T> beanClass)` | JSON字符串转为实体类对象，转换异常将被抛出 |
| `cn.hutool.json.JSONUtil` | `T toBean(String jsonString,JSONConfig config,Class<T> beanClass)` | JSON字符串转为实体类对象，转换异常将被抛出 通过JSONConfig可选是否忽略大小写、忽略null等配置 |
| `cn.hutool.json.JSONUtil` | `T toBean(String jsonString,Type beanType,boolean ignoreError)` | JSON字符串转为实体类对象，转换异常将被抛出 |
| `cn.hutool.json.JSONUtil` | `T toBean(String jsonString,TypeReference<T> typeReference,boolean ignoreError)` | JSON字符串转为实体类对象，转换异常将被抛出 |
| `cn.hutool.json.JSONUtil` | `Writer quote(String str,Writer writer)` | 对所有双引号做转义处理（使用双反斜杠做转义） 为了能在HTML中较好的显示，会将</转义为<\/ JSON字符串中不能包含控制字符和未经转义的引号和反斜杠 |
| `cn.hutool.json.JSONUtil` | `Writer quote(String str,Writer writer,boolean isWrap)` | 对所有双引号做转义处理（使用双反斜杠做转义） 为了能在HTML中较好的显示，会将</转义为<\/ JSON字符串中不能包含控制字符和未经转义的引号和反斜杠 |
| `cn.hutool.json.JSONUtil` | `boolean isJson(String str)` | 是否为JSON字符串，首尾都为大括号或中括号判定为JSON字符串 |
| `cn.hutool.json.JSONUtil` | `boolean isJsonArray(String str)` | 是否为JSONArray字符串，首尾都为中括号判定为JSONArray字符串 |
| `cn.hutool.json.JSONUtil` | `boolean isJsonObj(String str)` | 是否为JSONObject字符串，首尾都为大括号判定为JSONObject字符串 |
| `cn.hutool.json.JSONUtil` | `boolean isNull(Object obj)` | 是否为null对象，null的情况包括： |
| `cn.hutool.json.JSONUtil` | `boolean isTypeJSON(String str)` | 是否为JSON类型字符串，首尾都为大括号或中括号判定为JSON字符串 |
| `cn.hutool.json.JSONUtil` | `boolean isTypeJSONArray(String str)` | 是否为JSONArray类型的字符串，首尾都为中括号判定为JSONArray字符串 |
| `cn.hutool.json.JSONUtil` | `boolean isTypeJSONObject(String str)` | 是否为JSONObject类型字符串，首尾都为大括号判定为JSONObject字符串 |
| `cn.hutool.json.JSONUtil` | `void putByPath(JSON json,String expression,Object value)` | 设置表达式指定位置（或filed对应）的值 若表达式指向一个JSONArray则设置其坐标对应位置的值，若指向JSONObject则put对应key的值 注意：如果为JSONArray，则设置值得下标不能大于已有JSONArray的长度 .表达式，可以获取Bean对象中的属性（字段）值或者Map中key对应的值 []表达式，可以获取集合等对象中对应index的值 表达式栗子： |
| `cn.hutool.json.JSONUtil` | `void putDeserializer(Type type,JSONDeserializer<?> deserializer)` | 加入自定义的反序列化器 |
| `cn.hutool.json.JSONUtil` | `void putSerializer(Type type,JSONArraySerializer<?> serializer)` | 加入自定义的序列化器 |
| `cn.hutool.json.JSONUtil` | `void putSerializer(Type type,JSONObjectSerializer<?> serializer)` | 加入自定义的序列化器 |
| `cn.hutool.json.JSONUtil` | `void toJsonStr(JSON json,Writer writer)` | 转为JSON字符串，并写出到write |
| `cn.hutool.json.JSONUtil` | `void toJsonStr(Object obj,Writer writer)` | 转换为JSON字符串并写出到writer |
| `cn.hutool.json.ObjectMapper` | `ObjectMapper of(Object source)` | 创建ObjectMapper |
| `cn.hutool.json.ObjectMapper` | `void map(JSONArray jsonArray,Filter<Mutable<Object>> filter)` | 初始化 |
| `cn.hutool.json.ObjectMapper` | `void map(JSONObject jsonObject,Filter<MutablePair<String, Object>> filter)` | 将给定对象转换为JSONObject |
| `cn.hutool.json.XML` | `JSONObject toJSONObject(JSONObject jo,String xmlStr,boolean keepStrings)` | 转换XML为JSONObject 转换过程中一些信息可能会丢失，JSON中无法区分节点和属性，相同的节点将被处理为JSONArray。 |
| `cn.hutool.json.XML` | `JSONObject toJSONObject(String string)` | 转换XML为JSONObject 转换过程中一些信息可能会丢失，JSON中无法区分节点和属性，相同的节点将被处理为JSONArray。 Content text may be placed in a "content" member. Comments, prologs, DTDs, and are ignored. |
| `cn.hutool.json.XML` | `JSONObject toJSONObject(String string,boolean keepStrings)` | 转换XML为JSONObject 转换过程中一些信息可能会丢失，JSON中无法区分节点和属性，相同的节点将被处理为JSONArray。 Content text may be placed in a "content" member. Comments, prologs, DTDs, and are ignored. All values are converted as strings, for 1, 01, 29.0 will not be coerced to numbers but will instead be the exact value as seen in the XML d… |
| `cn.hutool.json.XML` | `JSONObject toJSONObject(final JSONObject jo,final String xmlStr,final ParseConfig parseConfig)` | 转换XML为JSONObject 转换过程中一些信息可能会丢失，JSON中无法区分节点和属性，相同的节点将被处理为JSONArray。 |
| `cn.hutool.json.XML` | `JSONObject toJSONObject(final String string,final ParseConfig parseConfig)` | 转换XML为JSONObject 转换过程中一些信息可能会丢失，JSON中无法区分节点和属性，相同的节点将被处理为JSONArray。 Content text may be placed in a "content" member. Comments, prologs, DTDs, and are ignored. All values are converted as strings, for 1, 01, 29.0 will not be coerced to numbers but will instead be the exact value as seen in the XML d… |
| `cn.hutool.json.XML` | `String toXml(Object object)` | 转换JSONObject为XML |
| `cn.hutool.json.XML` | `String toXml(Object object,String tagName)` | 转换JSONObject为XML |
| `cn.hutool.json.XML` | `String toXml(Object object,String tagName,String... contentKeys)` | 转换JSONObject为XML |
| `cn.hutool.json.XMLTokener` | `Object nextContent()` | 【原文待译】Get the next XML outer token, trimming whitespace. There are two kinds of tokens: the '>' character which begins a markup tag, and the content text between markup tags. |
| `cn.hutool.json.XMLTokener` | `Object nextEntity(char ampersand)` | 【原文待译】Return the next entity. These entities are translated to Characters: & ' > < ". |
| `cn.hutool.json.XMLTokener` | `Object nextMeta()` | 【原文待译】Returns the next XML meta token. This is used for skipping over <!...> and <?...?> structures. |
| `cn.hutool.json.XMLTokener` | `Object nextToken()` | 【原文待译】Get the next XML Token. These tokens are found inside of angle brackets. It may be one of these characters: / > = ! ? or it may be a string wrapped in single quotes or double quotes, or it may be a name. |
| `cn.hutool.json.XMLTokener` | `String nextCDATA()` | 【原文待译】Get the text in the CDATA block. |
| `cn.hutool.json.XMLTokener` | `boolean skipPast(String to)` | 【原文待译】Skip characters until past the requested string. If it is not found, we are left at the end of the source with a result of false. |
