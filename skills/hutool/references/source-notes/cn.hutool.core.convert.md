# cn.hutool.core.convert

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.convert.AbstractConverter` | `Class<T> getTargetType()` | 获得此类实现类的泛型类型 |
| `cn.hutool.core.convert.AbstractConverter` | `T convert(Object value,T defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.convert.AbstractConverter` | `T convertQuietly(Object value,T defaultValue)` | 不抛异常转换 当转换失败时返回默认值 |
| `cn.hutool.core.convert.BasicType` | `Class<?> unWrap(Class<?> clazz)` | 包装类转为原始类，非包装类返回原类 |
| `cn.hutool.core.convert.BasicType` | `Class<?> wrap(Class<?> clazz)` | 原始类转为包装类，非原始类返回原类 |
| `cn.hutool.core.convert.CastUtil` | `Collection<T> castDown(Collection<? super T> collection)` | 泛型集合向下转型。例如将Collection<Number>转换为Collection<Integer> |
| `cn.hutool.core.convert.CastUtil` | `Collection<T> castUp(Collection<? extends T> collection)` | 泛型集合向上转型。例如将Collection<Integer>转换为Collection<Number> |
| `cn.hutool.core.convert.CastUtil` | `List<T> castDown(List<? super T> list)` | 泛型集合向下转型。例如将List<Number>转换为List<Integer> |
| `cn.hutool.core.convert.CastUtil` | `List<T> castUp(List<? extends T> list)` | 泛型接口向上转型。例如将List<Integer>转换为List<Number> |
| `cn.hutool.core.convert.CastUtil` | `Map<K, V> castDown(Map<? super K, ? super V> map)` | 泛型集合向下转型。例如将Map<Number,Number>转换为Map<Integer, Integer> |
| `cn.hutool.core.convert.CastUtil` | `Map<K, V> castUp(Map<? extends K, ? extends V> map)` | 泛型集合向下转型。例如将Map<Integer, Integer>转换为Map<Number,Number> |
| `cn.hutool.core.convert.CastUtil` | `Set<T> castDown(Set<? super T> set)` | 泛型集合向下转型。例如将Set<Number>转换为Set<Integer> |
| `cn.hutool.core.convert.CastUtil` | `Set<T> castUp(Set<? extends T> set)` | 泛型集合向上转型。例如将Set<Integer>转换为Set<Number> |
| `cn.hutool.core.convert.Convert` | `BigDecimal chineseMoneyToNumber(String chineseMoneyAmount)` | 中文大写数字金额转换为数字，返回结果以元为单位的BigDecimal类型数字 如： “陆万柒仟伍佰伍拾陆元叁角贰分”返回“67556.32” “叁角贰分”返回“0.32” |
| `cn.hutool.core.convert.Convert` | `BigDecimal toBigDecimal(Object value)` | 转换为BigDecimal 如果给定的值为空，或者转换失败，返回null 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `BigDecimal toBigDecimal(Object value,BigDecimal defaultValue)` | 转换为BigDecimal 如果给定的值为空，或者转换失败，返回默认值 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `BigInteger toBigInteger(Object value)` | 转换为BigInteger 如果给定的值为空，或者转换失败，返回默认值null 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `BigInteger toBigInteger(Object value,BigInteger defaultValue)` | 转换为BigInteger 如果给定的值为空，或者转换失败，返回默认值 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `Boolean toBool(Object value)` | 转换为boolean 如果给定的值为空，或者转换失败，返回默认值null 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `Boolean toBool(Object value,Boolean defaultValue)` | 转换为boolean String支持的值为：true、false、yes、ok、no，1,0 如果给定的值为空，或者转换失败，返回默认值 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `Boolean[] toBooleanArray(Object value)` | 转换为Boolean数组 |
| `cn.hutool.core.convert.Convert` | `Byte toByte(Object value)` | 转换为byte 如果给定的值为null，或者转换失败，返回默认值null 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `Byte toByte(Object value,Byte defaultValue)` | 转换为byte 如果给定的值为null，或者转换失败，返回默认值 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `Byte[] toByteArray(Object value)` | 转换为Byte数组 |
| `cn.hutool.core.convert.Convert` | `Character toChar(Object value)` | 转换为字符 如果给定的值为null，或者转换失败，返回默认值null 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `Character toChar(Object value,Character defaultValue)` | 转换为字符 如果给定的值为null，或者转换失败，返回默认值 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `Character[] toCharArray(Object value)` | 转换为Character数组 |
| `cn.hutool.core.convert.Convert` | `Class<?> unWrap(Class<?> clazz)` | 包装类转为原始类，非包装类返回原类 |
| `cn.hutool.core.convert.Convert` | `Class<?> wrap(Class<?> clazz)` | 原始类转为包装类，非原始类返回原类 |
| `cn.hutool.core.convert.Convert` | `Collection<?> toCollection(Class<?> collectionType,Class<?> elementType,Object value)` | 转换为集合类 |
| `cn.hutool.core.convert.Convert` | `Date toDate(Object value)` | 转换为Date 如果给定的值为空，或者转换失败，返回null 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `Date toDate(Object value,Date defaultValue)` | 转换为Date 如果给定的值为空，或者转换失败，返回默认值 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `Date toInstant(Object value,Date defaultValue)` | Instant 如果给定的值为空，或者转换失败，返回默认值 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `Double toDouble(Object value)` | 转换为double 如果给定的值为空，或者转换失败，返回默认值null 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `Double toDouble(Object value,Double defaultValue)` | 转换为double 如果给定的值为空，或者转换失败，返回默认值 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `Double[] toDoubleArray(Object value)` | 转换为Double数组 |
| `cn.hutool.core.convert.Convert` | `E toEnum(Class<E> clazz,Object value)` | 转换为Enum对象 如果给定的值为空，或者转换失败，返回默认值null |
| `cn.hutool.core.convert.Convert` | `E toEnum(Class<E> clazz,Object value,E defaultValue)` | 转换为Enum对象 如果给定的值为空，或者转换失败，返回默认值 |
| `cn.hutool.core.convert.Convert` | `Float toFloat(Object value)` | 转换为Float 如果给定的值为空，或者转换失败，返回默认值null 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `Float toFloat(Object value,Float defaultValue)` | 转换为Float 如果给定的值为空，或者转换失败，返回默认值 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `Float[] toFloatArray(Object value)` | 转换为Float数组 |
| `cn.hutool.core.convert.Convert` | `Integer toInt(Object value)` | 转换为int 如果给定的值为null，或者转换失败，返回默认值null 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `Integer toInt(Object value,Integer defaultValue)` | 转换为int 如果给定的值为空，或者转换失败，返回默认值 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `Integer[] toIntArray(Object value)` | 转换为Integer数组 |
| `cn.hutool.core.convert.Convert` | `List<?> toList(Object value)` | 转换为ArrayList，元素类型默认Object |
| `cn.hutool.core.convert.Convert` | `List<T> toList(Class<T> elementType,Object value)` | 转换为ArrayList |
| `cn.hutool.core.convert.Convert` | `LocalDateTime toLocalDateTime(Object value)` | 转换为LocalDateTime 如果给定的值为空，或者转换失败，返回null 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `LocalDateTime toLocalDateTime(Object value,LocalDateTime defaultValue)` | LocalDateTime 如果给定的值为空，或者转换失败，返回默认值 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `Long toLong(Object value)` | 转换为long 如果给定的值为null，或者转换失败，返回默认值null 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `Long toLong(Object value,Long defaultValue)` | 转换为long 如果给定的值为空，或者转换失败，返回默认值 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `Long[] toLongArray(Object value)` | 转换为Long数组 |
| `cn.hutool.core.convert.Convert` | `Map<K, V> toMap(Class<? extends Map> mapType,Class<K> keyType,Class<V> valueType,Object value)` | 转换为Map |
| `cn.hutool.core.convert.Convert` | `Map<K, V> toMap(Class<K> keyType,Class<V> valueType,Object value)` | 转换为Map，若value原本就是Map，则转为原始类型，若不是则默认转为HashMap |
| `cn.hutool.core.convert.Convert` | `Number toNumber(Object value)` | 转换为Number 如果给定的值为空，或者转换失败，返回默认值null 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `Number toNumber(Object value,Number defaultValue)` | 转换为Number 如果给定的值为空，或者转换失败，返回默认值 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `Number[] toNumberArray(Object value)` | 转换为Number数组 |
| `cn.hutool.core.convert.Convert` | `Set<T> toSet(Class<T> elementType,Object value)` | 转换为HashSet |
| `cn.hutool.core.convert.Convert` | `Short toShort(Object value)` | 转换为Short 如果给定的值为null，或者转换失败，返回默认值null 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `Short toShort(Object value,Short defaultValue)` | 转换为Short 如果给定的值为null，或者转换失败，返回默认值 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `Short[] toShortArray(Object value)` | 转换为Short数组 |
| `cn.hutool.core.convert.Convert` | `String convertCharset(String str,String sourceCharset,String destCharset)` | 给定字符串转换字符编码 如果参数为空，则返回原字符串，不报错。 |
| `cn.hutool.core.convert.Convert` | `String digitToChinese(Number n)` | 金额转为中文形式 |
| `cn.hutool.core.convert.Convert` | `String hexToStr(String hexStr,Charset charset)` | 十六进制转换字符串 |
| `cn.hutool.core.convert.Convert` | `String numberToChinese(double number,boolean isUseTraditional)` | 将阿拉伯数字转为中文表达方式 |
| `cn.hutool.core.convert.Convert` | `String numberToSimple(Number number)` | 将阿拉伯数字转为精简表示形式，例如: |
| `cn.hutool.core.convert.Convert` | `String numberToWord(Number number)` | 将阿拉伯数字转为英文表达方式 |
| `cn.hutool.core.convert.Convert` | `String strToUnicode(String strText)` | String的字符串转换成unicode的String |
| `cn.hutool.core.convert.Convert` | `String toDBC(String input)` | 全角转半角 |
| `cn.hutool.core.convert.Convert` | `String toDBC(String text,Set<Character> notConvertSet)` | 替换全角为半角 |
| `cn.hutool.core.convert.Convert` | `String toHex(String str,Charset charset)` | 字符串转换成十六进制字符串，结果为小写 |
| `cn.hutool.core.convert.Convert` | `String toHex(byte[] bytes)` | byte数组转16进制串 |
| `cn.hutool.core.convert.Convert` | `String toSBC(String input)` | 半角转全角，null返回null |
| `cn.hutool.core.convert.Convert` | `String toSBC(String input,Set<Character> notConvertSet)` | 半角转全角，null返回null |
| `cn.hutool.core.convert.Convert` | `String toStr(Object value)` | 转换为字符串 如果给定的值为null，或者转换失败，返回默认值null 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `String toStr(Object value,String defaultValue)` | 转换为字符串 如果给定的值为null，或者转换失败，返回默认值 转换失败不会报错 |
| `cn.hutool.core.convert.Convert` | `String unicodeToStr(String unicode)` | unicode的String转换成String的字符串 |
| `cn.hutool.core.convert.Convert` | `String[] toStrArray(Object value)` | 转换为String数组 |
| `cn.hutool.core.convert.Convert` | `T convert(Class<T> type,Object value)` | 转换值为指定类型 |
| `cn.hutool.core.convert.Convert` | `T convert(Class<T> type,Object value,T defaultValue)` | 转换值为指定类型 |
| `cn.hutool.core.convert.Convert` | `T convert(Type type,Object value)` | 转换值为指定类型 |
| `cn.hutool.core.convert.Convert` | `T convert(Type type,Object value,T defaultValue)` | 转换值为指定类型 |
| `cn.hutool.core.convert.Convert` | `T convert(TypeReference<T> reference,Object value)` | 转换值为指定类型 |
| `cn.hutool.core.convert.Convert` | `T convertByClassName(String className,Object value)` | 转换值为指定类型，类型采用字符串表示 |
| `cn.hutool.core.convert.Convert` | `T convertQuietly(Type type,Object value)` | 转换值为指定类型，不抛异常转换 当转换失败时返回null |
| `cn.hutool.core.convert.Convert` | `T convertQuietly(Type type,Object value,T defaultValue)` | 转换值为指定类型，不抛异常转换 当转换失败时返回默认值 |
| `cn.hutool.core.convert.Convert` | `T convertWithCheck(Type type,Object value,T defaultValue,boolean quietly)` | 转换值为指定类型，可选是否不抛异常转换 当转换失败时返回默认值 |
| `cn.hutool.core.convert.Convert` | `byte intToByte(int intValue)` | int转byte |
| `cn.hutool.core.convert.Convert` | `byte[] hexToBytes(String src)` | Hex字符串转换为Byte值 |
| `cn.hutool.core.convert.Convert` | `byte[] intToBytes(int intValue)` | int转byte数组 默认以小端序转换 |
| `cn.hutool.core.convert.Convert` | `byte[] longToBytes(long longValue)` | long转byte数组 默认以小端序转换 from: https://stackoverflow.com/questions/4485128/how-do-i-convert-long-to-byte-and-back-in-java |
| `cn.hutool.core.convert.Convert` | `byte[] shortToBytes(short shortValue)` | short转byte数组 默认以小端序转换 |
| `cn.hutool.core.convert.Convert` | `byte[] toPrimitiveByteArray(Object value)` | 转换为Byte数组 |
| `cn.hutool.core.convert.Convert` | `int byteToUnsignedInt(byte byteValue)` | byte转无符号int |
| `cn.hutool.core.convert.Convert` | `int bytesToInt(byte[] bytes)` | byte[]转int值 默认以小端序转换 |
| `cn.hutool.core.convert.Convert` | `int chineseToNumber(String number)` | 数字中文表示形式转数字 一百一十二 -》 112 一千零一十二 -》 1012 |
| `cn.hutool.core.convert.Convert` | `long bytesToLong(byte[] bytes)` | byte数组转long 默认以小端序转换 from: https://stackoverflow.com/questions/4485128/how-do-i-convert-long-to-byte-and-back-in-java |
| `cn.hutool.core.convert.Convert` | `long convertTime(long sourceDuration,TimeUnit sourceUnit,TimeUnit destUnit)` | 转换时间单位 |
| `cn.hutool.core.convert.Convert` | `short bytesToShort(byte[] bytes)` | byte数组转short 默认以小端序转换 |
| `cn.hutool.core.convert.Converter` | `T convert(Object value,T defaultValue)` | 转换为指定类型 如果类型无法确定，将读取默认值的类型做为目标类型 |
| `cn.hutool.core.convert.Converter` | `T convertWithCheck(Object value,T defaultValue,boolean quietly)` | 转换值为指定类型，可选是否不抛异常转换 当转换失败时返回默认值 |
| `cn.hutool.core.convert.ConverterRegistry` | `Converter<T> getConverter(Type type,boolean isCustomFirst)` | 获得转换器 |
| `cn.hutool.core.convert.ConverterRegistry` | `Converter<T> getCustomConverter(Type type)` | 获得自定义转换器 |
| `cn.hutool.core.convert.ConverterRegistry` | `Converter<T> getDefaultConverter(Type type)` | 获得默认转换器 |
| `cn.hutool.core.convert.ConverterRegistry` | `ConverterRegistry getInstance()` | 获得单例的 ConverterRegistry |
| `cn.hutool.core.convert.ConverterRegistry` | `ConverterRegistry putCustom(Type type,Class<? extends Converter<?>> converterClass)` | 登记自定义转换器 |
| `cn.hutool.core.convert.ConverterRegistry` | `ConverterRegistry putCustom(Type type,Converter<?> converter)` | 登记自定义转换器 |
| `cn.hutool.core.convert.ConverterRegistry` | `T convert(Type type,Object value)` | 转换值为指定类型 |
| `cn.hutool.core.convert.ConverterRegistry` | `T convert(Type type,Object value,T defaultValue)` | 转换值为指定类型 自定义转换器优先 |
| `cn.hutool.core.convert.ConverterRegistry` | `T convert(Type type,Object value,T defaultValue,boolean isCustomFirst)` | 转换值为指定类型 |
| `cn.hutool.core.convert.NumberChineseFormatter` | `BigDecimal chineseMoneyToNumber(String chineseMoneyAmount)` | 中文大写数字金额转换为数字，返回结果以元为单位的BigDecimal类型数字 如： “陆万柒仟伍佰伍拾陆元叁角贰分”返回“67556.32” “叁角贰分”返回“0.32” |
| `cn.hutool.core.convert.NumberChineseFormatter` | `String format(BigDecimal amount,boolean isUseTraditional,boolean isUseColloquial)` | 阿拉伯数字转换成中文. 使用于整数、小数的转换. 支持多位小数 |
| `cn.hutool.core.convert.NumberChineseFormatter` | `String format(double amount,boolean isUseTraditional)` | 阿拉伯数字转换成中文,小数点后四舍五入保留两位. 使用于整数、小数的转换. |
| `cn.hutool.core.convert.NumberChineseFormatter` | `String format(double amount,boolean isUseTraditional,boolean isMoneyMode)` | 阿拉伯数字转换成中文,小数点后四舍五入保留两位. 使用于整数、小数的转换. |
| `cn.hutool.core.convert.NumberChineseFormatter` | `String format(double amount,boolean isUseTraditional,boolean isMoneyMode,String negativeName,String unitName)` | 阿拉伯数字转换成中文. 主要是对发票票面金额转换的扩展 如：-12.32 发票票面转换为：(负数)壹拾贰圆叁角贰分 而非：负壹拾贰元叁角贰分 共两点不同：1、(负数) 而非 负；2、圆 而非 元 2022/3/9 |
| `cn.hutool.core.convert.NumberChineseFormatter` | `String format(long amount,boolean isUseTraditional)` | 阿拉伯数字（支持正负整数）转换成中文 |
| `cn.hutool.core.convert.NumberChineseFormatter` | `String formatSimple(long amount)` | 阿拉伯数字（支持正负整数）四舍五入后转换成中文节权位简洁计数单位，例如 -5_5555 =》 -5.56万 |
| `cn.hutool.core.convert.NumberChineseFormatter` | `String formatThousand(int amount,boolean isUseTraditional)` | 格式化-999~999之间的数字 这个方法显示10~19以下的数字时使用"十一"而非"一十一"。 |
| `cn.hutool.core.convert.NumberChineseFormatter` | `String numberCharToChinese(char c,boolean isUseTraditional)` | 数字字符转中文，非数字字符原样返回 |
| `cn.hutool.core.convert.NumberChineseFormatter` | `int chineseToNumber(String chinese)` | 把中文转换为数字 如 二百二十 220 一百一十二 -》 112 一千零一十二 -》 1012 |
| `cn.hutool.core.convert.NumberWithFormat` | `Object convert(Type targetType,Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.convert.NumberWithFormat` | `Object getNumber()` | 获取原始Number |
| `cn.hutool.core.convert.NumberWithFormat` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.convert.NumberWithFormat` | `double doubleValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.convert.NumberWithFormat` | `float floatValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.convert.NumberWithFormat` | `int compareTo(NumberWithFormat o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.convert.NumberWithFormat` | `int intValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.convert.NumberWithFormat` | `long longValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.convert.NumberWordFormatter` | `String format(Object x)` | 将阿拉伯数字转为英文表达式 |
| `cn.hutool.core.convert.NumberWordFormatter` | `String formatSimple(long value)` | 将阿拉伯数字转化为简洁计数单位，例如 2100 =》 2.1k 范围默认只到w |
| `cn.hutool.core.convert.NumberWordFormatter` | `String formatSimple(long value,boolean isTwo)` | 将阿拉伯数字转化为简介计数单位，例如 2100 =》 2.1k |
| `cn.hutool.core.convert.TypeConverter` | `Object convert(Type targetType,Object value)` | 转换为指定类型 如果类型无法确定，将读取默认值的类型做为目标类型 |
