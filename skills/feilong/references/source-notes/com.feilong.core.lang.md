# com.feilong.core.lang

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.core.lang.ArrayUtil` | `T getElement(Object array,int index)` | 得到指定数组对象 array 中指定索引 index 的元素. |
| `com.feilong.core.lang.ArrayUtil` | `T[] newArray(Class<T> componentType,int length)` | 构造一个指定类型 componentType 以及指定长度 length 的数组. |
| `com.feilong.core.lang.ClassLoaderUtil` | `InputStream getResourceAsStream(String resourceName,Class<?> callingClass)` | 加载资源 resourceName 为 InputStream. |
| `com.feilong.core.lang.ClassLoaderUtil` | `URL getResource(String resourceName)` | 获得给定名称 resourceName 的资源. |
| `com.feilong.core.lang.ClassLoaderUtil` | `URL getResourceInAllClassLoader(String resourceName,Class<?> callingClass)` | 【原文待译】Load a given resource. |
| `com.feilong.core.lang.ClassUtil` | `Class<?> getClass(String className)` | JVM查找并加载指定的类. |
| `com.feilong.core.lang.ClassUtil` | `Class<?>[] toClass(Object... paramValues)` | 解析对象参数 paramValues ,获得参数类型. |
| `com.feilong.core.lang.ClassUtil` | `boolean isAssignableFrom(Class<?> klass,Class<?> cls)` | Checks if is assignable from. instanceof :子 -----> 父 isAssignableFrom :父 -----> 子 |
| `com.feilong.core.lang.ClassUtil` | `boolean isInstance(Object obj,Class<?> klass)` | 判断一个对象 obj 是不是某个类 klass 的实例. |
| `com.feilong.core.lang.ClassUtil` | `boolean isInstanceAnyClass(Object obj,Class<?>... klasses)` | 判断 obj 是否isInstance 任意的一个 klasses . |
| `com.feilong.core.lang.ClassUtil` | `boolean isInterface(Class<?> ownerClass)` | 判断类 ownerClass 是否是接口. |
| `com.feilong.core.lang.EnumUtil` | `E getEnumByPropertyValue(Class<E> enumClass,String propertyName,T specifiedValue)` | 通过 propertyName 的 specifiedValue 获得枚举(equals判断, 区分大小写 ). |
| `com.feilong.core.lang.EnumUtil` | `E getEnumByPropertyValueIgnoreCase(Class<E> enumClass,String propertyName,T specifiedValue)` | 通过 propertyName 的 specifiedValue (忽视大小写) 获得枚举(equalsIgnoreCase判断). |
| `com.feilong.core.lang.NumberUtil` | `BigDecimal getAddValue(Number... numbers)` | 所有数加起来. 关于精度: 返回结果的精度等于精度最大的元素的精度,比如 NumberUtil.getAddValue(2, 4, 5.00000) = 11.00000 |
| `com.feilong.core.lang.NumberUtil` | `BigDecimal getDivideValue(Number one,Number two,int scale)` | 获得除法结果 one/two ,四舍五入RoundingMode#HALF_UP,小数位数 scale 指定. |
| `com.feilong.core.lang.NumberUtil` | `BigDecimal getDivideValue(Number one,Number two,int scale,RoundingMode roundingMode)` | 获得除法结果 one/two ,指定舍入方式 roundingMode 以及 小数位数 scale . |
| `com.feilong.core.lang.NumberUtil` | `BigDecimal getMultiplyValue(Number one,Number two,int scale)` | 将第一个数字 one 和第二个数字 two 相乘,指定精度 scale , 返回BigDecimal. |
| `com.feilong.core.lang.NumberUtil` | `BigDecimal getSubtractValue(Number beSubtractedValue,Number... subtractions)` | 所有数相减. 关于精度: 返回结果的精度等于精度最大的元素的精度,比如 NumberUtil.getSubtractValue(1000, 99.5, 99.0000) = 801.5000 |
| `com.feilong.core.lang.NumberUtil` | `BigDecimal getSubtractValueWithScale(Number beSubtractedValue,Number subtraction,int scale)` | 数相减. |
| `com.feilong.core.lang.NumberUtil` | `BigDecimal setScale(Number value,int scale)` | 使用四舍五入 RoundingMode#HALF_UP 设置小数点位数. |
| `com.feilong.core.lang.NumberUtil` | `BigDecimal setScale(Number value,int scale,RoundingMode roundingMode)` | 使用 roundingMode 来设置小数点位数. |
| `com.feilong.core.lang.NumberUtil` | `String getProgress(Number current,Number total)` | 计算进度(当前量 current /总量 total ,使用百分比两位小数点 NumberPattern#PERCENT_WITH_2POINT 转成指定的字符串格式. 常用于友好的显示 下载进度 , 执行进度 等等场景 |
| `com.feilong.core.lang.NumberUtil` | `String getProgress(Number current,Number total,String numberPattern)` | 计算进度(当前量 current /总量 total ,然后转成指定的字符串格式 numberPattern ). 常用于友好的显示 下载进度 , 执行进度 等等场景 |
| `com.feilong.core.lang.NumberUtil` | `String toString(Number value,String numberPattern)` | 将数字 value 按照指定的格式 numberPattern 格式成字符串 . 调用 NumberFormatUtil#format(Number, String, RoundingMode),当遇到需要舍入的时候,使用常用的 RoundingMode#HALF_UP |
| `com.feilong.core.lang.NumberUtil` | `boolean isEquals(Number one,Number two)` | 判断第1个数字数字值 one 是不是= (等于) 第2个数字数字值 two . |
| `com.feilong.core.lang.NumberUtil` | `boolean isGreaterThan(Number one,Number two)` | 判断第1个数字数字值 one 是不是> (大于) 第2个数字数字值 two . |
| `com.feilong.core.lang.NumberUtil` | `boolean isGreaterThanOrEquals(Number one,Number two)` | 判断第1个数字数字值 one 是不是>= (大于等于) 第2个数字数字值 two . |
| `com.feilong.core.lang.NumberUtil` | `boolean isLessThan(Number one,Number two)` | 判断第1个数字数字值 one 是不是 two . |
| `com.feilong.core.lang.NumberUtil` | `boolean isLessThanOrEquals(Number one,Number two)` | 判断第1个数字数字值 one 是不是 two . |
| `com.feilong.core.lang.ObjectUtil` | `Integer defaultCountIfNullZeroOrGreaterThan(Integer count,Integer defaultValue)` | 如果 count 是null或者> defaultValue ,返回默认值 defaultValue ,否则返回 i . 常用于控制分页count传入的参数值,控制不要超过最大值, 比如限定一次最多只能获取50条数据 |
| `com.feilong.core.lang.ObjectUtil` | `Integer defaultIfNullOrLessThanOne(Integer i,Integer defaultValue)` | 如果 i 是null或者 defaultValue . 常用于分页处理页面的场景 |
| `com.feilong.core.lang.ObjectUtil` | `Integer defaultPageNo(Integer pageNo)` | 如果 pageNo 是null或者 1 . 用于分页处理页面的场景 |
| `com.feilong.core.lang.ObjectUtil` | `Integer defaultZero(Integer i)` | 如果 i 是null或者 0 . |
| `com.feilong.core.lang.ObjectUtil` | `List<T> defaultEmptyListIfNull(final List<T> list)` | 如果 list 是null,返回默认值 java.util.Collections#emptyList(). |
| `com.feilong.core.lang.ObjectUtil` | `List<T> defaultNewArrayListIfNull(final List<T> list)` | 如果 list 是null,返回默认值 com.feilong.core.util.CollectionsUtil#newArrayList(). |
| `com.feilong.core.lang.ObjectUtil` | `Map<K, V> defaultEmptyMapIfNull(final Map<K, V> map)` | 如果 map 是null,返回默认值 java.util.Collections#emptyMap(). |
| `com.feilong.core.lang.ObjectUtil` | `Map<K, V> defaultNewHashMapIfNull(final Map<K, V> map)` | 如果 map 是null,返回默认值 com.feilong.core.util.MapUtil#newHashMap(). |
| `com.feilong.core.lang.ObjectUtil` | `Map<K, V> defaultNewLinkedHashMapIfNull(final Map<K, V> map)` | 如果 map 是null,返回默认值 com.feilong.core.util.MapUtil#newLinkedHashMap(). |
| `com.feilong.core.lang.ObjectUtil` | `Set<T> defaultEmptySetIfNull(final Set<T> set)` | 如果 set 是null,返回默认值 java.util.Collections#emptySet(). |
| `com.feilong.core.lang.ObjectUtil` | `Set<T> defaultNewHashSetIfNull(final Set<T> set)` | 如果 set 是null,返回默认值 com.feilong.core.util.CollectionsUtil#newHashSet(). |
| `com.feilong.core.lang.ObjectUtil` | `String defaultEmptyStringIfNull(final String str)` | 如果 str 是null,返回默认值 com.feilong.core.lang.StringUtil#EMPTY. |
| `com.feilong.core.lang.ObjectUtil` | `T defaultIfNull(final T object,final T defaultValue)` | 如果 object 是null,返回默认值 defaultValue . |
| `com.feilong.core.lang.ObjectUtil` | `T defaultIfNullOrEmpty(final T object,final T defaultValue)` | 如果 object 是null或者empty,返回默认值 defaultValue . |
| `com.feilong.core.lang.ObjectUtil` | `T newFrom(final Class<T> klass,Object fromObj,String... includePropertyNames)` | 新建klass实例, 并将fromObj中的 指定属于 includePropertyNames 设置到新建的实例中. |
| `com.feilong.core.lang.ObjectUtil` | `boolean defaultFalseIfNull(final Boolean booleanValue)` | 如果 booleanValue 是null,返回 booleanValue ;非null时候原样返回. |
| `com.feilong.core.lang.ObjectUtil` | `boolean defaultTrueIfNull(final Boolean booleanValue)` | 如果 booleanValue 是null,返回 true ;非null时候原样返回. |
| `com.feilong.core.lang.ObjectUtil` | `boolean equalsAny(T t,T... searchTargets)` | 对比 given t to a vararg of searchTargets, 如果 true if the t is equal to any of the searchTargets. 比 apache commons-lang3 StringUtils#equalsAny 适用面更广 |
| `com.feilong.core.lang.ObjectUtil` | `boolean isArray(Object object)` | 判断指定的对象 object 是否是数组. |
| `com.feilong.core.lang.ObjectUtil` | `boolean isPrimitiveArray(Object object)` | 判断指定的对象 object 是否是原生类型数组. |
| `com.feilong.core.lang.StringUtil` | `List<String> tokenizeToList(String str)` | 使用 默认分隔符 ;, (逗号,分号和空格) 分隔给定的字符串,转成List,去除 tokens的空格并且忽略empty tokens. (此方法借鉴 "org.springframework.util.StringUtils#tokenizeToStringArray"). 调用了 #tokenizeToStringArray(String, String, boolean, boolean), 本方法默认使用参数 trimTokens = true; ignoreEmptyTokens = true; , 默认分隔符 ;, (逗号,分号和空格) |
| `com.feilong.core.lang.StringUtil` | `List<T> tokenizeToList(String str,Class<T> perElementConvertClass)` | 使用 默认分隔符 ;, (逗号,分号和空格) 分隔给定的字符串,转成List,去除 tokens的空格并且忽略empty tokens, 然后将每个元素转换成指定的类型 perElementConvertClass 对应的list. (此方法借鉴 "org.springframework.util.StringUtils#tokenizeToStringArray"). 调用了 #tokenizeToStringArray(String, String, boolean, boolean), 本方法默认使用参数 trimTokens = true; ignoreEmptyTokens = tr… |
| `com.feilong.core.lang.StringUtil` | `Map<String, List<String>> toMultiValueMap(String configString)` | 将 asedeffrrfgg=张飞,关羽;asedcccccfgg=吕布;这种格式的字符串转换成map , map的key 是asedeffrrfgg,asedcccccfgg 这种, value 是张飞,关羽 吕布 这种等号后面的值,使用逗号分隔成list. |
| `com.feilong.core.lang.StringUtil` | `Map<String, List<V>> toMultiValueMap(String configString,Class<V> valueElementClass)` | 将 asedeffrrfgg=张飞,关羽;asedcccccfgg=吕布;这种格式的字符串转换成map , map的key 是asedeffrrfgg,asedcccccfgg 这种, value 是张飞,关羽 吕布 这种等号后面的值,使用逗号分隔成list. |
| `com.feilong.core.lang.StringUtil` | `Map<String, String> toSingleValueMap(String configString)` | 将 189=988;200=455;这种格式的字符串转换成map , map的key 是189这种, value 是988,455 这种等号后面的值,使用逗号分隔成list. |
| `com.feilong.core.lang.StringUtil` | `Map<T, List<V>> toMultiValueMap(String configString,Class<T> keyClass,Class<V> valueElementClass)` | 将 189=988,900;200=455;这种格式的字符串转换成map , map的key 是189,200 这种, value 是988,900,455 这种等号后面的值,使用逗号分隔成list. |
| `com.feilong.core.lang.StringUtil` | `Map<T, V> toMap(String configString,Class<T> keyClass,StringToBeanConverter<V> valueStringToBeanConverter)` | 将 73034693=0-50;11487680=0-43;51099626=0-50; 这种格式的字符串转换成map. map的key 是73034693这种, value 可以TrackQueryExtendParam对象 |
| `com.feilong.core.lang.StringUtil` | `Map<T, V> toSingleValueMap(String configString,Class<T> keyClass,Class<V> valueElementClass)` | 将 189=988;200=455;这种格式的字符串转换成map , map的key 是189这种, value 是988,455 这种等号后面的值,使用逗号分隔成list. |
| `com.feilong.core.lang.StringUtil` | `Set<String> tokenizeToSet(String str)` | 使用 默认分隔符 ;, (逗号,分号和空格) 分隔给定的字符串,转成Set,去除 tokens的空格并且忽略empty tokens. (此方法借鉴 "org.springframework.util.StringUtils#tokenizeToStringArray"). 调用了 #tokenizeToStringArray(String, String, boolean, boolean), 本方法默认使用参数 trimTokens = true; ignoreEmptyTokens = true; , 默认分隔符 ;, (逗号,分号和空格) |
| `com.feilong.core.lang.StringUtil` | `Set<T> tokenizeToSet(String str,Class<T> perElementConvertClass)` | 使用 默认分隔符 ;, (逗号,分号和空格) 分隔给定的字符串,转成Set,去除 tokens的空格并且忽略empty tokens, 然后将每个元素转换成指定的类型 perElementConvertClass 对应的set. (此方法借鉴 "org.springframework.util.StringUtils#tokenizeToStringArray"). 调用了 #tokenizeToStringArray(String, String, boolean, boolean), 本方法默认使用参数 trimTokens = true; ignoreEmptyTokens = true… |
| `com.feilong.core.lang.StringUtil` | `String clean(CharSequence charSequence)` | 清除charSequence 中一些特殊符号, 目前会清除 backspace (\b), 三个特殊空格 , , . |
| `com.feilong.core.lang.StringUtil` | `String format(String format,Object... args)` | 将各类数据,使用String#format(String, Object...)格式化为字符串. |
| `com.feilong.core.lang.StringUtil` | `String formatPattern(String messagePattern,Object... args)` | 格式化字符串,此方法是抽取slf4j的核心方法. 在java中,常会拼接字符串生成新的字符串值,在字符串拼接过程中容易写错或者位置写错 slf4j的log支持格式化输出log,比如: log.debug("{}","feilong"); log.info("{},{}","feilong","hello"); 这些写法非常简洁且有效,不易出错 因此,你可以在代码中出现这样的写法: |
| `com.feilong.core.lang.StringUtil` | `String newString(byte[] bytes)` | Constructs a new String by decoding the specified array of bytes using the given charset. 默认使用 CharsetType#UTF8 |
| `com.feilong.core.lang.StringUtil` | `String newString(byte[] bytes,String charsetType)` | 【原文待译】Constructs a new String by decoding the specified array of bytes using the given charset. |
| `com.feilong.core.lang.StringUtil` | `String removeSpecialSpace(CharSequence charSequence)` | 删除特殊空格. , , |
| `com.feilong.core.lang.StringUtil` | `String replace(CharSequence templateString,Map<String, V> valuesMap)` | 使用给定的字符串 templateString 作为模板,解析匹配的变量 . |
| `com.feilong.core.lang.StringUtil` | `String replace(final String text,final String searchString,final String replacement)` | 将 text 中的 searchString 替换成 replacement . |
| `com.feilong.core.lang.StringUtil` | `String replaceAll(CharSequence content,String regex,String replacement)` | 使用给定的 replacement 替换 content 此字符串所有匹配给定的正则表达式 regex 的子字符串. |
| `com.feilong.core.lang.StringUtil` | `String substring(final String text,final int beginIndex)` | [截取]从指定索引处( beginIndex )的字符开始,直到此字符串末尾. 如果 beginIndex 是负数,那么表示倒过来截取,从结尾开始截取长度,此时等同于 #substringLast(String, int) |
| `com.feilong.core.lang.StringUtil` | `String substring(final String text,int startIndex,int length)` | [截取]从开始位置( startIndex ),截取固定长度( length )字符串. |
| `com.feilong.core.lang.StringUtil` | `String substringLast(final String text,int lastLenth)` | [截取]:获取文字最后位数 lastLenth 的字符串. |
| `com.feilong.core.lang.StringUtil` | `String substringWithoutLast(final CharSequence text,final String lastString)` | [截取]:去除最后的字符串 lastString . |
| `com.feilong.core.lang.StringUtil` | `String substringWithoutLast(final String text,final int lastLenth)` | [截取]:去除最后几位 lastLenth . 调用了 java.lang.String#substring(int, int) |
| `com.feilong.core.lang.StringUtil` | `String[] split(String value,String regexSpliter)` | 将字符串 value 使用分隔符 regexSpliter 分隔成 字符串数组. 建议使用 #tokenizeToStringArray(String, String) 或者 StringUtils#split(String) |
| `com.feilong.core.lang.StringUtil` | `String[] tokenizeToStringArray(String str)` | 使用 默认分隔符 ;, (逗号,分号和空格) 分隔给定的字符串到字符串数组,去除 tokens的空格并且忽略empty tokens. (此方法借鉴 "org.springframework.util.StringUtils#tokenizeToStringArray"). 调用了 #tokenizeToStringArray(String, String, boolean, boolean), 本方法默认使用参数 trimTokens = true; ignoreEmptyTokens = true; , 默认分隔符 ;, (逗号,分号和空格) |
| `com.feilong.core.lang.StringUtil` | `String[] tokenizeToStringArray(String str,String delimiters)` | 使用StringTokenizer分隔给定的字符串到字符串数组,去除 tokens的空格并且忽略empty tokens. (此方法借鉴 "org.springframework.util.StringUtils#tokenizeToStringArray"). 调用了 #tokenizeToStringArray(String, String, boolean, boolean), 本方法默认使用参数 trimTokens = true; ignoreEmptyTokens = true; |
| `com.feilong.core.lang.StringUtil` | `String[] tokenizeToStringArray(String str,String delimiters,boolean trimTokens,boolean ignoreEmptyTokens)` | 使用StringTokenizer分隔给定的字符串到字符串数组. (此方法借鉴 "org.springframework.util.StringUtils#tokenizeToStringArray"). |
| `com.feilong.core.lang.StringUtil` | `boolean tokenizeToArrayContains(String config,String delimiters,T element)` | 将配置类型的逗号分隔字符串分割转换成数组,然后自动转换成element一样的类型,判断是否包含. |
| `com.feilong.core.lang.StringUtil` | `boolean tokenizeToArrayContains(String config,T element)` | 将配置类型的逗号分隔字符串分割转换成数组,然后自动转换成element一样的类型,判断是否包含. |
| `com.feilong.core.lang.StringUtil` | `boolean trimAndEqualsIgnoreCase(String s1,String s2)` | 将两个字符串,去空格之后忽视大小写对比. |
| `com.feilong.core.lang.StringUtil` | `byte[] getBytes(String value)` | 字符串转换成byte数组. |
| `com.feilong.core.lang.StringUtil` | `byte[] getBytes(String value,String charsetName)` | 字符串 value 转换成byte数组. |
| `com.feilong.core.lang.SystemUtil` | `Map<String, String> getEnvMap()` | 取到 System#getenv(),转成 java.util.TreeMap,以遍输出log的时候,会顺序显示. |
| `com.feilong.core.lang.SystemUtil` | `Map<String, String> getPropertiesMap()` | 取到 System#getProperty(String),转成 java.util.TreeMap,以遍输出log的时候,会顺序显示. |
| `com.feilong.core.lang.SystemUtil` | `String getEnv(String key)` | 读取环境变量. |
| `com.feilong.core.lang.SystemUtil` | `String getSystemProperty(final String property)` | 【原文待译】Gets a System property, defaulting to null if the property cannot be read. If a SecurityException is caught, the return value is null and a message is written to System.err. |
| `com.feilong.core.lang.SystemUtil` | `void setPropertiesFromMap(Map<String, String> map)` | 循环 map ,设置到系统属性 java.lang.System#setProperty(String, String). 如果 map 是null,抛出 NullPointerException 如果 map 是empty,抛出 IllegalArgumentException |
| `com.feilong.core.lang.SystemUtil` | `void setPropertiesFromProperties(Properties properties)` | 设置 properties from properties. 如果 properties 是null,抛出 NullPointerException |
| `com.feilong.core.lang.ThreadUtil` | `void execute(List<T> list,Map<String, ?> paramsMap,PartitionPerHandler<T> partitionPerHandler)` | 给定一个待解析的 list ,自动 构造多条线程 并运行. |
| `com.feilong.core.lang.ThreadUtil` | `void execute(List<T> list,PartitionPerHandler<T> partitionPerHandler)` | 给定一个待解析的 list ,自动 构造多条线程 并运行. |
| `com.feilong.core.lang.ThreadUtil` | `void execute(List<T> list,PartitionThreadConfig partitionThreadConfig,Map<String, ?> paramsMap,PartitionPerHandler<T> partitionPerHandler)` | 给定一个待解析的 list ,设定每个线程执行多少条 eachSize ,传入一些额外的参数 paramsMap ,使用自定义的 partitionPerHandler ,自动 构造多条线程 并运行. |
| `com.feilong.core.lang.ThreadUtil` | `void execute(List<T> list,int eachSize,Map<String, ?> paramsMap,PartitionPerHandler<T> partitionPerHandler)` | 给定一个待解析的 list ,设定每个线程执行多少条 eachSize ,传入一些额外的参数 paramsMap ,使用自定义的 partitionPerHandler ,自动 构造多条线程 并运行. 主要是用来简化 #execute(List, int, Map, PartitionRunnableBuilder) 调用 |
| `com.feilong.core.lang.ThreadUtil` | `void execute(List<T> list,int eachSize,Map<String, ?> paramsMap,PartitionRunnableBuilder<T> partitionRunnableBuilder)` | 给定一个待解析的 list ,设定每个线程执行多少条 eachSize ,传入一些额外的参数 paramsMap ,使用自定义的 partitionRunnableBuilder ,自动 构造多条线程 并运行. |
| `com.feilong.core.lang.ThreadUtil` | `void execute(List<T> list,int eachSize,PartitionPerHandler<T> partitionPerHandler)` | 给定一个待解析的 list ,设定每个线程执行多少条 eachSize ,使用自定义的 partitionRunnableBuilder ,自动 构造多条线程 并运行. 主要是用来简化 #execute(List, int, PartitionRunnableBuilder) 调用 |
| `com.feilong.core.lang.ThreadUtil` | `void execute(List<T> list,int eachSize,PartitionRunnableBuilder<T> partitionRunnableBuilder)` | 给定一个待解析的 list ,设定每个线程执行多少条 eachSize ,使用自定义的 partitionRunnableBuilder ,自动 构造多条线程 并运行. |
| `com.feilong.core.lang.ThreadUtil` | `void execute(Runnable runnable,int threadCount)` | 创建指定数量 threadCount 的线程,并执行. |
| `com.feilong.core.lang.ThreadUtil` | `void executeUsePerElement(List<T> list,Map<String, ?> paramsMap,PartitionPerElementHandler<T> partitionPerElementHandler)` | 给定一个待解析的 list ,自动 构造多条线程 并运行. |
| `com.feilong.core.lang.ThreadUtil` | `void executeUsePerElement(List<T> list,PartitionPerElementHandler<T> partitionPerElementHandler)` | 给定一个待解析的 list ,自动 构造多条线程 并运行. |
| `com.feilong.core.lang.ThreadUtil` | `void executeUsePerElement(List<T> list,PartitionThreadConfig partitionThreadConfig,Map<String, ?> paramsMap,PartitionPerElementHandler<T> partitionPerElementHandler)` | 给定一个待解析的 list ,设定每个线程执行多少条 eachSize ,传入一些额外的参数 paramsMap ,使用自定义的 partitionPerHandler ,自动 构造多条线程 并运行. |
| `com.feilong.core.lang.ThreadUtil` | `void sleep(int milliseconds)` | 强制当前正在执行的线程 休眠(暂停执行) milliseconds 毫秒. 该方法简便的地方在于,捕获了异常和记录了日志,不需要再写这些额外代码 |
| `com.feilong.core.lang.ThreadUtil` | `void sleep(long milliseconds)` | 强制当前正在执行的线程 休眠(暂停执行) milliseconds 毫秒. 该方法简便的地方在于,捕获了异常和记录了日志,不需要再写这些额外代码 |
| `com.feilong.core.lang.ThreadUtil` | `void sleepSeconds(int seconds)` | 强制当前正在执行的线程 休眠(暂停执行) seconds 秒. 该方法简便的地方在于,捕获了异常和记录了日志,不需要再写这些额外代码 |
| `com.feilong.core.lang.ThreadUtil` | `void startAndJoin(Thread[] threads)` | 循环 threads 调用 java.lang.Thread#start() 再循环 threads 调用 java.lang.Thread#join(). threads are run concurrently and this method waits for them to finish. 如果 threads 是null,抛出 NullPointerException 如果 threads 是empty,抛出 IllegalArgumentException |
