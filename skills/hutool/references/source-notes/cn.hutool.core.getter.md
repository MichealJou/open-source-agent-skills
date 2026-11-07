# cn.hutool.core.getter

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.getter.ArrayTypeGetter` | `BigDecimal[] getBigDecimals(String key)` | 获取BigDecimal型属性值数组 |
| `cn.hutool.core.getter.ArrayTypeGetter` | `BigInteger[] getBigIntegers(String key)` | 获取BigInteger型属性值数组 |
| `cn.hutool.core.getter.ArrayTypeGetter` | `Boolean[] getBools(String key)` | 获取Boolean型属性值数组 |
| `cn.hutool.core.getter.ArrayTypeGetter` | `Byte[] getBytes(String key)` | 获取Byte型属性值数组 |
| `cn.hutool.core.getter.ArrayTypeGetter` | `Character[] getChars(String key)` | 获取Character型属性值数组 |
| `cn.hutool.core.getter.ArrayTypeGetter` | `Double[] getDoubles(String key)` | 获取Double型属性值数组 |
| `cn.hutool.core.getter.ArrayTypeGetter` | `Integer[] getInts(String key)` | 获取Integer型属性值数组 |
| `cn.hutool.core.getter.ArrayTypeGetter` | `Long[] getLongs(String key)` | 获取Long型属性值数组 |
| `cn.hutool.core.getter.ArrayTypeGetter` | `Short[] getShorts(String key)` | 获取Short型属性值数组 |
| `cn.hutool.core.getter.ArrayTypeGetter` | `String[] getObjs(String key)` | 获取Object型属性值数组 |
| `cn.hutool.core.getter.ArrayTypeGetter` | `String[] getStrs(String key)` | 获取String型属性值数组 |
| `cn.hutool.core.getter.BasicTypeGetter` | `BigDecimal getBigDecimal(K key)` | 获取BigDecimal型属性值 |
| `cn.hutool.core.getter.BasicTypeGetter` | `BigInteger getBigInteger(K key)` | 获取BigInteger型属性值 |
| `cn.hutool.core.getter.BasicTypeGetter` | `Boolean getBool(K key)` | 获取boolean型属性值 |
| `cn.hutool.core.getter.BasicTypeGetter` | `Byte getByte(K key)` | 获取byte型属性值 |
| `cn.hutool.core.getter.BasicTypeGetter` | `Character getChar(K key)` | 获取char型属性值 |
| `cn.hutool.core.getter.BasicTypeGetter` | `Date getDate(K key)` | 获取Date类型值 |
| `cn.hutool.core.getter.BasicTypeGetter` | `Double getDouble(K key)` | 获取double型属性值 |
| `cn.hutool.core.getter.BasicTypeGetter` | `E getEnum(Class<E> clazz,K key)` | 获得Enum类型的值 |
| `cn.hutool.core.getter.BasicTypeGetter` | `Float getFloat(K key)` | 获取float型属性值 |
| `cn.hutool.core.getter.BasicTypeGetter` | `Integer getInt(K key)` | 获取int型属性值 |
| `cn.hutool.core.getter.BasicTypeGetter` | `Long getLong(K key)` | 获取long型属性值 |
| `cn.hutool.core.getter.BasicTypeGetter` | `Object getObj(K key)` | 获取Object属性值 |
| `cn.hutool.core.getter.BasicTypeGetter` | `Short getShort(K key)` | 获取short型属性值 |
| `cn.hutool.core.getter.BasicTypeGetter` | `String getStr(K key)` | 获取字符串型属性值 |
| `cn.hutool.core.getter.GroupedTypeGetter` | `BigDecimal getBigDecimalByGroup(String key,String group)` | 获取BigDecimal型属性值 |
| `cn.hutool.core.getter.GroupedTypeGetter` | `BigInteger getBigIntegerByGroup(String key,String group)` | 获取BigInteger型属性值 |
| `cn.hutool.core.getter.GroupedTypeGetter` | `Boolean getBoolByGroup(String key,String group)` | 获取boolean型属性值 |
| `cn.hutool.core.getter.GroupedTypeGetter` | `Byte getByteByGroup(String key,String group)` | 获取byte型属性值 |
| `cn.hutool.core.getter.GroupedTypeGetter` | `Character getCharByGroup(String key,String group)` | 获取char型属性值 |
| `cn.hutool.core.getter.GroupedTypeGetter` | `Double getDoubleByGroup(String key,String group)` | 获取double型属性值 |
| `cn.hutool.core.getter.GroupedTypeGetter` | `Integer getIntByGroup(String key,String group)` | 获取int型属性值 |
| `cn.hutool.core.getter.GroupedTypeGetter` | `Long getLongByGroup(String key,String group)` | 获取Long型属性值 |
| `cn.hutool.core.getter.GroupedTypeGetter` | `Short getShortByGroup(String key,String group)` | 获取short型属性值 |
| `cn.hutool.core.getter.GroupedTypeGetter` | `String getStrByGroup(String key,String group)` | 获取字符串型属性值 |
| `cn.hutool.core.getter.ListTypeGetter` | `List<BigDecimal> getBigDecimalList(String key)` | 获取BigDecimal型属性值列表 |
| `cn.hutool.core.getter.ListTypeGetter` | `List<BigInteger> getBigIntegerList(String key)` | 获取BigInteger型属性值列表 |
| `cn.hutool.core.getter.ListTypeGetter` | `List<Boolean> getBoolList(String key)` | 获取Boolean型属性值列表 |
| `cn.hutool.core.getter.ListTypeGetter` | `List<Byte> getByteList(String key)` | 获取Byte型属性值列表 |
| `cn.hutool.core.getter.ListTypeGetter` | `List<Character> getCharList(String key)` | 获取Character型属性值列表 |
| `cn.hutool.core.getter.ListTypeGetter` | `List<Double> getDoubleList(String key)` | 获取Double型属性值列表 |
| `cn.hutool.core.getter.ListTypeGetter` | `List<Integer> getIntList(String key)` | 获取Integer型属性值列表 |
| `cn.hutool.core.getter.ListTypeGetter` | `List<Long> getLongList(String key)` | 获取Long型属性值列表 |
| `cn.hutool.core.getter.ListTypeGetter` | `List<Object> getObjList(String key)` | 获取Object型属性值列表 |
| `cn.hutool.core.getter.ListTypeGetter` | `List<Short> getShortList(String key)` | 获取Short型属性值列表 |
| `cn.hutool.core.getter.ListTypeGetter` | `List<String> getStrList(String key)` | 获取String型属性值列表 |
| `cn.hutool.core.getter.OptArrayTypeGetter` | `BigDecimal[] getBigDecimals(String key,BigDecimal[] defaultValue)` | 获取BigDecimal型属性值数组 |
| `cn.hutool.core.getter.OptArrayTypeGetter` | `BigInteger[] getBigIntegers(String key,BigInteger[] defaultValue)` | 获取BigInteger型属性值数组 |
| `cn.hutool.core.getter.OptArrayTypeGetter` | `Boolean[] getBools(String key,Boolean[] defaultValue)` | 获取Boolean型属性值数组 |
| `cn.hutool.core.getter.OptArrayTypeGetter` | `Byte[] getBytes(String key,Byte[] defaultValue)` | 获取Byte型属性值数组 |
| `cn.hutool.core.getter.OptArrayTypeGetter` | `Character[] getChars(String key,Character[] defaultValue)` | 获取Character型属性值数组 |
| `cn.hutool.core.getter.OptArrayTypeGetter` | `Double[] getDoubles(String key,Double[] defaultValue)` | 获取Double型属性值数组 |
| `cn.hutool.core.getter.OptArrayTypeGetter` | `Integer[] getInts(String key,Integer[] defaultValue)` | 获取Integer型属性值数组 |
| `cn.hutool.core.getter.OptArrayTypeGetter` | `Long[] getLongs(String key,Long[] defaultValue)` | 获取Long型属性值数组 |
| `cn.hutool.core.getter.OptArrayTypeGetter` | `Object[] getObjs(String key,Object[] defaultValue)` | 获取Object型属性值数组 |
| `cn.hutool.core.getter.OptArrayTypeGetter` | `Short[] getShorts(String key,Short[] defaultValue)` | 获取Short型属性值数组 |
| `cn.hutool.core.getter.OptArrayTypeGetter` | `String[] getStrs(String key,String[] defaultValue)` | 获取String型属性值数组 |
| `cn.hutool.core.getter.OptBasicTypeGetter` | `BigDecimal getBigDecimal(K key,BigDecimal defaultValue)` | 获取BigDecimal型属性值 若获得的值为不可见字符，使用默认值 |
| `cn.hutool.core.getter.OptBasicTypeGetter` | `BigInteger getBigInteger(K key,BigInteger defaultValue)` | 获取BigInteger型属性值 若获得的值为不可见字符，使用默认值 |
| `cn.hutool.core.getter.OptBasicTypeGetter` | `Boolean getBool(K key,Boolean defaultValue)` | 获取boolean型属性值 若获得的值为不可见字符，使用默认值 |
| `cn.hutool.core.getter.OptBasicTypeGetter` | `Byte getByte(K key,Byte defaultValue)` | 获取byte型属性值 若获得的值为不可见字符，使用默认值 |
| `cn.hutool.core.getter.OptBasicTypeGetter` | `Character getChar(K key,Character defaultValue)` | 获取char型属性值 若获得的值为不可见字符，使用默认值 |
| `cn.hutool.core.getter.OptBasicTypeGetter` | `Date getDate(K key,Date defaultValue)` | 获取Date类型值 |
| `cn.hutool.core.getter.OptBasicTypeGetter` | `Double getDouble(K key,Double defaultValue)` | 获取double型属性值 若获得的值为不可见字符，使用默认值 |
| `cn.hutool.core.getter.OptBasicTypeGetter` | `E getEnum(Class<E> clazz,K key,E defaultValue)` | 获得Enum类型的值 |
| `cn.hutool.core.getter.OptBasicTypeGetter` | `Float getFloat(K key,Float defaultValue)` | 获取float型属性值 若获得的值为不可见字符，使用默认值 |
| `cn.hutool.core.getter.OptBasicTypeGetter` | `Integer getInt(K key,Integer defaultValue)` | 获取int型属性值 若获得的值为不可见字符，使用默认值 |
| `cn.hutool.core.getter.OptBasicTypeGetter` | `Long getLong(K key,Long defaultValue)` | 获取Long型属性值 若获得的值为不可见字符，使用默认值 |
| `cn.hutool.core.getter.OptBasicTypeGetter` | `Object getObj(K key,Object defaultValue)` | 获取Object属性值 |
| `cn.hutool.core.getter.OptBasicTypeGetter` | `Short getShort(K key,Short defaultValue)` | 获取short型属性值 若获得的值为不可见字符，使用默认值 |
| `cn.hutool.core.getter.OptBasicTypeGetter` | `String getStr(K key,String defaultValue)` | 获取字符串型属性值 若获得的值为不可见字符，使用默认值 |
| `cn.hutool.core.getter.OptNullBasicTypeFromObjectGetter` | `BigDecimal getBigDecimal(K key,BigDecimal defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromObjectGetter` | `BigInteger getBigInteger(K key,BigInteger defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromObjectGetter` | `Boolean getBool(K key,Boolean defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromObjectGetter` | `Byte getByte(K key,Byte defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromObjectGetter` | `Character getChar(K key,Character defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromObjectGetter` | `Date getDate(K key,Date defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromObjectGetter` | `Double getDouble(K key,Double defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromObjectGetter` | `E getEnum(Class<E> clazz,K key,E defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromObjectGetter` | `Float getFloat(K key,Float defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromObjectGetter` | `Integer getInt(K key,Integer defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromObjectGetter` | `Long getLong(K key,Long defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromObjectGetter` | `Short getShort(K key,Short defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromObjectGetter` | `String getStr(K key,String defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromStringGetter` | `BigDecimal getBigDecimal(K key,BigDecimal defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromStringGetter` | `BigInteger getBigInteger(K key,BigInteger defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromStringGetter` | `Boolean getBool(K key,Boolean defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromStringGetter` | `Byte getByte(K key,Byte defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromStringGetter` | `Character getChar(K key,Character defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromStringGetter` | `Date getDate(K key,Date defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromStringGetter` | `Double getDouble(K key,Double defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromStringGetter` | `E getEnum(Class<E> clazz,K key,E defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromStringGetter` | `Float getFloat(K key,Float defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromStringGetter` | `Integer getInt(K key,Integer defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromStringGetter` | `Long getLong(K key,Long defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromStringGetter` | `Object getObj(K key,Object defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeFromStringGetter` | `Short getShort(K key,Short defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeGetter` | `BigDecimal getBigDecimal(K key)` | 获取BigDecimal型属性值 无值或获取错误返回null |
| `cn.hutool.core.getter.OptNullBasicTypeGetter` | `BigInteger getBigInteger(K key)` | 获取BigInteger型属性值 无值或获取错误返回null |
| `cn.hutool.core.getter.OptNullBasicTypeGetter` | `Boolean getBool(K key)` | 获取boolean型属性值 无值或获取错误返回null |
| `cn.hutool.core.getter.OptNullBasicTypeGetter` | `Byte getByte(K key)` | 获取byte型属性值 无值或获取错误返回null |
| `cn.hutool.core.getter.OptNullBasicTypeGetter` | `Character getChar(K key)` | 获取char型属性值 无值或获取错误返回null |
| `cn.hutool.core.getter.OptNullBasicTypeGetter` | `Date getDate(K key)` | 获取Date型属性值 无值或获取错误返回null |
| `cn.hutool.core.getter.OptNullBasicTypeGetter` | `Double getDouble(K key)` | 获取double型属性值 无值或获取错误返回null |
| `cn.hutool.core.getter.OptNullBasicTypeGetter` | `E getEnum(Class<E> clazz,K key)` | 获取Enum型属性值 无值或获取错误返回null |
| `cn.hutool.core.getter.OptNullBasicTypeGetter` | `Float getFloat(K key)` | 获取float型属性值 无值或获取错误返回null |
| `cn.hutool.core.getter.OptNullBasicTypeGetter` | `Integer getInt(K key)` | 获取int型属性值 无值或获取错误返回null |
| `cn.hutool.core.getter.OptNullBasicTypeGetter` | `Long getLong(K key)` | 获取long型属性值 无值或获取错误返回null |
| `cn.hutool.core.getter.OptNullBasicTypeGetter` | `Object getObj(K key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.getter.OptNullBasicTypeGetter` | `Short getShort(K key)` | 获取short型属性值 无值或获取错误返回null |
| `cn.hutool.core.getter.OptNullBasicTypeGetter` | `String getStr(K key)` | 获取字符串型属性值 无值或获取错误返回null |
