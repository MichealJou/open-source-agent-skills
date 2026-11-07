# cn.hutool.core.util

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.util.ArrayUtil` | `Class<?> getArrayType(Class<?> componentType)` | 根据数组元素类型，获取数组的类型 方法是通过创建一个空数组从而获取其类型 |
| `cn.hutool.core.util.ArrayUtil` | `Class<?> getComponentType(Class<?> arrayClass)` | 获取数组对象的元素类型 |
| `cn.hutool.core.util.ArrayUtil` | `Class<?> getComponentType(Object array)` | 获取数组对象的元素类型 |
| `cn.hutool.core.util.ArrayUtil` | `List<R> map(T[] array,Function<? super T, ? extends R> func)` | 按照指定规则，将一种类型的数组元素提取后转换为List |
| `cn.hutool.core.util.ArrayUtil` | `Map<K, V> zip(K[] keys,V[] values)` | 映射键值（参考Python的zip()函数），返回Map无序 例如： keys = [a,b,c,d] values = [1,2,3,4] 则得到的Map是 {a=1, b=2, c=3, d=4} 如果两个数组长度不同，则只对应最短部分 |
| `cn.hutool.core.util.ArrayUtil` | `Map<K, V> zip(K[] keys,V[] values,boolean isOrder)` | 映射键值（参考Python的zip()函数） 例如： keys = [a,b,c,d] values = [1,2,3,4] 则得到的Map是 {a=1, b=2, c=3, d=4} 如果两个数组长度不同，则只对应最短部分 |
| `cn.hutool.core.util.ArrayUtil` | `Object append(Object array,T... newElements)` | 将新元素添加到已有数组中 添加新元素会生成一个新的数组，不影响原数组 |
| `cn.hutool.core.util.ArrayUtil` | `Object copy(Object src,Object dest,int length)` | 包装 System#arraycopy(Object, int, Object, int, int) 数组复制，缘数组和目标数组都是从位置0开始复制 |
| `cn.hutool.core.util.ArrayUtil` | `Object copy(Object src,int srcPos,Object dest,int destPos,int length)` | 包装 System#arraycopy(Object, int, Object, int, int) 数组复制 |
| `cn.hutool.core.util.ArrayUtil` | `Object insert(Object array,int index,T... newElements)` | 将新元素插入到到已有数组中的某个位置 添加新元素会生成一个新的数组，不影响原数组 如果插入位置为为负数，从原数组从后向前计数，若大于原数组长度，则空白处用null填充 |
| `cn.hutool.core.util.ArrayUtil` | `Object resize(Object array,int newSize)` | 生成一个新的重新设置大小的数组 调整大小后拷贝原数组到新数组下。扩大则占位前N个位置，其它位置补充0，缩小则截断 |
| `cn.hutool.core.util.ArrayUtil` | `Object setOrAppend(Object array,int index,Object value)` | 将元素值设置为数组的某个位置，当给定的index大于数组长度，则追加 替换时返回原数组，追加时返回新数组 |
| `cn.hutool.core.util.ArrayUtil` | `Object swap(Object array,int index1,int index2)` | 交换数组中两个位置的值 |
| `cn.hutool.core.util.ArrayUtil` | `Object[] cast(Class<?> type,Object arrayObj)` | 强转数组类型 强制转换的前提是数组元素类型可被强制转换 强制转换后会生成一个新数组 |
| `cn.hutool.core.util.ArrayUtil` | `Object[] newArray(int newSize)` | 新建一个空数组 |
| `cn.hutool.core.util.ArrayUtil` | `Object[] sub(Object array,int start,int end)` | 获取子数组 |
| `cn.hutool.core.util.ArrayUtil` | `Object[] sub(Object array,int start,int end,int step)` | 获取子数组 |
| `cn.hutool.core.util.ArrayUtil` | `Object[] wrap(Object obj)` | 包装数组对象 |
| `cn.hutool.core.util.ArrayUtil` | `R[] map(Object array,Class<R> targetComponentType,Function<? super T, ? extends R> func)` | 按照指定规则，将一种类型的数组转换为另一种类型 |
| `cn.hutool.core.util.ArrayUtil` | `R[] map(T[] array,Class<R> targetComponentType,Function<? super T, ? extends R> func)` | 按照指定规则，将一种类型的数组转换为另一种类型 |
| `cn.hutool.core.util.ArrayUtil` | `Set<R> mapToSet(T[] array,Function<? super T, ? extends R> func)` | 按照指定规则，将一种类型的数组元素提取后转换为Set |
| `cn.hutool.core.util.ArrayUtil` | `String join(Object array,CharSequence conjunction)` | 以 conjunction 为分隔符将数组转换为字符串 |
| `cn.hutool.core.util.ArrayUtil` | `String join(T[] array,CharSequence conjunction)` | 以 conjunction 为分隔符将数组转换为字符串 |
| `cn.hutool.core.util.ArrayUtil` | `String join(T[] array,CharSequence conjunction,Editor<T> editor)` | 以 conjunction 为分隔符将数组转换为字符串 |
| `cn.hutool.core.util.ArrayUtil` | `String join(T[] array,CharSequence delimiter,String prefix,String suffix)` | 以 conjunction 为分隔符将数组转换为字符串 |
| `cn.hutool.core.util.ArrayUtil` | `String toString(Object obj)` | 数组或集合转String |
| `cn.hutool.core.util.ArrayUtil` | `String[] nullToEmpty(String[] array)` | 数组元素中的null转换为"" |
| `cn.hutool.core.util.ArrayUtil` | `T clone(final T obj)` | 克隆数组，如果非数组返回null |
| `cn.hutool.core.util.ArrayUtil` | `T firstMatch(Matcher<T> matcher,T... array)` | 返回数组中第一个匹配规则的值 |
| `cn.hutool.core.util.ArrayUtil` | `T firstNonNull(T... array)` | 返回数组中第一个非空元素 |
| `cn.hutool.core.util.ArrayUtil` | `T get(Object array,int index)` | 获取数组对象中指定index的值，支持负数，例如-1表示倒数第一个值 如果数组下标越界，返回null |
| `cn.hutool.core.util.ArrayUtil` | `T max(T[] numberArray)` | 取最大值 |
| `cn.hutool.core.util.ArrayUtil` | `T max(T[] numberArray,Comparator<T> comparator)` | 取最大值 |
| `cn.hutool.core.util.ArrayUtil` | `T min(T[] numberArray)` | 取最小值 |
| `cn.hutool.core.util.ArrayUtil` | `T min(T[] numberArray,Comparator<T> comparator)` | 取最小值 |
| `cn.hutool.core.util.ArrayUtil` | `T[] addAll(T[]... arrays)` | 将多个数组合并在一起 忽略null的数组 |
| `cn.hutool.core.util.ArrayUtil` | `T[] append(T[] buffer,T... newElements)` | 将新元素添加到已有数组中 添加新元素会生成一个新的数组，不影响原数组 |
| `cn.hutool.core.util.ArrayUtil` | `T[] clone(T[] array)` | 克隆数组 |
| `cn.hutool.core.util.ArrayUtil` | `T[] defaultIfEmpty(T[] array,T[] defaultArray)` | 如果给定数组为空，返回默认数组 |
| `cn.hutool.core.util.ArrayUtil` | `T[] distinct(T[] array)` | 去重数组中的元素，去重后生成新的数组，原数组不变 此方法通过LinkedHashSet 去重 |
| `cn.hutool.core.util.ArrayUtil` | `T[] distinct(T[] array,Function<T, K> uniqueGenerator,boolean override)` | 去重数组中的元素，去重后生成新的数组，原数组不变 此方法通过LinkedHashSet 去重 |
| `cn.hutool.core.util.ArrayUtil` | `T[] edit(T[] array,Editor<T> editor)` | 编辑数组 编辑过程通过传入的Editor实现来返回需要的元素内容，这个Editor实现可以实现以下功能： |
| `cn.hutool.core.util.ArrayUtil` | `T[] filter(T[] array,Filter<T> filter)` | 过滤 过滤过程通过传入的Filter实现来过滤返回需要的元素内容，这个Filter实现可以实现以下功能： |
| `cn.hutool.core.util.ArrayUtil` | `T[] getAny(Object array,int... indexes)` | 获取数组中指定多个下标元素值，组成新数组 |
| `cn.hutool.core.util.ArrayUtil` | `T[] insert(T[] buffer,int index,T... newElements)` | 将新元素插入到到已有数组中的某个位置 添加新元素会生成一个新的数组，不影响原数组 如果插入位置为为负数，从原数组从后向前计数，若大于原数组长度，则空白处用null填充 |
| `cn.hutool.core.util.ArrayUtil` | `T[] newArray(Class<?> componentType,int newSize)` | 新建一个空数组 |
| `cn.hutool.core.util.ArrayUtil` | `T[] remove(T[] array,int index)` | 移除数组中对应位置的元素 copy from commons-lang |
| `cn.hutool.core.util.ArrayUtil` | `T[] removeBlank(T[] array)` | 去除null或者""或者空白字符串 元素 |
| `cn.hutool.core.util.ArrayUtil` | `T[] removeEle(T[] array,T element)` | 移除数组中指定的元素 只会移除匹配到的第一个元素 copy from commons-lang |
| `cn.hutool.core.util.ArrayUtil` | `T[] removeEmpty(T[] array)` | 去除null或者"" 元素 |
| `cn.hutool.core.util.ArrayUtil` | `T[] removeNull(T[] array)` | 去除null 元素 |
| `cn.hutool.core.util.ArrayUtil` | `T[] replace(T[] buffer,int index,T... values)` | 将新元素插入到到已有数组中的某个位置 添加新元素会生成一个新数组或原有数组 如果插入位置为为负数，那么生成一个由插入元素顺序加已有数组顺序的新数组 |
| `cn.hutool.core.util.ArrayUtil` | `T[] resize(T[] buffer,int newSize)` | 生成一个新的重新设置大小的数组 新数组的类型为原数组的类型，调整大小后拷贝原数组到新数组下。扩大则占位前N个位置，缩小则截断 |
| `cn.hutool.core.util.ArrayUtil` | `T[] resize(T[] data,int newSize,Class<?> componentType)` | 生成一个新的重新设置大小的数组 调整大小后拷贝原数组到新数组下。扩大则占位前N个位置，缩小则截断 |
| `cn.hutool.core.util.ArrayUtil` | `T[] reverse(T[] array)` | 反转数组，会变更原数组 |
| `cn.hutool.core.util.ArrayUtil` | `T[] reverse(T[] array,final int startIndexInclusive,final int endIndexExclusive)` | 反转数组，会变更原数组 |
| `cn.hutool.core.util.ArrayUtil` | `T[] setOrAppend(T[] buffer,int index,T value)` | 将元素值设置为数组的某个位置，当给定的index大于数组长度，则追加 |
| `cn.hutool.core.util.ArrayUtil` | `T[] shuffle(T[] array)` | 打乱数组顺序，会变更原数组 |
| `cn.hutool.core.util.ArrayUtil` | `T[] shuffle(T[] array,Random random)` | 打乱数组顺序，会变更原数组 |
| `cn.hutool.core.util.ArrayUtil` | `T[] sub(T[] array,int start,int end)` | 获取子数组 |
| `cn.hutool.core.util.ArrayUtil` | `T[] swap(T[] array,int index1,int index2)` | 交换数组中两个位置的值 |
| `cn.hutool.core.util.ArrayUtil` | `T[] toArray(Collection<T> collection,Class<T> componentType)` | 将集合转为数组 |
| `cn.hutool.core.util.ArrayUtil` | `T[] toArray(Iterable<T> iterable,Class<T> componentType)` | 将集合转为数组 |
| `cn.hutool.core.util.ArrayUtil` | `T[] toArray(Iterator<T> iterator,Class<T> componentType)` | 将集合转为数组 |
| `cn.hutool.core.util.ArrayUtil` | `boolean contains(T[] array,T value)` | 数组中是否包含元素 |
| `cn.hutool.core.util.ArrayUtil` | `boolean containsAll(T[] array,T... values)` | 数组中是否包含指定元素中的全部 |
| `cn.hutool.core.util.ArrayUtil` | `boolean containsAny(T[] array,T... values)` | 数组中是否包含指定元素中的任意一个 |
| `cn.hutool.core.util.ArrayUtil` | `boolean containsIgnoreCase(CharSequence[] array,CharSequence value)` | 数组中是否包含元素，忽略大小写 |
| `cn.hutool.core.util.ArrayUtil` | `boolean equals(Object array1,Object array2)` | 判断两个数组是否相等，判断依据包括数组长度和每个元素都相等。 |
| `cn.hutool.core.util.ArrayUtil` | `boolean hasEmpty(Object... args)` | 是否存在null或空对象，通过ObjectUtil#isEmpty(Object) 判断元素 |
| `cn.hutool.core.util.ArrayUtil` | `boolean hasNull(T... array)` | 是否包含null元素 |
| `cn.hutool.core.util.ArrayUtil` | `boolean isAllEmpty(Object... args)` | 是否全都为null或空对象，通过ObjectUtil#isEmpty(Object) 判断元素 |
| `cn.hutool.core.util.ArrayUtil` | `boolean isAllNotEmpty(Object... args)` | 是否全都不为null或空对象，通过ObjectUtil#isEmpty(Object) 判断元素 |
| `cn.hutool.core.util.ArrayUtil` | `boolean isAllNotNull(T... array)` | 多个字段是否全部不为null |
| `cn.hutool.core.util.ArrayUtil` | `boolean isAllNull(T... array)` | 多个字段是否全为null |
| `cn.hutool.core.util.ArrayUtil` | `boolean isArray(Object obj)` | 对象是否为数组对象 |
| `cn.hutool.core.util.ArrayUtil` | `boolean isEmpty(Object array)` | 数组是否为空 此方法会匹配单一对象，如果此对象为null则返回true 如果此对象为非数组，理解为此对象为数组的第一个元素，则返回false 如果此对象为数组对象，数组长度大于0情况下返回false，否则返回true |
| `cn.hutool.core.util.ArrayUtil` | `boolean isEmpty(T[] array)` | 数组是否为空 |
| `cn.hutool.core.util.ArrayUtil` | `boolean isNotEmpty(Object array)` | 数组是否为非空 此方法会匹配单一对象，如果此对象为null则返回false 如果此对象为非数组，理解为此对象为数组的第一个元素，则返回true 如果此对象为数组对象，数组长度大于0情况下返回true，否则返回false |
| `cn.hutool.core.util.ArrayUtil` | `boolean isNotEmpty(T[] array)` | 数组是否为非空 |
| `cn.hutool.core.util.ArrayUtil` | `boolean isSorted(T[] array)` | 检查数组是否升序，即array[i].compareTo(array[i + 1]) <= 0，若传入空数组，则返回false |
| `cn.hutool.core.util.ArrayUtil` | `boolean isSorted(T[] array,Comparator<? super T> comparator)` | 检查数组是否有序，即comparator.compare(array[i], array[i + 1]) <= 0，若传入空数组或空比较器，则返回false |
| `cn.hutool.core.util.ArrayUtil` | `boolean isSortedASC(T[] array)` | 检查数组是否升序，即array[i].compareTo(array[i + 1]) <= 0，若传入空数组，则返回false |
| `cn.hutool.core.util.ArrayUtil` | `boolean isSortedDESC(T[] array)` | 检查数组是否降序，即array[i].compareTo(array[i + 1]) >= 0，若传入空数组，则返回false |
| `cn.hutool.core.util.ArrayUtil` | `boolean isSub(T[] array,T[] subArray)` | 查找子数组的位置 |
| `cn.hutool.core.util.ArrayUtil` | `byte[] toArray(ByteBuffer bytebuffer)` | ByteBuffer 转byte数组 |
| `cn.hutool.core.util.ArrayUtil` | `int emptyCount(Object... args)` | 计算null或空元素对象的个数，通过ObjectUtil#isEmpty(Object) 判断元素 |
| `cn.hutool.core.util.ArrayUtil` | `int indexOf(T[] array,Object value)` | 返回数组中指定元素所在位置，未找到返回#INDEX_NOT_FOUND |
| `cn.hutool.core.util.ArrayUtil` | `int indexOf(T[] array,Object value,int beginIndexInclude)` | 返回数组中指定元素所在位置，未找到返回#INDEX_NOT_FOUND |
| `cn.hutool.core.util.ArrayUtil` | `int indexOfIgnoreCase(CharSequence[] array,CharSequence value)` | 返回数组中指定元素所在位置，忽略大小写，未找到返回#INDEX_NOT_FOUND |
| `cn.hutool.core.util.ArrayUtil` | `int indexOfSub(T[] array,T[] subArray)` | 查找子数组的位置 |
| `cn.hutool.core.util.ArrayUtil` | `int indexOfSub(T[] array,int beginInclude,T[] subArray)` | 查找子数组的位置 |
| `cn.hutool.core.util.ArrayUtil` | `int lastIndexOf(T[] array,Object value)` | 返回数组中指定元素所在最后的位置，未找到返回#INDEX_NOT_FOUND |
| `cn.hutool.core.util.ArrayUtil` | `int lastIndexOf(T[] array,Object value,int endInclude)` | 返回数组中指定元素所在最后的位置，未找到返回#INDEX_NOT_FOUND |
| `cn.hutool.core.util.ArrayUtil` | `int lastIndexOfSub(T[] array,T[] subArray)` | 查找最后一个子数组的开始位置 |
| `cn.hutool.core.util.ArrayUtil` | `int lastIndexOfSub(T[] array,int endInclude,T[] subArray)` | 查找最后一个子数组的开始位置 |
| `cn.hutool.core.util.ArrayUtil` | `int length(Object array)` | 获取数组长度 如果参数为null，返回0 |
| `cn.hutool.core.util.ArrayUtil` | `int matchIndex(Matcher<T> matcher,T... array)` | 返回数组中第一个匹配规则的值的位置 |
| `cn.hutool.core.util.ArrayUtil` | `int matchIndex(Matcher<T> matcher,int beginIndexInclude,T... array)` | 返回数组中第一个匹配规则的值的位置 |
| `cn.hutool.core.util.BooleanUtil` | `Boolean andOfWrap(Boolean... array)` | 对Boolean数组取与 |
| `cn.hutool.core.util.BooleanUtil` | `Boolean negate(Boolean bool)` | 取相反值 |
| `cn.hutool.core.util.BooleanUtil` | `Boolean orOfWrap(Boolean... array)` | 对Boolean数组取或 |
| `cn.hutool.core.util.BooleanUtil` | `Boolean toBooleanObject(String valueStr)` | 转换字符串为boolean值 如果为["true", "yes", "y", "t", "ok", "1", "on", "是", "对", "真", "對", "√"]，返回true 如果为["false", "no", "n", "f", "0", "off", "否", "错", "假", "錯", "×"]，返回false 其他情况返回null |
| `cn.hutool.core.util.BooleanUtil` | `Boolean xorOfWrap(Boolean... array)` | 对Boolean数组取异或 |
| `cn.hutool.core.util.BooleanUtil` | `Byte toByteObj(boolean value)` | boolean值转为Byte |
| `cn.hutool.core.util.BooleanUtil` | `Character toCharacter(boolean value)` | boolean值转为Character |
| `cn.hutool.core.util.BooleanUtil` | `Double toDoubleObj(boolean value)` | boolean值转为double |
| `cn.hutool.core.util.BooleanUtil` | `Float toFloatObj(boolean value)` | boolean值转为Float |
| `cn.hutool.core.util.BooleanUtil` | `Integer toInteger(boolean value)` | boolean值转为Integer |
| `cn.hutool.core.util.BooleanUtil` | `Long toLongObj(boolean value)` | boolean值转为Long |
| `cn.hutool.core.util.BooleanUtil` | `Short toShortObj(boolean value)` | boolean值转为Short |
| `cn.hutool.core.util.BooleanUtil` | `String toString(Boolean bool,String trueString,String falseString,String nullString)` | 将boolean转换为字符串 |
| `cn.hutool.core.util.BooleanUtil` | `String toString(boolean bool,String trueString,String falseString)` | 将boolean转换为字符串 |
| `cn.hutool.core.util.BooleanUtil` | `String toStringOnOff(boolean bool)` | 将boolean转换为字符串 'on' 或者 'off'. |
| `cn.hutool.core.util.BooleanUtil` | `String toStringTrueFalse(boolean bool)` | 将boolean转换为字符串 'true' 或者 'false'. |
| `cn.hutool.core.util.BooleanUtil` | `String toStringYesNo(boolean bool)` | 将boolean转换为字符串 'yes' 或者 'no'. |
| `cn.hutool.core.util.BooleanUtil` | `boolean and(boolean... array)` | 对Boolean数组取与 |
| `cn.hutool.core.util.BooleanUtil` | `boolean exactlyOneTrue(final boolean... array)` | 判断 boolean 数组中是否 恰好只有一个 元素为 true。 常用于互斥条件校验场景，例如： 多个角色只能同时存在一个 多个条件只能命中一个分支 与 #xor(boolean...) 不同， 本方法在出现多个 true 时会直接返回 false。 |
| `cn.hutool.core.util.BooleanUtil` | `boolean isBoolean(Class<?> clazz)` | 给定类是否为Boolean或者boolean |
| `cn.hutool.core.util.BooleanUtil` | `boolean isFalse(Boolean bool)` | 检查 Boolean 值是否为 false |
| `cn.hutool.core.util.BooleanUtil` | `boolean isTrue(Boolean bool)` | 检查 Boolean 值是否为 true |
| `cn.hutool.core.util.BooleanUtil` | `boolean negate(boolean bool)` | 取相反值 |
| `cn.hutool.core.util.BooleanUtil` | `boolean or(boolean... array)` | 对Boolean数组取或 |
| `cn.hutool.core.util.BooleanUtil` | `boolean toBoolean(String valueStr)` | 转换字符串为boolean值 |
| `cn.hutool.core.util.BooleanUtil` | `boolean xor(boolean... array)` | 对Boolean数组取异或 当前实现的语义为：当数组中 true 的数量为奇数时返回 true，数量为偶数时返回 false。 注意：该方法并不是判断“是否恰好只有一个 true”， 不适用于互斥条件校验（例如：多个条件只能有一个成立的场景）。 |
| `cn.hutool.core.util.BooleanUtil` | `byte toByte(boolean value)` | boolean值转为byte |
| `cn.hutool.core.util.BooleanUtil` | `char toChar(boolean value)` | boolean值转为char |
| `cn.hutool.core.util.BooleanUtil` | `double toDouble(boolean value)` | boolean值转为double |
| `cn.hutool.core.util.BooleanUtil` | `float toFloat(boolean value)` | boolean值转为float |
| `cn.hutool.core.util.BooleanUtil` | `int toInt(boolean value)` | boolean值转为int |
| `cn.hutool.core.util.BooleanUtil` | `long toLong(boolean value)` | boolean值转为long |
| `cn.hutool.core.util.BooleanUtil` | `short toShort(boolean value)` | boolean值转为short |
| `cn.hutool.core.util.ByteUtil` | `T bytesToNumber(byte[] bytes,Class<T> targetClass,ByteOrder byteOrder)` | byte数组转换为指定类型数字 |
| `cn.hutool.core.util.ByteUtil` | `byte intToByte(int intValue)` | int转byte |
| `cn.hutool.core.util.ByteUtil` | `byte[] doubleToBytes(double doubleValue)` | double转byte数组 默认以小端序转换 |
| `cn.hutool.core.util.ByteUtil` | `byte[] doubleToBytes(double doubleValue,ByteOrder byteOrder)` | double转byte数组 自定义端序 from: https://stackoverflow.com/questions/4485128/how-do-i-convert-long-to-byte-and-back-in-java |
| `cn.hutool.core.util.ByteUtil` | `byte[] floatToBytes(float floatValue)` | float转byte数组，默认以小端序转换 |
| `cn.hutool.core.util.ByteUtil` | `byte[] floatToBytes(float floatValue,ByteOrder byteOrder)` | float转byte数组，自定义端序 |
| `cn.hutool.core.util.ByteUtil` | `byte[] intToBytes(int intValue)` | int转byte数组 默认以小端序转换 |
| `cn.hutool.core.util.ByteUtil` | `byte[] intToBytes(int intValue,ByteOrder byteOrder)` | int转byte数组 自定义端序 |
| `cn.hutool.core.util.ByteUtil` | `byte[] longToBytes(long longValue)` | long转byte数组 默认以小端序转换 from: https://stackoverflow.com/questions/4485128/how-do-i-convert-long-to-byte-and-back-in-java |
| `cn.hutool.core.util.ByteUtil` | `byte[] longToBytes(long longValue,ByteOrder byteOrder)` | long转byte数组 自定义端序 from: https://stackoverflow.com/questions/4485128/how-do-i-convert-long-to-byte-and-back-in-java |
| `cn.hutool.core.util.ByteUtil` | `byte[] numberToBytes(Number number)` | 将Number转换为 |
| `cn.hutool.core.util.ByteUtil` | `byte[] numberToBytes(Number number,ByteOrder byteOrder)` | 将Number转换为 |
| `cn.hutool.core.util.ByteUtil` | `byte[] shortToBytes(short shortValue)` | short转byte数组 默认以小端序转换 |
| `cn.hutool.core.util.ByteUtil` | `byte[] shortToBytes(short shortValue,ByteOrder byteOrder)` | short转byte数组 自定义端序 |
| `cn.hutool.core.util.ByteUtil` | `double bytesToDouble(byte[] bytes)` | byte数组转Double 默认以小端序转换 |
| `cn.hutool.core.util.ByteUtil` | `double bytesToDouble(byte[] bytes,ByteOrder byteOrder)` | byte数组转double 自定义端序 |
| `cn.hutool.core.util.ByteUtil` | `float bytesToFloat(byte[] bytes)` | byte数组转float 默认以小端序转换 |
| `cn.hutool.core.util.ByteUtil` | `float bytesToFloat(byte[] bytes,ByteOrder byteOrder)` | byte数组转float 自定义端序 |
| `cn.hutool.core.util.ByteUtil` | `int byteToUnsignedInt(byte byteValue)` | byte转无符号int |
| `cn.hutool.core.util.ByteUtil` | `int bytesToInt(byte[] bytes)` | byte[]转int值 默认以小端序转换 |
| `cn.hutool.core.util.ByteUtil` | `int bytesToInt(byte[] bytes,ByteOrder byteOrder)` | byte[]转int值 自定义端序 |
| `cn.hutool.core.util.ByteUtil` | `int bytesToInt(byte[] bytes,int start,ByteOrder byteOrder)` | byte[]转int值 自定义端序 |
| `cn.hutool.core.util.ByteUtil` | `long bytesToLong(byte[] bytes)` | byte数组转long 默认以小端序转换 from: https://stackoverflow.com/questions/4485128/how-do-i-convert-long-to-byte-and-back-in-java |
| `cn.hutool.core.util.ByteUtil` | `long bytesToLong(byte[] bytes,ByteOrder byteOrder)` | byte数组转long 自定义端序 from: https://stackoverflow.com/questions/4485128/how-do-i-convert-long-to-byte-and-back-in-java |
| `cn.hutool.core.util.ByteUtil` | `long bytesToLong(byte[] bytes,int start,ByteOrder byteOrder)` | byte数组转long 自定义端序 from: https://stackoverflow.com/questions/4485128/how-do-i-convert-long-to-byte-and-back-in-java |
| `cn.hutool.core.util.ByteUtil` | `short bytesToShort(byte[] bytes)` | byte数组转short 默认以小端序转换 |
| `cn.hutool.core.util.ByteUtil` | `short bytesToShort(final byte[] bytes,final ByteOrder byteOrder)` | byte数组转short 自定义端序 |
| `cn.hutool.core.util.ByteUtil` | `short bytesToShort(final byte[] bytes,final int start,final ByteOrder byteOrder)` | byte数组转short 自定义端序 |
| `cn.hutool.core.util.CharUtil` | `String toString(char c)` | 字符转为字符串 如果为ASCII字符，使用缓存 |
| `cn.hutool.core.util.CharUtil` | `boolean equals(char c1,char c2,boolean caseInsensitive)` | 比较两个字符是否相同 |
| `cn.hutool.core.util.CharUtil` | `boolean isAscii(char ch)` | 是否为ASCII字符，ASCII字符位于0~127之间 |
| `cn.hutool.core.util.CharUtil` | `boolean isAsciiControl(final char ch)` | 是否为ASCII控制符（不可见字符），控制符位于0~31和127 |
| `cn.hutool.core.util.CharUtil` | `boolean isAsciiPrintable(char ch)` | 是否为可见ASCII字符，可见字符位于32~126之间 |
| `cn.hutool.core.util.CharUtil` | `boolean isBlankChar(char c)` | 是否空白符 空白符包括空格、制表符、全角空格和不间断空格 |
| `cn.hutool.core.util.CharUtil` | `boolean isBlankChar(int c)` | 是否空白符 空白符包括空格、制表符、全角空格和不间断空格 |
| `cn.hutool.core.util.CharUtil` | `boolean isChar(Object value)` | 给定对象对应的类是否为字符类，字符类包括： |
| `cn.hutool.core.util.CharUtil` | `boolean isCharClass(Class<?> clazz)` | 给定类名是否为字符类，字符类包括： |
| `cn.hutool.core.util.CharUtil` | `boolean isEmoji(char c)` | 判断是否为emoji表情符 |
| `cn.hutool.core.util.CharUtil` | `boolean isFileSeparator(char c)` | 是否为Windows或者Linux（Unix）文件分隔符 Windows平台下分隔符为\，Linux（Unix）为/ |
| `cn.hutool.core.util.CharUtil` | `boolean isHexChar(char c)` | 是否为16进制规范的字符，判断是否为如下字符 |
| `cn.hutool.core.util.CharUtil` | `boolean isLetter(char ch)` | 判断是否为字母（包括大写字母和小写字母） 字母包括A~Z和a~z |
| `cn.hutool.core.util.CharUtil` | `boolean isLetterLower(final char ch)` | 检查字符是否为小写字母，小写字母指a~z |
| `cn.hutool.core.util.CharUtil` | `boolean isLetterOrNumber(final char ch)` | 是否为字母或数字，包括A~Z、a~z、0~9 |
| `cn.hutool.core.util.CharUtil` | `boolean isLetterUpper(final char ch)` | 判断是否为大写字母，大写字母包括A~Z |
| `cn.hutool.core.util.CharUtil` | `boolean isNumber(char ch)` | 检查是否为数字字符，数字字符指0~9 |
| `cn.hutool.core.util.CharUtil` | `char toCloseByNumber(int number)` | 将[1-20]数字转换为带圈的字符： |
| `cn.hutool.core.util.CharUtil` | `char toCloseChar(char c)` | 将字母、数字转换为带圈的字符： |
| `cn.hutool.core.util.CharUtil` | `int digit16(int b)` | 获取给定字符的16进制数值 |
| `cn.hutool.core.util.CharUtil` | `int getType(int c)` | 获取字符类型 |
| `cn.hutool.core.util.CharsetUtil` | `Charset charset(String charsetName)` | 转换为Charset对象 |
| `cn.hutool.core.util.CharsetUtil` | `Charset defaultCharset()` | 系统默认字符集编码 |
| `cn.hutool.core.util.CharsetUtil` | `Charset defaultCharset(InputStream in,Charset... charsets)` | 探测编码 注意：此方法会读取流的一部分，然后关闭流，如重复使用流，请使用使用支持reset方法的流 |
| `cn.hutool.core.util.CharsetUtil` | `Charset defaultCharset(int bufferSize,InputStream in,Charset... charsets)` | 探测编码 注意：此方法会读取流的一部分，然后关闭流，如重复使用流，请使用使用支持reset方法的流 |
| `cn.hutool.core.util.CharsetUtil` | `Charset parse(String charsetName)` | 解析字符串编码为Charset对象，解析失败返回系统默认编码 |
| `cn.hutool.core.util.CharsetUtil` | `Charset parse(String charsetName,Charset defaultCharset)` | 解析字符串编码为Charset对象，解析失败返回默认编码 |
| `cn.hutool.core.util.CharsetUtil` | `Charset systemCharset()` | 系统字符集编码，如果是Windows，则默认为GBK编码，否则取 CharsetUtil#defaultCharsetName() |
| `cn.hutool.core.util.CharsetUtil` | `File convert(File file,Charset srcCharset,Charset destCharset)` | 转换文件编码 此方法用于转换文件编码，读取的文件实际编码必须与指定的srcCharset编码一致，否则导致乱码 |
| `cn.hutool.core.util.CharsetUtil` | `String convert(String source,Charset srcCharset,Charset destCharset)` | 转换字符串的字符集编码 当以错误的编码读取为字符串时，打印字符串将出现乱码。 此方法用于纠正因读取使用编码错误导致的乱码问题。 例如，在Servlet请求中客户端用GBK编码了请求参数，我们使用UTF-8读取到的是乱码，此时，使用此方法即可还原原编码的内容 |
| `cn.hutool.core.util.CharsetUtil` | `String convert(String source,String srcCharset,String destCharset)` | 转换字符串的字符集编码 |
| `cn.hutool.core.util.CharsetUtil` | `String defaultCharsetName()` | 系统默认字符集编码 |
| `cn.hutool.core.util.CharsetUtil` | `String systemCharsetName()` | 系统字符集编码，如果是Windows，则默认为GBK编码，否则取 CharsetUtil#defaultCharsetName() |
| `cn.hutool.core.util.ClassLoaderUtil` | `Class<?> loadClass(File jarOrDir,String name)` | 加载外部类 |
| `cn.hutool.core.util.ClassLoaderUtil` | `Class<?> loadClass(String name)` | 加载类，通过传入类的字符串，返回其对应的类名，使用默认ClassLoader并初始化类（调用static模块内容和初始化static属性） 扩展Class#forName(String, boolean, ClassLoader)方法，支持以下几类类名的加载： |
| `cn.hutool.core.util.ClassLoaderUtil` | `Class<?> loadClass(String name,ClassLoader classLoader,boolean isInitialized)` | 加载类，通过传入类的字符串，返回其对应的类名 此方法支持缓存，第一次被加载的类之后会读取缓存中的类 加载失败的原因可能是此类不存在或其关联引用类不存在 扩展Class#forName(String, boolean, ClassLoader)方法，支持以下几类类名的加载： |
| `cn.hutool.core.util.ClassLoaderUtil` | `Class<?> loadClass(String name,boolean isInitialized)` | 加载类，通过传入类的字符串，返回其对应的类名，使用默认ClassLoader 扩展Class#forName(String, boolean, ClassLoader)方法，支持以下几类类名的加载： |
| `cn.hutool.core.util.ClassLoaderUtil` | `Class<?> loadPrimitiveClass(String name)` | 加载原始类型的类。包括原始类型、原始类型数组和void |
| `cn.hutool.core.util.ClassLoaderUtil` | `ClassLoader getClassLoader()` | 获取ClassLoader 获取顺序如下： |
| `cn.hutool.core.util.ClassLoaderUtil` | `ClassLoader getContextClassLoader()` | 获取当前线程的ClassLoader |
| `cn.hutool.core.util.ClassLoaderUtil` | `ClassLoader getSystemClassLoader()` | 获取系统ClassLoader |
| `cn.hutool.core.util.ClassLoaderUtil` | `JarClassLoader getJarClassLoader(File jarOrDir)` | 创建新的JarClassLoader，并使用此Classloader加载目录下的class文件和jar文件 |
| `cn.hutool.core.util.ClassLoaderUtil` | `boolean isPresent(String className)` | 指定类是否被提供，使用默认ClassLoader 通过调用#loadClass(String, ClassLoader, boolean)方法尝试加载指定类名的类，如果加载失败返回false 加载失败的原因可能是此类不存在或其关联引用类不存在 |
| `cn.hutool.core.util.ClassLoaderUtil` | `boolean isPresent(String className,ClassLoader classLoader)` | 指定类是否被提供 通过调用#loadClass(String, ClassLoader, boolean)方法尝试加载指定类名的类，如果加载失败返回false 加载失败的原因可能是此类不存在或其关联引用类不存在 |
| `cn.hutool.core.util.ClassUtil` | `Class<?> getEnclosingClass(Class<?> clazz)` | 获得外围类 返回定义此类或匿名类所在的类，如果类本身是在包中定义的，返回null |
| `cn.hutool.core.util.ClassUtil` | `Class<?> getTypeArgument(Class<?> clazz)` | 获得给定类的第一个泛型参数 |
| `cn.hutool.core.util.ClassUtil` | `Class<?> getTypeArgument(Class<?> clazz,int index)` | 获得给定类的泛型参数 |
| `cn.hutool.core.util.ClassUtil` | `Class<?>[] getClasses(Object... objects)` | 获得对象数组的类数组 |
| `cn.hutool.core.util.ClassUtil` | `Class<T> getClass(T obj)` | null安全的获取对象类型 |
| `cn.hutool.core.util.ClassUtil` | `Class<T> loadClass(String className)` | 加载类并初始化 |
| `cn.hutool.core.util.ClassUtil` | `Class<T> loadClass(String className,boolean isInitialized)` | 加载类 |
| `cn.hutool.core.util.ClassUtil` | `ClassLoader getClassLoader()` | 获取ClassLoader 获取顺序如下： |
| `cn.hutool.core.util.ClassUtil` | `ClassLoader getContextClassLoader()` | 获取当前线程的ClassLoader |
| `cn.hutool.core.util.ClassUtil` | `Field getDeclaredField(Class<?> clazz,String fieldName)` | 查找指定类中的所有字段（包括非public字段）， 字段不存在则返回null |
| `cn.hutool.core.util.ClassUtil` | `Field[] getDeclaredFields(Class<?> clazz)` | 查找指定类中的所有字段（包括非public字段) |
| `cn.hutool.core.util.ClassUtil` | `List<Method> getPublicMethods(Class<?> clazz,Filter<Method> filter)` | 获得指定类过滤后的Public方法列表 |
| `cn.hutool.core.util.ClassUtil` | `List<Method> getPublicMethods(Class<?> clazz,Method... excludeMethods)` | 获得指定类过滤后的Public方法列表 |
| `cn.hutool.core.util.ClassUtil` | `List<Method> getPublicMethods(Class<?> clazz,String... excludeMethodNames)` | 获得指定类过滤后的Public方法列表 |
| `cn.hutool.core.util.ClassUtil` | `List<URL> getResources(String resource)` | 获取指定路径下的资源列表 路径格式必须为目录格式,用/分隔，例如: |
| `cn.hutool.core.util.ClassUtil` | `Method getDeclaredMethod(Class<?> clazz,String methodName,Class<?>... parameterTypes)` | 查找指定类中的所有方法（包括非public方法），也包括父类和Object类的方法 找不到方法会返回null |
| `cn.hutool.core.util.ClassUtil` | `Method getDeclaredMethodOfObj(Object obj,String methodName,Object... args)` | 查找指定对象中的所有方法（包括非public方法），也包括父对象和Object类的方法 |
| `cn.hutool.core.util.ClassUtil` | `Method getPublicMethod(Class<?> clazz,String methodName,Class<?>... paramTypes)` | 查找指定Public方法 如果找不到对应的方法或方法不为public的则返回null |
| `cn.hutool.core.util.ClassUtil` | `Method setAccessible(Method method)` | 设置方法为可访问 |
| `cn.hutool.core.util.ClassUtil` | `Method[] getDeclaredMethods(Class<?> clazz)` | 获得声明的所有方法，包括本类及其父类和接口的所有方法和Object类的方法 |
| `cn.hutool.core.util.ClassUtil` | `Method[] getPublicMethods(Class<?> clazz)` | 获得本类及其父类所有Public方法 |
| `cn.hutool.core.util.ClassUtil` | `Object getDefaultValue(Class<?> clazz)` | 获取指定类型分的默认值 默认值规则为： |
| `cn.hutool.core.util.ClassUtil` | `Object getPrimitiveDefaultValue(Class<?> clazz)` | 获取指定原始类型分的默认值 默认值规则为： |
| `cn.hutool.core.util.ClassUtil` | `Object[] getDefaultValues(Class<?>... classes)` | 获得默认值列表 |
| `cn.hutool.core.util.ClassUtil` | `Set<Class<?>> scanPackage()` | 扫描该包路径下所有class文件 |
| `cn.hutool.core.util.ClassUtil` | `Set<Class<?>> scanPackage(String packageName)` | 扫描该包路径下所有class文件 |
| `cn.hutool.core.util.ClassUtil` | `Set<Class<?>> scanPackage(String packageName,Filter<Class<?>> classFilter)` | 扫描包路径下满足class过滤器条件的所有class文件， 如果包路径为 com.abs + A.class 但是输入 abs会产生classNotFoundException 因为className 应该为 com.abs.A 现在却成为abs.A,此工具类对该异常进行忽略处理,有可能是一个不完善的地方，以后需要进行修改 |
| `cn.hutool.core.util.ClassUtil` | `Set<Class<?>> scanPackageByAnnotation(String packageName,final Class<? extends Annotation> annotationClass)` | 扫描指定包路径下所有包含指定注解的类 |
| `cn.hutool.core.util.ClassUtil` | `Set<Class<?>> scanPackageBySuper(String packageName,final Class<?> superClass)` | 扫描指定包路径下所有指定类或接口的子类或实现类 |
| `cn.hutool.core.util.ClassUtil` | `Set<String> getClassPathResources()` | 获得ClassPath，不解码路径中的特殊字符（例如空格和中文） |
| `cn.hutool.core.util.ClassUtil` | `Set<String> getClassPathResources(boolean isDecode)` | 获得ClassPath |
| `cn.hutool.core.util.ClassUtil` | `Set<String> getClassPaths(String packageName)` | 获得ClassPath，不解码路径中的特殊字符（例如空格和中文） |
| `cn.hutool.core.util.ClassUtil` | `Set<String> getClassPaths(String packageName,boolean isDecode)` | 获得ClassPath |
| `cn.hutool.core.util.ClassUtil` | `Set<String> getDeclaredMethodNames(Class<?> clazz)` | 获得指定类中的Public方法名 去重重载的方法 |
| `cn.hutool.core.util.ClassUtil` | `Set<String> getPublicMethodNames(Class<?> clazz)` | 获得指定类中的Public方法名 去重重载的方法 |
| `cn.hutool.core.util.ClassUtil` | `String getClassName(Class<?> clazz,boolean isSimple)` | 获取类名 类名并不包含“.class”这个扩展名 例如：ClassUtil这个类 |
| `cn.hutool.core.util.ClassUtil` | `String getClassName(Object obj,boolean isSimple)` | 获取类名 |
| `cn.hutool.core.util.ClassUtil` | `String getClassPath()` | 获得ClassPath，将编码后的中文路径解码为原字符 这个ClassPath路径会文件路径被标准化处理 |
| `cn.hutool.core.util.ClassUtil` | `String getClassPath(boolean isEncoded)` | 获得ClassPath，这个ClassPath路径会文件路径被标准化处理 |
| `cn.hutool.core.util.ClassUtil` | `String getLocationPath(Class<?> clazz)` | 获取class类路径, 不管是否在jar包中都会返回文件夹的路径 class在jar包中返回jar的路径,class不在jar中返回文件夹目录 jdk中的类不能使用此方法 |
| `cn.hutool.core.util.ClassUtil` | `String getPackage(Class<?> clazz)` | 获得给定类所在包的名称 例如： com.xiaoleilu.hutool.util.ClassUtil =》 com.xiaoleilu.hutool.util |
| `cn.hutool.core.util.ClassUtil` | `String getPackagePath(Class<?> clazz)` | 获得给定类所在包的路径 例如： com.xiaoleilu.hutool.util.ClassUtil =》 com/xiaoleilu/hutool/util |
| `cn.hutool.core.util.ClassUtil` | `String getShortClassName(String className)` | 获取完整类名的短格式如： cn.hutool.core.util.StrUtil -》c.h.c.u.StrUtil |
| `cn.hutool.core.util.ClassUtil` | `String[] getJavaClassPaths()` | @return 获得Java ClassPath路径，不包括 jre |
| `cn.hutool.core.util.ClassUtil` | `T invoke(String className,String methodName,Object[] args)` | 执行方法 可执行Private方法，也可执行static方法 执行非static方法时，必须满足对象有默认构造方法 非单例模式，如果是非静态方法，每次创建一个新对象 |
| `cn.hutool.core.util.ClassUtil` | `T invoke(String className,String methodName,boolean isSingleton,Object... args)` | 执行方法 可执行Private方法，也可执行static方法 执行非static方法时，必须满足对象有默认构造方法 |
| `cn.hutool.core.util.ClassUtil` | `T invoke(String classNameWithMethodName,Object[] args)` | 执行方法 可执行Private方法，也可执行static方法 执行非static方法时，必须满足对象有默认构造方法 非单例模式，如果是非静态方法，每次创建一个新对象 |
| `cn.hutool.core.util.ClassUtil` | `T invoke(String classNameWithMethodName,boolean isSingleton,Object... args)` | 执行方法 可执行Private方法，也可执行static方法 执行非static方法时，必须满足对象有默认构造方法 |
| `cn.hutool.core.util.ClassUtil` | `URL getClassPathURL()` | 获得ClassPath URL |
| `cn.hutool.core.util.ClassUtil` | `URL getLocation(Class<?> clazz)` | 获取class类路径URL, 不管是否在jar包中都会返回文件夹的路径 class在jar包中返回jar的路径,class不在jar中返回文件夹目录 jdk中的类不能使用此方法 |
| `cn.hutool.core.util.ClassUtil` | `URL getResourceURL(String resource)` | 获得资源的URL 路径用/分隔，例如: |
| `cn.hutool.core.util.ClassUtil` | `URL getResourceUrl(String resource,Class<?> baseClass)` | 获得资源相对路径对应的URL |
| `cn.hutool.core.util.ClassUtil` | `boolean equals(Class<?> clazz,String className,boolean ignoreCase)` | 指定类是否与给定的类名相同 |
| `cn.hutool.core.util.ClassUtil` | `boolean isAbstract(Class<?> clazz)` | 是否为抽象类 |
| `cn.hutool.core.util.ClassUtil` | `boolean isAbstractOrInterface(Class<?> clazz)` | 是否为抽象类或接口 |
| `cn.hutool.core.util.ClassUtil` | `boolean isAllAssignableFrom(Class<?>[] types1,Class<?>[] types2)` | 比较判断types1和types2两组类，如果types1中所有的类都与types2对应位置的类相同，或者是其父类或接口，则返回true |
| `cn.hutool.core.util.ClassUtil` | `boolean isAssignable(Class<?> targetType,Class<?> sourceType)` | 检查目标类是否可以从原类转化 转化包括： 1、原类是对象，目标类型是原类型实现的接口 2、目标类型是原类型的父类 3、两者是原始类型或者包装类型（相互转换） |
| `cn.hutool.core.util.ClassUtil` | `boolean isBasicType(Class<?> clazz)` | 是否为基本类型（包括包装类和原始类） |
| `cn.hutool.core.util.ClassUtil` | `boolean isEnum(Class<?> clazz)` | 判断类是否为枚举类型 |
| `cn.hutool.core.util.ClassUtil` | `boolean isInterface(Class<?> clazz)` | 是否为接口 |
| `cn.hutool.core.util.ClassUtil` | `boolean isJdkClass(Class<?> clazz)` | 是否为JDK中定义的类或接口，判断依据： |
| `cn.hutool.core.util.ClassUtil` | `boolean isNormalClass(Class<?> clazz)` | 是否为标准的类 这个类必须： |
| `cn.hutool.core.util.ClassUtil` | `boolean isNotPublic(Class<?> clazz)` | 指定类是否为非public |
| `cn.hutool.core.util.ClassUtil` | `boolean isNotPublic(Method method)` | 指定方法是否为非public |
| `cn.hutool.core.util.ClassUtil` | `boolean isPrimitiveWrapper(Class<?> clazz)` | 是否为包装类型 |
| `cn.hutool.core.util.ClassUtil` | `boolean isPublic(Class<?> clazz)` | 指定类是否为Public |
| `cn.hutool.core.util.ClassUtil` | `boolean isPublic(Method method)` | 指定方法是否为Public |
| `cn.hutool.core.util.ClassUtil` | `boolean isSimpleTypeOrArray(Class<?> clazz)` | 是否简单值类型或简单值类型的数组 包括：原始类型,、String、other CharSequence, a Number, a Date, a URI, a URL, a Locale or a Class及其数组 |
| `cn.hutool.core.util.ClassUtil` | `boolean isSimpleValueType(Class<?> clazz)` | 是否为简单值类型 包括： |
| `cn.hutool.core.util.ClassUtil` | `boolean isStatic(Method method)` | 是否为静态方法 |
| `cn.hutool.core.util.ClassUtil` | `boolean isTopLevelClass(Class<?> clazz)` | 是否为顶层类，即定义在包中的类，而非定义在类中的内部类 |
| `cn.hutool.core.util.CoordinateUtil` | `Coordinate bd09ToGcj02(double lng,double lat)` | 百度坐标系 (BD-09) 与 火星坐标系 (GCJ-02)的转换 即 百度 转 谷歌、高德 |
| `cn.hutool.core.util.CoordinateUtil` | `Coordinate bd09toWgs84(double lng,double lat)` | 百度坐标系 (BD-09) 与 WGS84 的转换 |
| `cn.hutool.core.util.CoordinateUtil` | `Coordinate gcj02ToBd09(double lng,double lat)` | 火星坐标系 (GCJ-02) 与百度坐标系 (BD-09) 的转换 |
| `cn.hutool.core.util.CoordinateUtil` | `Coordinate gcj02ToWgs84(double lng,double lat)` | 火星坐标系 (GCJ-02) 转换为 WGS84 |
| `cn.hutool.core.util.CoordinateUtil` | `Coordinate mercatorToWgs84(double mercatorX,double mercatorY)` | 墨卡托投影 转为 WGS84 坐标 |
| `cn.hutool.core.util.CoordinateUtil` | `Coordinate wgs84ToBd09(double lng,double lat)` | WGS84 坐标转为 百度坐标系 (BD-09) 坐标 |
| `cn.hutool.core.util.CoordinateUtil` | `Coordinate wgs84ToGcj02(double lng,double lat)` | WGS84 转换为 火星坐标系 (GCJ-02) |
| `cn.hutool.core.util.CoordinateUtil` | `Coordinate wgs84ToMercator(double lng,double lat)` | WGS84 坐标转为 墨卡托投影 |
| `cn.hutool.core.util.CoordinateUtil` | `boolean outOfChina(double lng,double lat)` | 判断坐标是否在国外 火星坐标系 (GCJ-02)只对国内有效，国外无需转换 |
| `cn.hutool.core.util.CoordinateUtil$Coordinate` | `Coordinate offset(Coordinate offset)` | 当前坐标偏移指定坐标 |
| `cn.hutool.core.util.CoordinateUtil$Coordinate` | `Coordinate setLat(double lat)` | 设置纬度 |
| `cn.hutool.core.util.CoordinateUtil$Coordinate` | `Coordinate setLng(double lng)` | 设置经度 |
| `cn.hutool.core.util.CoordinateUtil$Coordinate` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.util.CoordinateUtil$Coordinate` | `boolean equals(Object o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.util.CoordinateUtil$Coordinate` | `double getLat()` | 获取纬度 |
| `cn.hutool.core.util.CoordinateUtil$Coordinate` | `double getLng()` | 获取经度 |
| `cn.hutool.core.util.CoordinateUtil$Coordinate` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.util.CreditCodeUtil` | `String randomCreditCode()` | 获取一个随机的统一社会信用代码 |
| `cn.hutool.core.util.CreditCodeUtil` | `boolean isCreditCode(CharSequence creditCode)` | 是否是有效的统一社会信用代码 |
| `cn.hutool.core.util.CreditCodeUtil` | `boolean isCreditCodeSimple(CharSequence creditCode)` | 正则校验统一社会信用代码（18位） |
| `cn.hutool.core.util.DesensitizedUtil` | `Long userId()` | 【用户id】不对外提供userId |
| `cn.hutool.core.util.DesensitizedUtil` | `String address(String address,int sensitiveSize)` | 【地址】只显示到地区，不显示详细地址，比如：北京市海淀区**** |
| `cn.hutool.core.util.DesensitizedUtil` | `String bankCard(String bankCardNo)` | 【银行卡号脱敏】由于银行卡号长度不定，所以只展示前4位，后面的位数根据卡号决定展示1-4位 例如： |
| `cn.hutool.core.util.DesensitizedUtil` | `String carLicense(String carLicense)` | 【中国车牌】车牌中间用*代替 eg1：null -》 "" eg1："" -》 "" eg3：苏D40000 -》 苏D4***0 eg4：陕A12345D -》 陕A1****D eg5：京A123 -》 京A123 如果是错误的车牌，不处理 |
| `cn.hutool.core.util.DesensitizedUtil` | `String chineseName(String fullName)` | 【中文姓名】只显示第一个汉字，其他隐藏为2个星号，比如：李** |
| `cn.hutool.core.util.DesensitizedUtil` | `String clear()` | 清空为空字符串 |
| `cn.hutool.core.util.DesensitizedUtil` | `String clearToNull()` | 清空为null |
| `cn.hutool.core.util.DesensitizedUtil` | `String creditCode(String code)` | 统一社会信用代码脱敏 规则：前4后4，长度不足时保留最小有效信息 统一社会信用代码由18位数字或大写英文字母组成 示例：91110108MA01ABCDE7 → 9111**********CDE7 |
| `cn.hutool.core.util.DesensitizedUtil` | `String desensitized(CharSequence str,DesensitizedUtil.DesensitizedType desensitizedType)` | 脱敏，使用默认的脱敏策略 |
| `cn.hutool.core.util.DesensitizedUtil` | `String email(String email)` | 【电子邮箱】邮箱前缀仅显示第一个字母，前缀其他隐藏，用星号代替，@及后面的地址显示，比如：d**@126.com |
| `cn.hutool.core.util.DesensitizedUtil` | `String firstMask(String str)` | 定义了一个first_mask的规则，只显示第一个字符。 脱敏前：123456789；脱敏后：1********。 |
| `cn.hutool.core.util.DesensitizedUtil` | `String fixedPhone(String num)` | 【固定电话 前四位，后两位 |
| `cn.hutool.core.util.DesensitizedUtil` | `String idCardNum(String idCardNum,int front,int end)` | 【身份证号】前1位 和后2位 |
| `cn.hutool.core.util.DesensitizedUtil` | `String ipv4(String ipv4)` | IPv4脱敏，如：脱敏前：192.0.2.1；脱敏后：192.*.*.*。 |
| `cn.hutool.core.util.DesensitizedUtil` | `String ipv6(String ipv6)` | IPv6脱敏，如：脱敏前：2001:0db8:86a3:08d3:1319:8a2e:0370:7344；脱敏后：2001:*:*:*:*:*:*:* |
| `cn.hutool.core.util.DesensitizedUtil` | `String mobilePhone(String num)` | 【手机号码】前三位，后4位，其他隐藏，比如135****2210 |
| `cn.hutool.core.util.DesensitizedUtil` | `String passport(String passport)` | 护照号脱敏 规则：前2后2，长度不足时保留最小有效信息 示例：PJ1234567 → PJ*****67 |
| `cn.hutool.core.util.DesensitizedUtil` | `String password(String password)` | 【密码】密码的全部字符都用*代替，比如：****** |
| `cn.hutool.core.util.EnumUtil` | `E fromString(Class<E> enumClass,String value)` | 字符串转枚举，调用Enum#valueOf(Class, String) |
| `cn.hutool.core.util.EnumUtil` | `E fromString(Class<E> enumClass,String value,E defaultValue)` | 字符串转枚举，调用Enum#valueOf(Class, String) 如果无枚举值，返回默认值 |
| `cn.hutool.core.util.EnumUtil` | `E fromStringQuietly(Class<E> enumClass,String value)` | 字符串转枚举，调用Enum#valueOf(Class, String)，转换失败返回null 而非报错 |
| `cn.hutool.core.util.EnumUtil` | `E getBy(Class<E> enumClass,Func1<E, C> condition,C value)` | 通过 某字段对应值 获取 枚举，获取不到时为 null LambdaUtil#getRealClass(Func1)} 是相对耗时的 如果枚举值比较多,那么EnumUtil#getBy(Func1, Object) 方法 大部分时间都是被LambdaUtil#getRealClass(Func1)}所消耗的 如果可以在编码过程中可以提供对应的枚举类 该方法与枚举的Enum.values()方法是差不多的。 |
| `cn.hutool.core.util.EnumUtil` | `E getBy(Class<E> enumClass,Func1<E, C> condition,C value,E defaultEnum)` | 通过 某字段对应值 获取 枚举，获取不到时为 defaultEnum |
| `cn.hutool.core.util.EnumUtil` | `E getBy(Class<E> enumClass,Predicate<? super E> predicate)` | 通过 某字段对应值 获取 枚举，获取不到时为 null |
| `cn.hutool.core.util.EnumUtil` | `E getBy(Class<E> enumClass,Predicate<? super E> predicate,E defaultEnum)` | 通过 某字段对应值 获取 枚举，获取不到时为 defaultEnum 通过缓存减少反射带来的影响 |
| `cn.hutool.core.util.EnumUtil` | `E getBy(Func1<E, C> condition,C value)` | 通过 某字段对应值 获取 枚举，获取不到时为 null |
| `cn.hutool.core.util.EnumUtil` | `E getBy(Func1<E, C> condition,C value,E defaultEnum)` | 通过 某字段对应值 获取 枚举，获取不到时为 defaultEnum |
| `cn.hutool.core.util.EnumUtil` | `E getEnumAt(Class<E> enumClass,int index)` | 获取给定位置的枚举值 |
| `cn.hutool.core.util.EnumUtil` | `E likeValueOf(Class<E> enumClass,Object value)` | 模糊匹配转换为枚举，给定一个值，匹配枚举中定义的所有字段名（包括name属性），一旦匹配到返回这个枚举对象，否则返回null |
| `cn.hutool.core.util.EnumUtil` | `F getFieldBy(Func1<E, F> field,Function<E, C> condition,C value)` | 通过 某字段对应值 获取 枚举中另一字段值，获取不到时为 null |
| `cn.hutool.core.util.EnumUtil` | `LinkedHashMap<String, E> getEnumMap(final Class<E> enumClass)` | 获取枚举字符串值和枚举对象的Map对应，使用LinkedHashMap保证有序 结果中键为枚举名，值为枚举对象 |
| `cn.hutool.core.util.EnumUtil` | `List<Object> getFieldValues(Class<? extends Enum<?>> clazz,String fieldName)` | 获得枚举类中各枚举对象下指定字段的值 |
| `cn.hutool.core.util.EnumUtil` | `List<String> getFieldNames(Class<? extends Enum<?>> clazz)` | 获得枚举类中所有的字段名 除用户自定义的字段名，也包括“name”字段，例如： |
| `cn.hutool.core.util.EnumUtil` | `List<String> getNames(Class<? extends Enum<?>> clazz)` | 枚举类中所有枚举对象的name列表 |
| `cn.hutool.core.util.EnumUtil` | `Map<String, Object> getNameFieldMap(Class<? extends Enum<?>> clazz,String fieldName)` | 获得枚举名对应指定字段值的Map 键为枚举名，值为字段值 |
| `cn.hutool.core.util.EnumUtil` | `String toString(Enum<?> e)` | Enum对象转String，调用Enum#name() 方法 |
| `cn.hutool.core.util.EnumUtil` | `boolean contains(final Class<E> enumClass,String val)` | 判断某个值是存在枚举中 |
| `cn.hutool.core.util.EnumUtil` | `boolean equals(final Enum<?> e,String val)` | 检查某个枚举值是否匹配指定值 |
| `cn.hutool.core.util.EnumUtil` | `boolean equalsIgnoreCase(final Enum<?> e,String val)` | 忽略大小检查某个枚举值是否匹配指定值 |
| `cn.hutool.core.util.EnumUtil` | `boolean isEnum(Class<?> clazz)` | 指定类是否为Enum类 |
| `cn.hutool.core.util.EnumUtil` | `boolean isEnum(Object obj)` | 指定类是否为Enum类 |
| `cn.hutool.core.util.EnumUtil` | `boolean notContains(final Class<E> enumClass,String val)` | 判断某个值是不存在枚举中 |
| `cn.hutool.core.util.EnumUtil` | `void clearCache()` | 清空缓存，重新加载枚举类 |
| `cn.hutool.core.util.EscapeUtil` | `String escape(CharSequence content)` | Escape编码（Unicode）（等同于JS的escape()方法） 该方法不会对 ASCII 字母和数字进行编码，也不会对下面这些 ASCII 标点符号进行编码： * @ - _ + . / 其他所有的字符都会被转义序列替换。 |
| `cn.hutool.core.util.EscapeUtil` | `String escape(CharSequence content,Filter<Character> filter)` | Escape编码（Unicode） 该方法不会对 ASCII 字母和数字进行编码。其他所有的字符都会被转义序列替换。 |
| `cn.hutool.core.util.EscapeUtil` | `String escapeAll(CharSequence content)` | Escape编码（Unicode） 该方法不会对 ASCII 字母和数字进行编码。其他所有的字符都会被转义序列替换。 |
| `cn.hutool.core.util.EscapeUtil` | `String escapeHtml4(CharSequence html)` | 转义HTML4中的特殊字符 |
| `cn.hutool.core.util.EscapeUtil` | `String escapeXml(CharSequence xml)` | 转义XML中的特殊字符 |
| `cn.hutool.core.util.EscapeUtil` | `String safeUnescape(String content)` | 安全的unescape文本，当文本不是被escape的时候，返回原文。 |
| `cn.hutool.core.util.EscapeUtil` | `String unescape(final String content)` | Escape解码支持两种转义格式的解码： %XX - 两位十六进制数字，用于表示ASCII字符（0-255） %uXXXX - 四位十六进制数字，用于表示Unicode字符 对于不完整的转义序列，本方法会将其原样保留而不抛出异常： 字符串末尾的单独"%"字符会被原样保留 "%u"后面不足4位十六进制数字时，整个不完整序列会被原样保留 "%"后面不足2位十六进制数字时（非%u格式），整个不完整序列会被原样保留 例如： |
| `cn.hutool.core.util.EscapeUtil` | `String unescapeHtml4(CharSequence html)` | 反转义HTML4中的特殊字符 |
| `cn.hutool.core.util.EscapeUtil` | `String unescapeXml(CharSequence xml)` | 反转义XML中的特殊字符 |
| `cn.hutool.core.util.HashUtil` | `int additiveHash(String key,int prime)` | 加法hash |
| `cn.hutool.core.util.HashUtil` | `int apHash(String str)` | AP算法 |
| `cn.hutool.core.util.HashUtil` | `int bernstein(String key)` | 【原文待译】Bernstein's hash |
| `cn.hutool.core.util.HashUtil` | `int bkdrHash(String str)` | BKDR算法 |
| `cn.hutool.core.util.HashUtil` | `int cityHash32(byte[] data)` | CityHash算法32-bit实现 |
| `cn.hutool.core.util.HashUtil` | `int dekHash(String str)` | DEK算法 |
| `cn.hutool.core.util.HashUtil` | `int djbHash(String str)` | DJB算法 |
| `cn.hutool.core.util.HashUtil` | `int elfHash(String str)` | ELF算法 |
| `cn.hutool.core.util.HashUtil` | `int fnvHash(String data)` | 改进的32位FNV算法1 |
| `cn.hutool.core.util.HashUtil` | `int fnvHash(byte[] data)` | 改进的32位FNV算法1 |
| `cn.hutool.core.util.HashUtil` | `int identityHashCode(Object obj)` | 根据对象的内存地址生成相应的Hash值 |
| `cn.hutool.core.util.HashUtil` | `int intHash(int key)` | Thomas Wang的算法，整数hash |
| `cn.hutool.core.util.HashUtil` | `int javaDefaultHash(String str)` | JAVA自己带的算法 |
| `cn.hutool.core.util.HashUtil` | `int jsHash(String str)` | JS算法 |
| `cn.hutool.core.util.HashUtil` | `int murmur32(byte[] data)` | MurmurHash算法32-bit实现 |
| `cn.hutool.core.util.HashUtil` | `int oneByOneHash(String key)` | 一次一个hash |
| `cn.hutool.core.util.HashUtil` | `int pjwHash(String str)` | PJW算法 |
| `cn.hutool.core.util.HashUtil` | `int rotatingHash(String key,int prime)` | 旋转hash |
| `cn.hutool.core.util.HashUtil` | `int rsHash(String str)` | RS算法hash |
| `cn.hutool.core.util.HashUtil` | `int sdbmHash(String str)` | SDBM算法 |
| `cn.hutool.core.util.HashUtil` | `int universal(char[] key,int mask,int[] tab)` | 【原文待译】Universal Hashing |
| `cn.hutool.core.util.HashUtil` | `int zobrist(char[] key,int mask,int[][] tab)` | 【原文待译】Zobrist Hashing |
| `cn.hutool.core.util.HashUtil` | `long cityHash64(byte[] data)` | CityHash算法64-bit实现 |
| `cn.hutool.core.util.HashUtil` | `long cityHash64(byte[] data,long seed)` | CityHash算法64-bit实现，种子1使用默认的CityHash#k2 |
| `cn.hutool.core.util.HashUtil` | `long cityHash64(byte[] data,long seed0,long seed1)` | CityHash算法64-bit实现，种子1使用默认的CityHash#k2 |
| `cn.hutool.core.util.HashUtil` | `long hfHash(String data)` | HF Hash算法 |
| `cn.hutool.core.util.HashUtil` | `long hfIpHash(String data)` | HFIP Hash算法 |
| `cn.hutool.core.util.HashUtil` | `long metroHash64(byte[] data)` | MetroHash 算法64-bit实现 |
| `cn.hutool.core.util.HashUtil` | `long metroHash64(byte[] data,long seed)` | MetroHash 算法64-bit实现 |
| `cn.hutool.core.util.HashUtil` | `long mixHash(String str)` | 混合hash算法，输出64位的值 |
| `cn.hutool.core.util.HashUtil` | `long murmur64(byte[] data)` | MurmurHash算法64-bit实现 |
| `cn.hutool.core.util.HashUtil` | `long tianlHash(String str)` | TianL Hash算法 |
| `cn.hutool.core.util.HashUtil` | `long[] cityHash128(byte[] data)` | CityHash算法128-bit实现 |
| `cn.hutool.core.util.HashUtil` | `long[] cityHash128(byte[] data,Number128 seed)` | CityHash算法128-bit实现 |
| `cn.hutool.core.util.HashUtil` | `long[] metroHash128(byte[] data)` | MetroHash 算法128-bit实现 |
| `cn.hutool.core.util.HashUtil` | `long[] metroHash128(byte[] data,long seed)` | MetroHash 算法128-bit实现 |
| `cn.hutool.core.util.HashUtil` | `long[] murmur128(byte[] data)` | MurmurHash算法128-bit实现 |
| `cn.hutool.core.util.HexUtil` | `BigInteger toBigInteger(String hexStr)` | Hex（16进制）字符串转为BigInteger |
| `cn.hutool.core.util.HexUtil` | `Color decodeColor(String hexColor)` | 将Hex颜色值转为 |
| `cn.hutool.core.util.HexUtil` | `String decodeHexStr(String hexStr)` | 将十六进制字符数组转换为字符串，默认编码UTF-8 |
| `cn.hutool.core.util.HexUtil` | `String decodeHexStr(String hexStr,Charset charset)` | 将十六进制字符数组转换为字符串 |
| `cn.hutool.core.util.HexUtil` | `String decodeHexStr(char[] hexData,Charset charset)` | 将十六进制字符数组转换为字符串 |
| `cn.hutool.core.util.HexUtil` | `String encodeColor(Color color)` | 将Color编码为Hex形式 |
| `cn.hutool.core.util.HexUtil` | `String encodeColor(Color color,String prefix)` | 将Color编码为Hex形式 |
| `cn.hutool.core.util.HexUtil` | `String encodeHexStr(String data)` | 将字符串转换为十六进制字符串，结果为小写，默认编码是UTF-8 |
| `cn.hutool.core.util.HexUtil` | `String encodeHexStr(String data,Charset charset)` | 将字符串转换为十六进制字符串，结果为小写 |
| `cn.hutool.core.util.HexUtil` | `String encodeHexStr(byte[] data)` | 将字节数组转换为十六进制字符串 |
| `cn.hutool.core.util.HexUtil` | `String encodeHexStr(byte[] data,boolean toLowerCase)` | 将字节数组转换为十六进制字符串 |
| `cn.hutool.core.util.HexUtil` | `String format(final String hexStr)` | 格式化Hex字符串，结果为每2位加一个空格，类似于： |
| `cn.hutool.core.util.HexUtil` | `String format(final String hexStr,String prefix)` | 格式化Hex字符串，结果为每2位加一个空格，类似于： |
| `cn.hutool.core.util.HexUtil` | `String toHex(double value)` | 转为16进制字符串 |
| `cn.hutool.core.util.HexUtil` | `String toHex(float value)` | 转为16进制字符串 |
| `cn.hutool.core.util.HexUtil` | `String toHex(int value)` | 转为16进制字符串 |
| `cn.hutool.core.util.HexUtil` | `String toHex(long value)` | 转为16进制字符串 |
| `cn.hutool.core.util.HexUtil` | `String toUnicodeHex(char ch)` | 将指定char值转换为Unicode字符串形式，常用于特殊字符（例如汉字）转Unicode形式 转换的字符串如果u后不足4位，则前面用0填充，例如： |
| `cn.hutool.core.util.HexUtil` | `String toUnicodeHex(int value)` | 将指定int值转换为Unicode字符串形式，常用于特殊字符（例如汉字）转Unicode形式 转换的字符串如果u后不足4位，则前面用0填充，例如： |
| `cn.hutool.core.util.HexUtil` | `boolean isHexNumber(String value)` | 判断给定字符串是否为16进制数 如果是，需要使用对应数字类型对象的decode方法解码 例如：Integer.decode方法解码int类型的16进制数字 |
| `cn.hutool.core.util.HexUtil` | `byte[] decodeHex(CharSequence hexData)` | 将十六进制字符数组转换为字节数组 |
| `cn.hutool.core.util.HexUtil` | `byte[] decodeHex(String hexStr)` | 将十六进制字符串解码为byte[] |
| `cn.hutool.core.util.HexUtil` | `byte[] decodeHex(char[] hexData)` | 将十六进制字符数组转换为字节数组 |
| `cn.hutool.core.util.HexUtil` | `char[] encodeHex(String str,Charset charset)` | 将字节数组转换为十六进制字符数组 |
| `cn.hutool.core.util.HexUtil` | `char[] encodeHex(byte[] data)` | 将字节数组转换为十六进制字符数组 |
| `cn.hutool.core.util.HexUtil` | `char[] encodeHex(byte[] data,boolean toLowerCase)` | 将字节数组转换为十六进制字符数组 |
| `cn.hutool.core.util.HexUtil` | `double hexToDouble(String value)` | 16进制字符串转为double |
| `cn.hutool.core.util.HexUtil` | `float hexToFloat(String value)` | 16进制字符串转为float |
| `cn.hutool.core.util.HexUtil` | `int hexToInt(String value)` | 16进制字符串转为int |
| `cn.hutool.core.util.HexUtil` | `long hexToLong(String value)` | 16进制字符串转为long |
| `cn.hutool.core.util.HexUtil` | `void appendHex(StringBuilder builder,byte b,boolean toLowerCase)` | 将byte值转为16进制并添加到StringBuilder中 |
| `cn.hutool.core.util.IdUtil` | `Snowflake createSnowflake(long workerId,long datacenterId)` | 创建Twitter的Snowflake 算法生成器。 特别注意：此方法调用后会创建独立的Snowflake对象，每个独立的对象ID不互斥，会导致ID重复，请自行保证单例！ 分布式系统中，有一些需要使用全局唯一ID的场景，有些时候我们希望能使用一种简单一些的ID，并且希望ID能够按照时间有序生成。 snowflake的结构如下(每部分用-分开): |
| `cn.hutool.core.util.IdUtil` | `Snowflake getSnowflake()` | 获取单例的Twitter的Snowflake 算法生成器对象 分布式系统中，有一些需要使用全局唯一ID的场景，有些时候我们希望能使用一种简单一些的ID，并且希望ID能够按照时间有序生成。 snowflake的结构如下(每部分用-分开): |
| `cn.hutool.core.util.IdUtil` | `Snowflake getSnowflake(long workerId)` | 获取单例的Twitter的Snowflake 算法生成器对象 分布式系统中，有一些需要使用全局唯一ID的场景，有些时候我们希望能使用一种简单一些的ID，并且希望ID能够按照时间有序生成。 snowflake的结构如下(每部分用-分开): |
| `cn.hutool.core.util.IdUtil` | `Snowflake getSnowflake(long workerId,long datacenterId)` | 获取单例的Twitter的Snowflake 算法生成器对象 分布式系统中，有一些需要使用全局唯一ID的场景，有些时候我们希望能使用一种简单一些的ID，并且希望ID能够按照时间有序生成。 snowflake的结构如下(每部分用-分开): |
| `cn.hutool.core.util.IdUtil` | `String fastSimpleUUID()` | 简化的UUID，去掉了横线，使用性能更好的ThreadLocalRandom生成UUID |
| `cn.hutool.core.util.IdUtil` | `String fastUUID()` | 获取随机UUID，使用性能更好的ThreadLocalRandom生成UUID |
| `cn.hutool.core.util.IdUtil` | `String getSnowflakeNextIdStr()` | 简单获取Snowflake 的 nextId 终端ID 数据中心ID 默认为PID和MAC地址生成 |
| `cn.hutool.core.util.IdUtil` | `String nanoId()` | 获取随机NanoId |
| `cn.hutool.core.util.IdUtil` | `String nanoId(int size)` | 获取随机NanoId |
| `cn.hutool.core.util.IdUtil` | `String objectId()` | 创建MongoDB ID生成策略实现 ObjectId由以下几部分组成： |
| `cn.hutool.core.util.IdUtil` | `String randomUUID()` | 获取随机UUID |
| `cn.hutool.core.util.IdUtil` | `String simpleUUID()` | 简化的UUID，去掉了横线 |
| `cn.hutool.core.util.IdUtil` | `long getDataCenterId(long maxDatacenterId)` | 获取数据中心ID 数据中心ID依赖于本地网卡MAC地址。 此算法来自于mybatis-plus#Sequence |
| `cn.hutool.core.util.IdUtil` | `long getSnowflakeNextId()` | 简单获取Snowflake 的 nextId 终端ID 数据中心ID 默认为PID和MAC地址生成 |
| `cn.hutool.core.util.IdUtil` | `long getWorkerId(long datacenterId,long maxWorkerId)` | 获取机器ID，使用进程ID配合数据中心ID生成 机器依赖于本进程ID或进程名的Hash值。 此算法来自于mybatis-plus#Sequence |
| `cn.hutool.core.util.IdcardUtil` | `DateTime getBirthDate(String idCard)` | 从身份证号码中获取生日日期，只支持15或18位身份证号码 |
| `cn.hutool.core.util.IdcardUtil` | `Idcard getIdcardInfo(String idcard)` | 获取身份证信息，包括身份、城市代码、生日、性别等 |
| `cn.hutool.core.util.IdcardUtil` | `Short getDayByIdCard(String idcard)` | 根据身份编号获取生日天，只支持15或18位身份证号码 |
| `cn.hutool.core.util.IdcardUtil` | `Short getMonthByIdCard(String idcard)` | 根据身份编号获取生日月，只支持15或18位身份证号码 |
| `cn.hutool.core.util.IdcardUtil` | `Short getYearByIdCard(String idcard)` | 根据身份编号获取生日年，只支持15或18位身份证号码 |
| `cn.hutool.core.util.IdcardUtil` | `String convert15To18(String idCard)` | 将15位身份证号码转换为18位 |
| `cn.hutool.core.util.IdcardUtil` | `String convert18To15(String idCard)` | 将18位身份证号码转换为15位 |
| `cn.hutool.core.util.IdcardUtil` | `String getBirth(String idCard)` | 根据身份编号获取生日，只支持15或18位身份证号码 |
| `cn.hutool.core.util.IdcardUtil` | `String getBirthByIdCard(String idcard)` | 根据身份编号获取生日，只支持15或18位身份证号码 |
| `cn.hutool.core.util.IdcardUtil` | `String getCityCodeByIdCard(String idcard)` | 根据身份编号获取地市级编码，只支持15或18位身份证号码 获取编码为4位 |
| `cn.hutool.core.util.IdcardUtil` | `String getDistrictCodeByIdCard(String idcard)` | 根据身份编号获取区县级编码，只支持15或18位身份证号码 获取编码为6位 |
| `cn.hutool.core.util.IdcardUtil` | `String getProvinceByIdCard(String idcard)` | 根据身份编号获取户籍省份，只支持15或18位身份证号码 |
| `cn.hutool.core.util.IdcardUtil` | `String getProvinceCodeByIdCard(String idcard)` | 根据身份编号获取户籍省份编码，只支持15或18位身份证号码 |
| `cn.hutool.core.util.IdcardUtil` | `String hide(String idcard,int startInclude,int endExclude)` | 隐藏指定位置的几个身份证号数字为“*” |
| `cn.hutool.core.util.IdcardUtil` | `String[] isValidCard10(String idcard)` | 验证10位身份编码是否合法 |
| `cn.hutool.core.util.IdcardUtil` | `boolean isValidCard(String idCard)` | 是否有效身份证号，忽略X的大小写 如果身份证号码中含有空格始终返回false |
| `cn.hutool.core.util.IdcardUtil` | `boolean isValidCard15(String idcard)` | 验证15位身份编码是否合法 |
| `cn.hutool.core.util.IdcardUtil` | `boolean isValidCard18(String idcard)` | 判断18位身份证的合法性 根据〖中华人民共和国国家标准GB11643-1999〗中有关公民身份号码的规定，公民身份号码是特征组合码，由十七位数字本体码和一位数字校验码组成。 排列顺序从左至右依次为：六位数字地址码，八位数字出生日期码，三位数字顺序码和一位数字校验码。 顺序码: 表示在同一地址码所标识的区域范围内，对同年、同月、同 日出生的人编定的顺序号，顺序码的奇数分配给男性，偶数分配 给女性。 第1、2位数字表示：所在省份的代码 第3、4位数字表示：所在城市的代码 第5、6位数字表示：所在区县的代码 第7~14位数字表示：出生年、月、日 第15、16位数字表示：所在地的派出所的代码 第17位… |
| `cn.hutool.core.util.IdcardUtil` | `boolean isValidCard18(String idcard,boolean ignoreCase)` | 判断18位身份证的合法性 根据〖中华人民共和国国家标准GB11643-1999〗中有关公民身份号码的规定，公民身份号码是特征组合码，由十七位数字本体码和一位数字校验码组成。 排列顺序从左至右依次为：六位数字地址码，八位数字出生日期码，三位数字顺序码和一位数字校验码。 顺序码: 表示在同一地址码所标识的区域范围内，对同年、同月、同 日出生的人编定的顺序号，顺序码的奇数分配给男性，偶数分配 给女性。 第1、2位数字表示：所在省份的代码 第3、4位数字表示：所在城市的代码 第5、6位数字表示：所在区县的代码 第7~14位数字表示：出生年、月、日 第15、16位数字表示：所在地的派出所的代码 第17位… |
| `cn.hutool.core.util.IdcardUtil` | `boolean isValidHKCard(String idcard)` | 验证香港身份证号码(存在Bug，部份特殊身份证无法检查) 身份证前2位为英文字符，如果只出现一个英文字符则表示第一位是空格，对应数字58 前2位英文字符A-Z分别对应数字10-35 最后一位校验码为0-9的数字加上字符"A"，"A"代表10 将身份证号码全部转换为数字，分别对应乘9-1相加的总和，整除11则证件号码有效 |
| `cn.hutool.core.util.IdcardUtil` | `boolean isValidTWCard(String idcard)` | 验证台湾身份证号码 |
| `cn.hutool.core.util.IdcardUtil` | `int getAgeByIdCard(String idcard)` | 根据身份编号获取年龄，只支持15或18位身份证号码 |
| `cn.hutool.core.util.IdcardUtil` | `int getAgeByIdCard(String idcard,Date dateToCompare)` | 根据身份编号获取指定日期当时的年龄年龄，只支持15或18位身份证号码 |
| `cn.hutool.core.util.IdcardUtil` | `int getGenderByIdCard(String idcard)` | 根据身份编号获取性别，只支持15或18位身份证号码 |
| `cn.hutool.core.util.IdcardUtil$Idcard` | `DateTime getBirthDate()` | 获得生日日期 |
| `cn.hutool.core.util.IdcardUtil$Idcard` | `Integer getGender()` | 获取性别代号，性别(1 : 男 ， 0 : 女) |
| `cn.hutool.core.util.IdcardUtil$Idcard` | `String getCityCode()` | 获取市级编码 |
| `cn.hutool.core.util.IdcardUtil$Idcard` | `String getProvince()` | 获取省份名称 |
| `cn.hutool.core.util.IdcardUtil$Idcard` | `String getProvinceCode()` | 获取省份代码 |
| `cn.hutool.core.util.IdcardUtil$Idcard` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.util.IdcardUtil$Idcard` | `int getAge()` | 获取年龄 |
| `cn.hutool.core.util.JAXBUtil` | `String beanToXml(Object bean)` | JavaBean转换成xml bean上面用的常用注解 |
| `cn.hutool.core.util.JAXBUtil` | `String beanToXml(Object bean,Charset charset,boolean format)` | JavaBean转换成xml |
| `cn.hutool.core.util.JAXBUtil` | `T xmlToBean(File file,Charset charset,Class<T> c)` | XML文件转Bean |
| `cn.hutool.core.util.JAXBUtil` | `T xmlToBean(Reader reader,Class<T> c)` | 从Reader中读取XML字符串，并转换为Bean |
| `cn.hutool.core.util.JAXBUtil` | `T xmlToBean(String xml,Class<T> c)` | xml转换成JavaBean |
| `cn.hutool.core.util.JNDIUtil` | `Attributes getAttributes(String uri,String... attrIds)` | 获取指定容器环境的对象的属性 如获取DNS属性，则URI为类似：dns:hutool.cn |
| `cn.hutool.core.util.JNDIUtil` | `InitialContext createInitialContext(Map<String, String> environment)` | 创建InitialContext 建议在应用启动时设置系统属性（禁用远程 codebase 加载） |
| `cn.hutool.core.util.JNDIUtil` | `InitialDirContext createInitialDirContext(Map<String, String> environment)` | 创建InitialDirContext 建议在应用启动时设置系统属性（禁用远程 codebase 加载） |
| `cn.hutool.core.util.ModifierUtil` | `boolean hasAllModifiers(final Class<?> clazz,final ModifierType... modifierTypes)` | 类中是否同时存在 所有 给定修饰符 如定义修饰符为：public static final，那么如果传入的modifierTypes为： public、static 返回true public、abstract返回false private、abstract返回false |
| `cn.hutool.core.util.ModifierUtil` | `boolean hasAllModifiers(final Member member,final ModifierType... modifierTypes)` | 成员中是否同时存在 所有 给定修饰符 如定义修饰符为：public static final，那么如果传入的modifierTypes为： public、static 返回true public、abstract返回false private、abstract返回false |
| `cn.hutool.core.util.ModifierUtil` | `boolean hasModifier(Class<?> clazz,ModifierType... modifierTypes)` | 类是否存在给定修饰符中的 任意一个 如定义修饰符为：public static final，那么如果传入的modifierTypes为： public、static 返回true public、abstract返回true private、abstract返回false |
| `cn.hutool.core.util.ModifierUtil` | `boolean hasModifier(Constructor<?> constructor,ModifierType... modifierTypes)` | 构造是否存在给定修饰符中的 任意一个 如定义修饰符为：public static final，那么如果传入的modifierTypes为： public、static 返回true public、abstract返回true private、abstract返回false |
| `cn.hutool.core.util.ModifierUtil` | `boolean hasModifier(Field field,ModifierType... modifierTypes)` | 字段是否存在给定修饰符中的 任意一个 如定义修饰符为：public static final，那么如果传入的modifierTypes为： public、static 返回true public、abstract返回true private、abstract返回false |
| `cn.hutool.core.util.ModifierUtil` | `boolean hasModifier(Method method,ModifierType... modifierTypes)` | 方法是否存在给定修饰符中的 任意一个 如定义修饰符为：public static final，那么如果传入的modifierTypes为： public、static 返回true public、abstract返回true private、abstract返回false |
| `cn.hutool.core.util.ModifierUtil` | `boolean isAbstract(Method method)` | 是否抽象方法 |
| `cn.hutool.core.util.ModifierUtil` | `boolean isPublic(Class<?> clazz)` | 是否是Public类 |
| `cn.hutool.core.util.ModifierUtil` | `boolean isPublic(Constructor<?> constructor)` | 是否是Public构造 |
| `cn.hutool.core.util.ModifierUtil` | `boolean isPublic(Field field)` | 是否是Public字段 |
| `cn.hutool.core.util.ModifierUtil` | `boolean isPublic(Method method)` | 是否是Public方法 |
| `cn.hutool.core.util.ModifierUtil` | `boolean isStatic(Class<?> clazz)` | 是否是static类 |
| `cn.hutool.core.util.ModifierUtil` | `boolean isStatic(Field field)` | 是否是static字段 |
| `cn.hutool.core.util.ModifierUtil` | `boolean isStatic(Method method)` | 是否是static方法 |
| `cn.hutool.core.util.ModifierUtil` | `boolean isSynthetic(Class<?> clazz)` | 是否是合成类（由java编译器生成的） |
| `cn.hutool.core.util.ModifierUtil` | `boolean isSynthetic(Field field)` | 是否是合成字段（由java编译器生成的） |
| `cn.hutool.core.util.ModifierUtil` | `boolean isSynthetic(Method method)` | 是否是合成方法（由java编译器生成的） |
| `cn.hutool.core.util.ModifierUtil` | `void removeFinalModify(Field field)` | 设置final的field字段可以被修改 只要不会被编译器内联优化的 final 属性就可以通过反射有效的进行修改 -- 修改后代码中可使用到新的值; 以下属性，编译器会内联优化，无法通过反射修改： 基本类型 byte, char, short, int, long, float, double, boolean Literal String 类型(直接双引号字符串) 以下属性，可以通过反射修改： 基本类型的包装类 Byte、Character、Short、Long、Float、Double、Boolean 字符串，通过 new String("")实例化 自定义java类 |
| `cn.hutool.core.util.ModifierUtil$ModifierType` | `int getValue()` | 获取修饰符枚举对应的int修饰符值，值见Modifier |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal add(BigDecimal... values)` | 提供精确的加法运算 如果传入多个值为null或者空，则返回0 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal add(Number v1,Number v2)` | 提供精确的加法运算 如果传入多个值为null或者空，则返回0 需要注意的是，在不同Locale下，数字的表示形式也是不同的，例如： 德国、荷兰、比利时、丹麦、意大利、罗马尼亚和欧洲大多地区使用','区分小数 也就是说，在这些国家地区，1.20表示120，而非1.2。 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal add(Number... values)` | 提供精确的加法运算 如果传入多个值为null或者空，则返回0 需要注意的是，在不同Locale下，数字的表示形式也是不同的，例如： 德国、荷兰、比利时、丹麦、意大利、罗马尼亚和欧洲大多地区使用','区分小数 也就是说，在这些国家地区，1.20表示120，而非1.2。 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal add(String... values)` | 提供精确的加法运算 如果传入多个值为null或者空，则返回0 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal div(BigDecimal v1,BigDecimal v2,int scale,RoundingMode roundingMode)` | 提供(相对)精确的除法运算,当发生除不尽的情况时,由scale指定精确度 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal div(Number v1,Number v2)` | 提供(相对)精确的除法运算,当发生除不尽的情况的时候,精确到小数点后10位,后面的四舍五入 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal div(Number v1,Number v2,int scale)` | 提供(相对)精确的除法运算,当发生除不尽的情况时,由scale指定精确度,后面的四舍五入 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal div(Number v1,Number v2,int scale,RoundingMode roundingMode)` | 提供(相对)精确的除法运算,当发生除不尽的情况时,由scale指定精确度 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal div(String v1,String v2)` | 提供(相对)精确的除法运算,当发生除不尽的情况的时候,精确到小数点后10位,后面的四舍五入 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal div(String v1,String v2,int scale)` | 提供(相对)精确的除法运算,当发生除不尽的情况时,由scale指定精确度,后面的四舍五入 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal div(String v1,String v2,int scale,RoundingMode roundingMode)` | 提供(相对)精确的除法运算,当发生除不尽的情况时,由scale指定精确度 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal max(BigDecimal... numberArray)` | 取最大值 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal min(BigDecimal... numberArray)` | 取最小值 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal mul(BigDecimal... values)` | 提供精确的乘法运算 如果传入多个值为null或者空，则返回0 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal mul(Number v1,Number v2)` | 提供精确的乘法运算 如果传入多个值为null或者空，则返回0 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal mul(Number... values)` | 提供精确的乘法运算 如果传入多个值为null或者空，则返回0 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal mul(String v1,String v2)` | 提供精确的乘法运算 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal mul(String... values)` | 提供精确的乘法运算 如果传入多个值为null或者空，则返回0 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal null2Zero(BigDecimal decimal)` | 空转0 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal nullToZero(BigDecimal number)` | 如果给定值为null，返回0，否则返回原值 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal pow(BigDecimal number,int n)` | 提供精确的幂运算 如果n为负数，则返回1/a的-n次方，默认四舍五入，保留两位小数 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal pow(BigDecimal number,int n,int scale,RoundingMode roundingMode)` | 提供精确的幂运算 如果n为负数，则返回1/a的-n次方，默认四舍五入 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal pow(Number number,int n)` | 提供精确的幂运算 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal round(BigDecimal number,int scale)` | 保留固定位数小数 采用四舍五入策略 RoundingMode#HALF_UP 例如保留2位小数：123.456789 =》 123.46 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal round(BigDecimal number,int scale,RoundingMode roundingMode)` | 保留固定位数小数 例如保留四位小数：123.456789 =》 123.4567 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal round(String numberStr,int scale)` | 保留固定位数小数 采用四舍五入策略 RoundingMode#HALF_UP 例如保留2位小数：123.456789 =》 123.46 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal round(String numberStr,int scale,RoundingMode roundingMode)` | 保留固定位数小数 例如保留四位小数：123.456789 =》 123.4567 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal round(double v,int scale)` | 保留固定位数小数 采用四舍五入策略 RoundingMode#HALF_UP 例如保留2位小数：123.456789 =》 123.46 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal round(double v,int scale,RoundingMode roundingMode)` | 保留固定位数小数 例如保留四位小数：123.456789 =》 123.4567 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal roundDown(BigDecimal value,int scale)` | 保留固定小数位数，舍去多余位数 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal roundDown(Number number,int scale)` | 保留固定小数位数，舍去多余位数 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal roundHalfEven(BigDecimal value,int scale)` | 四舍六入五成双计算法 四舍六入五成双是一种比较精确比较科学的计数保留法，是一种数字修约规则。 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal roundHalfEven(Number number,int scale)` | 四舍六入五成双计算法 四舍六入五成双是一种比较精确比较科学的计数保留法，是一种数字修约规则。 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal sub(BigDecimal... values)` | 提供精确的减法运算 如果传入多个值为null或者空，则返回0 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal sub(Number v1,Number v2)` | 提供精确的减法运算 如果传入多个值为null或者空，则返回0 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal sub(Number... values)` | 提供精确的减法运算 如果传入多个值为null或者空，则返回0 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal sub(String... values)` | 提供精确的减法运算 如果传入多个值为null或者空，则返回0 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal toBigDecimal(Number number)` | 数字转BigDecimal Float、Double等有精度问题，转换为字符串后再转换 null转换为0 |
| `cn.hutool.core.util.NumberUtil` | `BigDecimal toBigDecimal(String numberStr)` | 数字转BigDecimal null或""或空白符转换为0 |
| `cn.hutool.core.util.NumberUtil` | `BigInteger factorial(BigInteger n)` | 计算阶乘 n! = n * (n-1) * ... * 2 * 1 |
| `cn.hutool.core.util.NumberUtil` | `BigInteger factorial(BigInteger start,BigInteger end)` | 计算范围阶乘 factorial(start, end) = start * (start - 1) * ... * (end + 1) |
| `cn.hutool.core.util.NumberUtil` | `BigInteger fromUnsignedByteArray(byte[] buf)` | 无符号bytes转BigInteger |
| `cn.hutool.core.util.NumberUtil` | `BigInteger fromUnsignedByteArray(byte[] buf,int off,int length)` | 无符号bytes转BigInteger |
| `cn.hutool.core.util.NumberUtil` | `BigInteger newBigInteger(String str)` | 创建BigInteger，支持16进制、10进制和8进制，如果传入空白串返回null from Apache Common Lang |
| `cn.hutool.core.util.NumberUtil` | `BigInteger nullToZero(BigInteger number)` | 如果给定值为null，返回0，否则返回原值 |
| `cn.hutool.core.util.NumberUtil` | `BigInteger toBigInteger(Number number)` | 数字转BigInteger null转换为0 |
| `cn.hutool.core.util.NumberUtil` | `BigInteger toBigInteger(String number)` | 数字转BigInteger null或""或空白符转换为0 |
| `cn.hutool.core.util.NumberUtil` | `Collection<Integer> appendRange(int start,int stop,Collection<Integer> values)` | 将给定范围内的整数添加到已有集合中，步进为1 |
| `cn.hutool.core.util.NumberUtil` | `Collection<Integer> appendRange(int start,int stop,int step,Collection<Integer> values)` | 将给定范围内的整数添加到已有集合中 |
| `cn.hutool.core.util.NumberUtil` | `Double parseDouble(String numberStr,Double defaultValue)` | 解析转换数字字符串为 java.lang.Double 规则如下： |
| `cn.hutool.core.util.NumberUtil` | `Float parseFloat(String numberStr,Float defaultValue)` | 解析转换数字字符串为 java.lang.Float 规则如下： |
| `cn.hutool.core.util.NumberUtil` | `Integer parseInt(String numberStr,Integer defaultValue)` | 解析转换数字字符串为 java.lang.Integer 规则如下： |
| `cn.hutool.core.util.NumberUtil` | `Integer[] generateBySet(int begin,int end,int size)` | 生成不重复随机数 根据给定的最小数字和最大数字，以及随机数的个数，产生指定的不重复的数组 |
| `cn.hutool.core.util.NumberUtil` | `Long parseLong(String numberStr,Long defaultValue)` | 解析转换数字字符串为 java.lang.Long 规则如下： |
| `cn.hutool.core.util.NumberUtil` | `Number parseNumber(String numberStr)` | 将指定字符串转换为Number 对象 此方法不支持科学计数法 需要注意的是，在不同Locale下，数字的表示形式也是不同的，例如： 德国、荷兰、比利时、丹麦、意大利、罗马尼亚和欧洲大多地区使用','区分小数 也就是说，在这些国家地区，1.20表示120，而非1.2。 |
| `cn.hutool.core.util.NumberUtil` | `Number parseNumber(String numberStr,Number defaultValue)` | 将指定字符串转换为Number 此方法不支持科学计数法 |
| `cn.hutool.core.util.NumberUtil` | `String decimalFormat(String pattern,Object value)` | 格式化double 对 DecimalFormat 做封装 |
| `cn.hutool.core.util.NumberUtil` | `String decimalFormat(String pattern,Object value,RoundingMode roundingMode)` | 格式化double 对 DecimalFormat 做封装 |
| `cn.hutool.core.util.NumberUtil` | `String decimalFormat(String pattern,double value)` | 格式化double 对 DecimalFormat 做封装 |
| `cn.hutool.core.util.NumberUtil` | `String decimalFormat(String pattern,long value)` | 格式化double 对 DecimalFormat 做封装 |
| `cn.hutool.core.util.NumberUtil` | `String decimalFormatMoney(double value)` | 格式化金额输出，每三位用逗号分隔 |
| `cn.hutool.core.util.NumberUtil` | `String formatPercent(double number,int scale)` | 格式化百分比，小数采用四舍五入方式 |
| `cn.hutool.core.util.NumberUtil` | `String getBinaryStr(Number number)` | 获得数字对应的二进制字符串 Integer/Long：直接使用 JDK 内置方法转换 Byte/Short：转换为无符号整数后补充前导零至对应位数（Byte=8位，Short=16位） Float/Double：使用 IEEE 754 标准格式转换，Float=32位，Double=64位 |
| `cn.hutool.core.util.NumberUtil` | `String roundStr(String numberStr,int scale)` | 保留固定位数小数 采用四舍五入策略 RoundingMode#HALF_UP 例如保留2位小数：123.456789 =》 123.46 |
| `cn.hutool.core.util.NumberUtil` | `String roundStr(String numberStr,int scale,RoundingMode roundingMode)` | 保留固定位数小数 例如保留四位小数：123.456789 =》 123.4567 |
| `cn.hutool.core.util.NumberUtil` | `String roundStr(double v,int scale)` | 保留固定位数小数 采用四舍五入策略 RoundingMode#HALF_UP 例如保留2位小数：123.456789 =》 123.46 |
| `cn.hutool.core.util.NumberUtil` | `String roundStr(double v,int scale,RoundingMode roundingMode)` | 保留固定位数小数 例如保留四位小数：123.456789 =》 123.4567 |
| `cn.hutool.core.util.NumberUtil` | `String toStr(BigDecimal bigDecimal)` | BigDecimal数字转字符串 调用BigDecimal#toPlainString()，并去除尾小数点儿后多余的0 |
| `cn.hutool.core.util.NumberUtil` | `String toStr(BigDecimal bigDecimal,boolean isStripTrailingZeros)` | BigDecimal数字转字符串 调用BigDecimal#toPlainString()，可选去除尾小数点儿后多余的0 |
| `cn.hutool.core.util.NumberUtil` | `String toStr(Number number)` | 数字转字符串 调用Number#toString()或 BigDecimal#toPlainString()，并去除尾小数点儿后多余的0 |
| `cn.hutool.core.util.NumberUtil` | `String toStr(Number number,String defaultValue)` | 数字转字符串 调用Number#toString()，并去除尾小数点儿后多余的0 |
| `cn.hutool.core.util.NumberUtil` | `String toStr(Number number,boolean isStripTrailingZeros)` | 数字转字符串 调用Number#toString()或 BigDecimal#toPlainString()，并去除尾小数点儿后多余的0 |
| `cn.hutool.core.util.NumberUtil` | `T max(T[] numberArray)` | 取最大值 |
| `cn.hutool.core.util.NumberUtil` | `T min(T[] numberArray)` | 取最小值 |
| `cn.hutool.core.util.NumberUtil` | `boolean equals(BigDecimal bigNum1,BigDecimal bigNum2)` | 比较大小，值相等 返回true 此方法通过调用BigDecimal#compareTo(BigDecimal)方法来判断是否相等 此方法判断值相等时忽略精度的，即0.00 == 0 |
| `cn.hutool.core.util.NumberUtil` | `boolean equals(char c1,char c2,boolean ignoreCase)` | 比较两个字符是否相同 |
| `cn.hutool.core.util.NumberUtil` | `boolean equals(double num1,double num2)` | 比较大小，值相等 返回true 此方法通过调用Double#doubleToLongBits(double)方法来判断是否相等 此方法判断值相等时忽略精度的，即0.00 == 0 |
| `cn.hutool.core.util.NumberUtil` | `boolean equals(final Number number1,final Number number2)` | 比较数字值是否相等，相等返回true 需要注意的是BigDecimal需要特殊处理 BigDecimal使用compareTo方式判断，因为使用equals方法也判断小数位数，如2.0和2.00就不相等， 此方法判断值相等时忽略精度的，即0.00 == 0 如果用户提供两个Number都是BigDecimal，则通过调用BigDecimal#compareTo(BigDecimal)方法来判断是否相等 其他情况调用Number#equals(Object)比较 |
| `cn.hutool.core.util.NumberUtil` | `boolean equals(float num1,float num2)` | 比较大小，值相等 返回true 此方法通过调用Float#floatToIntBits(float)方法来判断是否相等 此方法判断值相等时忽略精度的，即0.00 == 0 |
| `cn.hutool.core.util.NumberUtil` | `boolean equals(long num1,long num2)` | 比较大小，值相等 返回true 此方法修复传入long型数据由于没有本类型重载方法,导致数据精度丢失 |
| `cn.hutool.core.util.NumberUtil` | `boolean isBeside(int number1,int number2)` | 判断两个数字是否相邻，例如1和2相邻，1和3不相邻 判断方法为做差取绝对值判断是否为1 |
| `cn.hutool.core.util.NumberUtil` | `boolean isBeside(long number1,long number2)` | 判断两个数字是否相邻，例如1和2相邻，1和3不相邻 判断方法为做差取绝对值判断是否为1 |
| `cn.hutool.core.util.NumberUtil` | `boolean isDouble(String s)` | 判断字符串是否是浮点数 |
| `cn.hutool.core.util.NumberUtil` | `boolean isEven(int num)` | 检查是否为偶数 |
| `cn.hutool.core.util.NumberUtil` | `boolean isGreater(BigDecimal bigNum1,BigDecimal bigNum2)` | 比较大小，参数1 > 参数2 返回true |
| `cn.hutool.core.util.NumberUtil` | `boolean isGreaterOrEqual(BigDecimal bigNum1,BigDecimal bigNum2)` | 比较大小，参数1 >= 参数2 返回true |
| `cn.hutool.core.util.NumberUtil` | `boolean isIn(final BigDecimal value,final BigDecimal minInclude,final BigDecimal maxInclude)` | 检查值是否在指定范围内 |
| `cn.hutool.core.util.NumberUtil` | `boolean isInteger(String s)` | 判断String是否是整数 支持10进制 |
| `cn.hutool.core.util.NumberUtil` | `boolean isLess(BigDecimal bigNum1,BigDecimal bigNum2)` | 比较大小，参数1 < 参数2 返回true |
| `cn.hutool.core.util.NumberUtil` | `boolean isLessOrEqual(BigDecimal bigNum1,BigDecimal bigNum2)` | 比较大小，参数1<=参数2 返回true |
| `cn.hutool.core.util.NumberUtil` | `boolean isLong(String s)` | 判断字符串是否是Long类型 支持10进制 |
| `cn.hutool.core.util.NumberUtil` | `boolean isNumber(CharSequence str)` | 是否为数字，支持包括： |
| `cn.hutool.core.util.NumberUtil` | `boolean isOdd(int num)` | 检查是否为奇数 |
| `cn.hutool.core.util.NumberUtil` | `boolean isPowerOfTwo(long n)` | 判断一个整数是否是2的幂 |
| `cn.hutool.core.util.NumberUtil` | `boolean isPrimes(int n)` | 是否是质数（素数） 质数表的质数又称素数。指整数在一个大于1的自然数中,除了1和此整数自身外,没法被其他自然数整除的数。 |
| `cn.hutool.core.util.NumberUtil` | `boolean isValid(double number)` | 检查是否为有效的数字 检查double否为无限大，或者Not a Number（NaN） |
| `cn.hutool.core.util.NumberUtil` | `boolean isValid(float number)` | 检查是否为有效的数字 检查double否为无限大，或者Not a Number（NaN） |
| `cn.hutool.core.util.NumberUtil` | `boolean isValidNumber(Number number)` | 检查是否为有效的数字 检查Double和Float是否为无限大，或者Not a Number 非数字类型和Null将返回false |
| `cn.hutool.core.util.NumberUtil` | `byte nullToZero(Byte number)` | 如果给定值为null，返回0，否则返回原值 |
| `cn.hutool.core.util.NumberUtil` | `byte[] toBytes(int value)` | int值转byte数组，使用大端字节序（高位字节在前，低位字节在后） 见： http://www.ruanyifeng.com/blog/2016/11/byte-order.html |
| `cn.hutool.core.util.NumberUtil` | `byte[] toUnsignedByteArray(BigInteger value)` | 以无符号字节数组的形式返回传入值。 |
| `cn.hutool.core.util.NumberUtil` | `byte[] toUnsignedByteArray(int length,BigInteger value)` | 以无符号字节数组的形式返回传入值。 |
| `cn.hutool.core.util.NumberUtil` | `double add(Double v1,Double v2)` | 提供精确的加法运算 |
| `cn.hutool.core.util.NumberUtil` | `double add(double v1,double v2)` | 提供精确的加法运算 |
| `cn.hutool.core.util.NumberUtil` | `double add(double v1,float v2)` | 提供精确的加法运算 |
| `cn.hutool.core.util.NumberUtil` | `double add(double v1,long v2)` | 提供精确的加法运算 |
| `cn.hutool.core.util.NumberUtil` | `double add(float v1,double v2)` | 提供精确的加法运算 |
| `cn.hutool.core.util.NumberUtil` | `double add(float v1,float v2)` | 提供精确的加法运算 |
| `cn.hutool.core.util.NumberUtil` | `double add(long v1,double v2)` | 提供精确的加法运算 |
| `cn.hutool.core.util.NumberUtil` | `double add(long v1,long v2)` | 提供精确的加法运算 |
| `cn.hutool.core.util.NumberUtil` | `double calculate(String expression)` | 计算数学表达式的值，只支持加减乘除和取余 如： |
| `cn.hutool.core.util.NumberUtil` | `double div(Double v1,Double v2)` | 提供(相对)精确的除法运算,当发生除不尽的情况的时候,精确到小数点后10位,后面的四舍五入 |
| `cn.hutool.core.util.NumberUtil` | `double div(Double v1,Double v2,int scale)` | 提供(相对)精确的除法运算,当发生除不尽的情况时,由scale指定精确度,后面的四舍五入 |
| `cn.hutool.core.util.NumberUtil` | `double div(Double v1,Double v2,int scale,RoundingMode roundingMode)` | 提供(相对)精确的除法运算,当发生除不尽的情况时,由scale指定精确度 |
| `cn.hutool.core.util.NumberUtil` | `double div(double v1,double v2)` | 提供(相对)精确的除法运算,当发生除不尽的情况的时候,精确到小数点后10位,后面的四舍五入 |
| `cn.hutool.core.util.NumberUtil` | `double div(double v1,double v2,int scale)` | 提供(相对)精确的除法运算,当发生除不尽的情况时,由scale指定精确度,后面的四舍五入 |
| `cn.hutool.core.util.NumberUtil` | `double div(double v1,double v2,int scale,RoundingMode roundingMode)` | 提供(相对)精确的除法运算,当发生除不尽的情况时,由scale指定精确度 |
| `cn.hutool.core.util.NumberUtil` | `double div(double v1,float v2)` | 提供(相对)精确的除法运算,当发生除不尽的情况的时候,精确到小数点后10位,后面的四舍五入 |
| `cn.hutool.core.util.NumberUtil` | `double div(double v1,float v2,int scale)` | 提供(相对)精确的除法运算,当发生除不尽的情况时,由scale指定精确度,后面的四舍五入 |
| `cn.hutool.core.util.NumberUtil` | `double div(double v1,float v2,int scale,RoundingMode roundingMode)` | 提供(相对)精确的除法运算,当发生除不尽的情况时,由scale指定精确度 |
| `cn.hutool.core.util.NumberUtil` | `double div(float v1,double v2)` | 提供(相对)精确的除法运算,当发生除不尽的情况的时候,精确到小数点后10位,后面的四舍五入 |
| `cn.hutool.core.util.NumberUtil` | `double div(float v1,double v2,int scale)` | 提供(相对)精确的除法运算,当发生除不尽的情况时,由scale指定精确度,后面的四舍五入 |
| `cn.hutool.core.util.NumberUtil` | `double div(float v1,double v2,int scale,RoundingMode roundingMode)` | 提供(相对)精确的除法运算,当发生除不尽的情况时,由scale指定精确度 |
| `cn.hutool.core.util.NumberUtil` | `double div(float v1,float v2)` | 提供(相对)精确的除法运算,当发生除不尽的情况的时候,精确到小数点后10位,后面的四舍五入 |
| `cn.hutool.core.util.NumberUtil` | `double div(float v1,float v2,int scale)` | 提供(相对)精确的除法运算,当发生除不尽的情况时,由scale指定精确度,后面的四舍五入 |
| `cn.hutool.core.util.NumberUtil` | `double div(float v1,float v2,int scale,RoundingMode roundingMode)` | 提供(相对)精确的除法运算,当发生除不尽的情况时,由scale指定精确度 |
| `cn.hutool.core.util.NumberUtil` | `double max(double... numberArray)` | 取最大值 |
| `cn.hutool.core.util.NumberUtil` | `double min(double... numberArray)` | 取最小值 |
| `cn.hutool.core.util.NumberUtil` | `double mul(Double v1,Double v2)` | 提供精确的乘法运算 如果传入多个值为null或者空，则返回0 |
| `cn.hutool.core.util.NumberUtil` | `double mul(double v1,double v2)` | 提供精确的乘法运算 |
| `cn.hutool.core.util.NumberUtil` | `double mul(double v1,float v2)` | 提供精确的乘法运算 |
| `cn.hutool.core.util.NumberUtil` | `double mul(float v1,double v2)` | 提供精确的乘法运算 |
| `cn.hutool.core.util.NumberUtil` | `double mul(float v1,float v2)` | 提供精确的乘法运算 |
| `cn.hutool.core.util.NumberUtil` | `double nullToZero(Double number)` | 如果给定值为null，返回0，否则返回原值 |
| `cn.hutool.core.util.NumberUtil` | `double parseDouble(String number)` | 解析转换数字字符串为long型数字，规则如下： |
| `cn.hutool.core.util.NumberUtil` | `double sub(Double v1,Double v2)` | 提供精确的减法运算 |
| `cn.hutool.core.util.NumberUtil` | `double sub(double v1,double v2)` | 提供精确的减法运算 |
| `cn.hutool.core.util.NumberUtil` | `double sub(double v1,float v2)` | 提供精确的减法运算 |
| `cn.hutool.core.util.NumberUtil` | `double sub(float v1,double v2)` | 提供精确的减法运算 |
| `cn.hutool.core.util.NumberUtil` | `double sub(float v1,float v2)` | 提供精确的减法运算 |
| `cn.hutool.core.util.NumberUtil` | `double toDouble(Number value)` | Number值转换为double float强制转换存在精度问题，此方法避免精度丢失 |
| `cn.hutool.core.util.NumberUtil` | `float max(float... numberArray)` | 取最大值 |
| `cn.hutool.core.util.NumberUtil` | `float min(float... numberArray)` | 取最小值 |
| `cn.hutool.core.util.NumberUtil` | `float nullToZero(Float number)` | 如果给定值为null，返回0，否则返回原值 |
| `cn.hutool.core.util.NumberUtil` | `float parseFloat(String number)` | 解析转换数字字符串为long型数字，规则如下： |
| `cn.hutool.core.util.NumberUtil` | `int binaryToInt(String binaryStr)` | 二进制转int |
| `cn.hutool.core.util.NumberUtil` | `int ceilDiv(int v1,int v2)` | 补充Math.ceilDiv() JDK8中添加了和Math.floorDiv()但却没有ceilDiv() |
| `cn.hutool.core.util.NumberUtil` | `int compare(byte x,byte y)` | 比较两个值的大小 |
| `cn.hutool.core.util.NumberUtil` | `int compare(char x,char y)` | 比较两个值的大小 |
| `cn.hutool.core.util.NumberUtil` | `int compare(double x,double y)` | 比较两个值的大小 |
| `cn.hutool.core.util.NumberUtil` | `int compare(int x,int y)` | 比较两个值的大小 |
| `cn.hutool.core.util.NumberUtil` | `int compare(long x,long y)` | 比较两个值的大小 |
| `cn.hutool.core.util.NumberUtil` | `int compare(short x,short y)` | 比较两个值的大小 |
| `cn.hutool.core.util.NumberUtil` | `int count(int total,int part)` | 计算等份个数 |
| `cn.hutool.core.util.NumberUtil` | `int divisor(int m,int n)` | 最大公约数 |
| `cn.hutool.core.util.NumberUtil` | `int max(int... numberArray)` | 取最大值 |
| `cn.hutool.core.util.NumberUtil` | `int min(int... numberArray)` | 取最小值 |
| `cn.hutool.core.util.NumberUtil` | `int multiple(int m,int n)` | 最小公倍数 |
| `cn.hutool.core.util.NumberUtil` | `int nullToZero(Integer number)` | 如果给定值为null，返回0，否则返回原值 |
| `cn.hutool.core.util.NumberUtil` | `int parseInt(String number)` | 解析转换数字字符串为int型数字，规则如下： |
| `cn.hutool.core.util.NumberUtil` | `int partValue(int total,int partCount)` | 把给定的总数平均分成N份，返回每份的个数 当除以分数有余数时每份+1 |
| `cn.hutool.core.util.NumberUtil` | `int partValue(int total,int partCount,boolean isPlusOneWhenHasRem)` | 把给定的总数平均分成N份，返回每份的个数 如果isPlusOneWhenHasRem为true，则当除以分数有余数时每份+1，否则丢弃余数部分 |
| `cn.hutool.core.util.NumberUtil` | `int processMultiple(int selectNum,int minNum)` | 可以用于计算双色球、大乐透注数的方法 比如大乐透35选5可以这样调用processMultiple(7,5); 就是数学中的：C75=7*6/2*1 |
| `cn.hutool.core.util.NumberUtil` | `int toInt(byte[] bytes)` | byte数组转int，使用大端字节序（高位字节在前，低位字节在后） 见： http://www.ruanyifeng.com/blog/2016/11/byte-order.html |
| `cn.hutool.core.util.NumberUtil` | `int zero2One(int value)` | 如果给定值为0，返回1，否则返回原值 |
| `cn.hutool.core.util.NumberUtil` | `int[] generateRandomNumber(int begin,int end,int size)` | 生成不重复随机数 根据给定的最小数字和最大数字，以及随机数的个数，产生指定的不重复的数组 |
| `cn.hutool.core.util.NumberUtil` | `int[] generateRandomNumber(int begin,int end,int size,int[] seed)` | 生成不重复随机数 根据给定的最小数字和最大数字，以及随机数的个数，产生指定的不重复的数组 |
| `cn.hutool.core.util.NumberUtil` | `int[] range(int start,int stop)` | 给定范围内的整数列表，步进为1 |
| `cn.hutool.core.util.NumberUtil` | `int[] range(int start,int stop,int step)` | 给定范围内的整数列表 |
| `cn.hutool.core.util.NumberUtil` | `int[] range(int stop)` | 从0开始给定范围内的整数列表，步进为1 |
| `cn.hutool.core.util.NumberUtil` | `long binaryToLong(String binaryStr)` | 二进制转long |
| `cn.hutool.core.util.NumberUtil` | `long factorial(long n)` | 计算阶乘 n! = n * (n-1) * ... * 2 * 1 |
| `cn.hutool.core.util.NumberUtil` | `long factorial(long start,long end)` | 计算范围阶乘 factorial(start, end) = start * (start - 1) * ... * (end + 1) |
| `cn.hutool.core.util.NumberUtil` | `long max(long... numberArray)` | 取最大值 |
| `cn.hutool.core.util.NumberUtil` | `long min(long... numberArray)` | 取最小值 |
| `cn.hutool.core.util.NumberUtil` | `long nullToZero(Long number)` | 如果给定值为null，返回0，否则返回原值 |
| `cn.hutool.core.util.NumberUtil` | `long parseLong(String number)` | 解析转换数字字符串为long型数字，规则如下： |
| `cn.hutool.core.util.NumberUtil` | `long sqrt(long x)` | 平方根算法 推荐使用 Math#sqrt(double) |
| `cn.hutool.core.util.NumberUtil` | `short max(short... numberArray)` | 取最大值 |
| `cn.hutool.core.util.NumberUtil` | `short min(short... numberArray)` | 取最小值 |
| `cn.hutool.core.util.NumberUtil` | `short nullToZero(Short number)` | 如果给定值为null，返回0，否则返回原值 |
| `cn.hutool.core.util.ObjectUtil` | `Class<?> getTypeArgument(Object obj)` | 获得给定类的第一个泛型参数 |
| `cn.hutool.core.util.ObjectUtil` | `Class<?> getTypeArgument(Object obj,int index)` | 获得给定类的第一个泛型参数 |
| `cn.hutool.core.util.ObjectUtil` | `R apply(final T source,final Function<T, R> handler)` | 如果指定的对象不为 null,则应用提供的映射函数并返回结果,否则返回 null。 |
| `cn.hutool.core.util.ObjectUtil` | `String toString(Object obj)` | 将Object转为String 策略为： |
| `cn.hutool.core.util.ObjectUtil` | `T clone(T obj)` | 克隆对象 如果对象实现Cloneable接口，调用其clone方法 如果实现Serializable接口，执行深度克隆 否则返回null |
| `cn.hutool.core.util.ObjectUtil` | `T cloneByStream(T obj)` | 序列化后拷贝流的方式克隆 对象必须实现Serializable接口 |
| `cn.hutool.core.util.ObjectUtil` | `T cloneIfPossible(final T obj)` | 返回克隆后的对象，如果克隆失败，返回原对象 |
| `cn.hutool.core.util.ObjectUtil` | `T defaultIfBlank(T str,Function<T, ? extends T> defaultValueSupplier)` | 如果被检查对象为 null 或 "" 或 空白字符串时，返回默认值（由 defaultValueSupplier 提供）；否则直接返回 |
| `cn.hutool.core.util.ObjectUtil` | `T defaultIfBlank(T str,Supplier<? extends T> defaultValueSupplier)` | 如果被检查对象为 null 或 "" 或 空白字符串时，返回默认值（由 defaultValueSupplier 提供）；否则直接返回 |
| `cn.hutool.core.util.ObjectUtil` | `T defaultIfBlank(final T str,final T defaultValue)` | 如果给定对象为null或者""或者空白符返回默认值 |
| `cn.hutool.core.util.ObjectUtil` | `T defaultIfEmpty(String str,Function<CharSequence, ? extends T> handle,final T defaultValue)` | 如果给定对象为null或者""返回默认值, 否则返回自定义handle处理后的返回值 |
| `cn.hutool.core.util.ObjectUtil` | `T defaultIfEmpty(String str,Supplier<? extends T> handle,final T defaultValue)` | 如果给定对象为null或者""返回默认值, 否则返回自定义handle处理后的返回值 |
| `cn.hutool.core.util.ObjectUtil` | `T defaultIfEmpty(T str,Function<T, ? extends T> defaultValueSupplier)` | 如果被检查对象为 null 或 "" 时，返回默认值（由 defaultValueSupplier 提供）；否则直接返回 |
| `cn.hutool.core.util.ObjectUtil` | `T defaultIfEmpty(T str,Supplier<? extends T> defaultValueSupplier)` | 如果被检查对象为 null 或 "" 时，返回默认值（由 defaultValueSupplier 提供）；否则直接返回 |
| `cn.hutool.core.util.ObjectUtil` | `T defaultIfEmpty(final T str,final T defaultValue)` | 如果给定对象为null或者 "" 返回默认值 |
| `cn.hutool.core.util.ObjectUtil` | `T defaultIfNull(Object source,Supplier<? extends T> handle,final T defaultValue)` | 如果给定对象为null 返回默认值, 如果不为null 返回自定义handle处理后的返回值 |
| `cn.hutool.core.util.ObjectUtil` | `T defaultIfNull(R source,Function<R, ? extends T> handle,final T defaultValue)` | 如果给定对象为null 返回默认值, 如果不为null 返回自定义handle处理后的返回值 |
| `cn.hutool.core.util.ObjectUtil` | `T defaultIfNull(T source,Function<T, ? extends T> defaultValueSupplier)` | 如果被检查对象为 null， 返回默认值（由 defaultValueSupplier 提供）；否则直接返回 |
| `cn.hutool.core.util.ObjectUtil` | `T defaultIfNull(T source,Supplier<? extends T> defaultValueSupplier)` | 如果被检查对象为 null， 返回默认值（由 defaultValueSupplier 提供）；否则直接返回 |
| `cn.hutool.core.util.ObjectUtil` | `T defaultIfNull(final T object,final T defaultValue)` | 如果给定对象为null返回默认值 |
| `cn.hutool.core.util.ObjectUtil` | `T deserialize(byte[] bytes,Class<?>... acceptClasses)` | 反序列化 对象必须实现Serializable接口 注意！！！ 此方法不会检查反序列化安全，可能存在反序列化漏洞风险！！！ |
| `cn.hutool.core.util.ObjectUtil` | `boolean contains(Object obj,Object element)` | 对象中是否包含元素 支持的对象类型包括： CharSequence Collection Map Iterator Enumeration Array |
| `cn.hutool.core.util.ObjectUtil` | `boolean equal(Object obj1,Object obj2)` | 比较两个对象是否相等。 相同的条件有两个，满足其一即可： obj1 == null && obj2 == null obj1.equals(obj2) 如果是BigDecimal比较，0 == obj1.compareTo(obj2) |
| `cn.hutool.core.util.ObjectUtil` | `boolean equals(Object obj1,Object obj2)` | 比较两个对象是否相等，此方法是 #equal(Object, Object)的别名方法。 相同的条件有两个，满足其一即可： obj1 == null && obj2 == null obj1.equals(obj2) 如果是BigDecimal比较，0 == obj1.compareTo(obj2) |
| `cn.hutool.core.util.ObjectUtil` | `boolean hasEmpty(Object... objs)` | 是否存在null或空对象，通过ObjectUtil#isEmpty(Object) 判断元素 |
| `cn.hutool.core.util.ObjectUtil` | `boolean hasNull(Object... objs)` | 是否存在null对象，通过ObjectUtil#isNull(Object) 判断元素 |
| `cn.hutool.core.util.ObjectUtil` | `boolean isAllEmpty(Object... objs)` | 是否全都为null或空对象，通过ObjectUtil#isEmpty(Object) 判断元素 |
| `cn.hutool.core.util.ObjectUtil` | `boolean isAllNotEmpty(Object... objs)` | 是否全都不为null或空对象，通过ObjectUtil#isEmpty(Object) 判断元素 |
| `cn.hutool.core.util.ObjectUtil` | `boolean isBasicType(Object object)` | 是否为基本类型，包括包装类型和非包装类型 |
| `cn.hutool.core.util.ObjectUtil` | `boolean isEmpty(Object obj)` | 判断指定对象是否为空，支持： |
| `cn.hutool.core.util.ObjectUtil` | `boolean isNotEmpty(Object obj)` | 判断指定对象是否为非空，支持： |
| `cn.hutool.core.util.ObjectUtil` | `boolean isNotNull(Object obj)` | 检查对象是否不为null |
| `cn.hutool.core.util.ObjectUtil` | `boolean isNull(Object obj)` | 检查对象是否为null 判断标准为： |
| `cn.hutool.core.util.ObjectUtil` | `boolean isValidIfNumber(Object obj)` | 检查是否为有效的数字 检查Double和Float是否为无限大，或者Not a Number 非数字类型和Null将返回true |
| `cn.hutool.core.util.ObjectUtil` | `boolean notEqual(Object obj1,Object obj2)` | 比较两个对象是否不相等。 |
| `cn.hutool.core.util.ObjectUtil` | `byte[] serialize(T obj)` | 序列化 对象必须实现Serializable接口 |
| `cn.hutool.core.util.ObjectUtil` | `int compare(T c1,T c2)` | null安全的对象比较，null对象排在末尾 |
| `cn.hutool.core.util.ObjectUtil` | `int compare(T c1,T c2,boolean nullGreater)` | null安全的对象比较 |
| `cn.hutool.core.util.ObjectUtil` | `int emptyCount(Object... objs)` | 存在多少个null或空对象，通过ObjectUtil#isEmpty(Object) 判断元素 |
| `cn.hutool.core.util.ObjectUtil` | `int length(Object obj)` | 计算对象长度，支持类型包括： null：默认返回0； 数组：返回数组长度； CharSequence：返回CharSequence#length()； Collection：返回Collection#size()； Iterator或Iterable：可迭代的元素数量；副作用：Iterator只能被迭代一次 Enumeration：返回可迭代的元素数量；副作用：Enumeration只能被迭代一次 |
| `cn.hutool.core.util.ObjectUtil` | `void accept(final T source,final Consumer<T> consumer)` | 如果指定的对象不为 null,则执行Consumer处理source，否则不进行操作 |
| `cn.hutool.core.util.PageUtil` | `Segment<Integer> toSegment(int pageNo,int pageSize)` | 将页数和每页条目数转换为开始位置和结束位置 此方法用于包括结束位置的分页方法 例如： |
| `cn.hutool.core.util.PageUtil` | `int getEnd(int pageNo,int pageSize)` | 将页数和每页条目数转换为结束位置 此方法用于不包括结束位置的分页方法 例如： |
| `cn.hutool.core.util.PageUtil` | `int getFirstPageNo()` | 获得首页的页码，可以为0或者1 |
| `cn.hutool.core.util.PageUtil` | `int getStart(int pageNo,int pageSize)` | 将页数和每页条目数转换为开始位置 此方法用于不包括结束位置的分页方法 例如： |
| `cn.hutool.core.util.PageUtil` | `int totalPage(int totalCount,int pageSize)` | 根据总数计算总页数 |
| `cn.hutool.core.util.PageUtil` | `int totalPage(long totalCount,int pageSize)` | 根据总数计算总页数 |
| `cn.hutool.core.util.PageUtil` | `int[] rainbow(int currentPage,int pageCount)` | 分页彩虹算法(默认展示10页) 来自： https://github.com/iceroot/iceroot/blob/master/src/main/java/com/icexxx/util/IceUtil.java |
| `cn.hutool.core.util.PageUtil` | `int[] rainbow(int pageNo,int totalPage,int displayCount)` | 分页彩虹算法 来自： https://github.com/iceroot/iceroot/blob/master/src/main/java/com/icexxx/util/IceUtil.java 通过传入的信息，生成一个分页列表显示 |
| `cn.hutool.core.util.PageUtil` | `int[] transToStartEnd(int pageNo,int pageSize)` | 将页数和每页条目数转换为开始位置和结束位置 此方法用于包括结束位置的分页方法 例如： |
| `cn.hutool.core.util.PageUtil` | `void setFirstPageNo(int customFirstPageNo)` | 设置首页页码，可以为0或者1 |
| `cn.hutool.core.util.PageUtil` | `void setOneAsFirstPageNo()` | 设置首页页码为1 |
| `cn.hutool.core.util.PhoneUtil` | `CharSequence hideAfter(CharSequence phone)` | 隐藏手机号最后4位 替换字符为"*" |
| `cn.hutool.core.util.PhoneUtil` | `CharSequence hideBefore(CharSequence phone)` | 隐藏手机号前7位 替换字符为"*" 栗子 |
| `cn.hutool.core.util.PhoneUtil` | `CharSequence hideBetween(CharSequence phone)` | 隐藏手机号中间4位 替换字符为"*" |
| `cn.hutool.core.util.PhoneUtil` | `CharSequence subAfter(CharSequence phone)` | 获取手机号后4位 |
| `cn.hutool.core.util.PhoneUtil` | `CharSequence subBefore(CharSequence phone)` | 获取手机号前3位 |
| `cn.hutool.core.util.PhoneUtil` | `CharSequence subBetween(CharSequence phone)` | 获取手机号中间4位 |
| `cn.hutool.core.util.PhoneUtil` | `CharSequence subTelAfter(CharSequence value)` | 获取固话号码中的号码 |
| `cn.hutool.core.util.PhoneUtil` | `CharSequence subTelBefore(CharSequence value)` | 获取固话号码中的区号 |
| `cn.hutool.core.util.PhoneUtil` | `boolean isMobile(CharSequence value)` | 验证是否为手机号码（中国大陆） |
| `cn.hutool.core.util.PhoneUtil` | `boolean isMobileHk(CharSequence value)` | 验证是否为手机号码（中国香港） |
| `cn.hutool.core.util.PhoneUtil` | `boolean isMobileMo(CharSequence value)` | 验证是否为手机号码（中国澳门） |
| `cn.hutool.core.util.PhoneUtil` | `boolean isMobileTw(CharSequence value)` | 验证是否为手机号码（中国台湾） |
| `cn.hutool.core.util.PhoneUtil` | `boolean isPhone(CharSequence value)` | 验证是否为座机号码+手机号码（CharUtil中国）+ 400 + 800电话 + 手机号号码（中国香港） |
| `cn.hutool.core.util.PhoneUtil` | `boolean isTel(CharSequence value)` | 验证是否为座机号码（中国大陆） |
| `cn.hutool.core.util.PhoneUtil` | `boolean isTel400800(CharSequence value)` | 验证是否为座机号码（中国大陆）+ 400 + 800 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `Boolean[] wrap(boolean... values)` | 将原始类型数组包装为包装类型 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `Byte[] wrap(byte... values)` | 将原始类型数组包装为包装类型 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `Character[] wrap(char... values)` | 将原始类型数组包装为包装类型 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `Double[] wrap(double... values)` | 将原始类型数组包装为包装类型 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `Float[] wrap(float... values)` | 将原始类型数组包装为包装类型 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `Integer[] wrap(int... values)` | 将原始类型数组包装为包装类型 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `Long[] wrap(long... values)` | 将原始类型数组包装为包装类型 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `Object remove(Object array,int index)` | 移除数组中对应位置的元素 copy from commons-lang |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `Short[] wrap(short... values)` | 将原始类型数组包装为包装类型 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean contains(boolean[] array,boolean value)` | 数组中是否包含元素 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean contains(byte[] array,byte value)` | 数组中是否包含元素 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean contains(char[] array,char value)` | 数组中是否包含元素 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean contains(double[] array,double value)` | 数组中是否包含元素 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean contains(float[] array,float value)` | 数组中是否包含元素 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean contains(int[] array,int value)` | 数组中是否包含元素 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean contains(long[] array,long value)` | 数组中是否包含元素 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean contains(short[] array,short value)` | 数组中是否包含元素 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isEmpty(boolean[] array)` | 数组是否为空 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isEmpty(byte[] array)` | 数组是否为空 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isEmpty(char[] array)` | 数组是否为空 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isEmpty(double[] array)` | 数组是否为空 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isEmpty(float[] array)` | 数组是否为空 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isEmpty(int[] array)` | 数组是否为空 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isEmpty(long[] array)` | 数组是否为空 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isEmpty(short[] array)` | 数组是否为空 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isNotEmpty(boolean[] array)` | 数组是否为非空 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isNotEmpty(byte[] array)` | 数组是否为非空 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isNotEmpty(char[] array)` | 数组是否为非空 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isNotEmpty(double[] array)` | 数组是否为非空 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isNotEmpty(float[] array)` | 数组是否为非空 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isNotEmpty(int[] array)` | 数组是否为非空 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isNotEmpty(long[] array)` | 数组是否为非空 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isNotEmpty(short[] array)` | 数组是否为非空 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isSorted(byte[] array)` | 检查数组是否升序，即array[i] <= array[i+1]，若传入空数组，则返回false |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isSorted(char[] array)` | 检查数组是否升序，即array[i] <= array[i+1]，若传入空数组，则返回false |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isSorted(double[] array)` | 检查数组是否升序，即array[i] <= array[i+1]，若传入空数组，则返回false |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isSorted(float[] array)` | 检查数组是否升序，即array[i] <= array[i+1]，若传入空数组，则返回false |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isSorted(int[] array)` | 检查数组是否升序，即array[i] <= array[i+1]，若传入空数组，则返回false |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isSorted(long[] array)` | 检查数组是否升序，即array[i] <= array[i+1]，若传入空数组，则返回false |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isSorted(short[] array)` | 检查数组是否升序，即array[i] <= array[i+1]，若传入空数组，则返回false |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isSortedASC(byte[] array)` | 检查数组是否升序，即array[i] <= array[i+1]，若传入空数组，则返回false |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isSortedASC(char[] array)` | 检查数组是否升序，即array[i] <= array[i+1]，若传入空数组，则返回false |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isSortedASC(double[] array)` | 检查数组是否升序，即array[i] <= array[i+1]，若传入空数组，则返回false |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isSortedASC(float[] array)` | 检查数组是否升序，即array[i] <= array[i+1]，若传入空数组，则返回false |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isSortedASC(int[] array)` | 检查数组是否升序，即array[i] <= array[i+1]，若传入空数组，则返回false |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isSortedASC(long[] array)` | 检查数组是否升序，即array[i] <= array[i+1]，若传入空数组，则返回false |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isSortedASC(short[] array)` | 检查数组是否升序，即array[i] <= array[i+1]，若传入空数组，则返回false |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isSortedDESC(byte[] array)` | 检查数组是否降序，即array[i] >= array[i+1]，若传入空数组，则返回false |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isSortedDESC(char[] array)` | 检查数组是否降序，即array[i] >= array[i+1]，若传入空数组，则返回false |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isSortedDESC(double[] array)` | 检查数组是否降序，即array[i] >= array[i+1]，若传入空数组，则返回false |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isSortedDESC(float[] array)` | 检查数组是否降序，即array[i] >= array[i+1]，若传入空数组，则返回false |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isSortedDESC(int[] array)` | 检查数组是否降序，即array[i] >= array[i+1]，若传入空数组，则返回false |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isSortedDESC(long[] array)` | 检查数组是否降序，即array[i] >= array[i+1]，若传入空数组，则返回false |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean isSortedDESC(short[] array)` | 检查数组是否降序，即array[i] >= array[i+1]，若传入空数组，则返回false |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean[] addAll(boolean[]... arrays)` | 将多个数组合并在一起 忽略null的数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean[] remove(boolean[] array,int index)` | 移除数组中对应位置的元素 copy from commons-lang |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean[] removeEle(boolean[] array,boolean element)` | 移除数组中指定的元素 只会移除匹配到的第一个元素 copy from commons-lang |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean[] reverse(boolean[] array)` | 反转数组，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean[] reverse(boolean[] array,final int startIndexInclusive,final int endIndexExclusive)` | 反转数组，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean[] shuffle(boolean[] array)` | 打乱数组顺序，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean[] shuffle(boolean[] array,Random random)` | 打乱数组顺序，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean[] sub(boolean[] array,int start,int end)` | 获取子数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean[] swap(boolean[] array,int index1,int index2)` | 交换数组中两个位置的值 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `boolean[] unWrap(Boolean... values)` | 包装类数组转为原始类型数组 null 按照 false 对待 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `byte max(byte... numberArray)` | 取最大值 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `byte min(byte... numberArray)` | 取最小值 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `byte[] addAll(byte[]... arrays)` | 将多个数组合并在一起 忽略null的数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `byte[] remove(byte[] array,int index)` | 移除数组中对应位置的元素 copy from commons-lang |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `byte[] removeEle(byte[] array,byte element)` | 移除数组中指定的元素 只会移除匹配到的第一个元素 copy from commons-lang |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `byte[] resize(byte[] bytes,int newSize)` | 生成一个新的重新设置大小的数组 调整大小后拷贝原数组到新数组下。扩大则占位前N个位置，其它位置补充0，缩小则截断 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `byte[] reverse(byte[] array)` | 反转数组，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `byte[] reverse(byte[] array,final int startIndexInclusive,final int endIndexExclusive)` | 反转数组，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `byte[] shuffle(byte[] array)` | 打乱数组顺序，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `byte[] shuffle(byte[] array,Random random)` | 打乱数组顺序，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `byte[] sub(byte[] array,int start,int end)` | 获取子数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `byte[] swap(byte[] array,int index1,int index2)` | 交换数组中两个位置的值 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `byte[] unWrap(Byte... values)` | 包装类数组转为原始类型数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `byte[][] split(byte[] array,int len)` | 拆分byte数组为几个等份（最后一份按照剩余长度分配空间） |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `char max(char... numberArray)` | 取最大值 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `char min(char... numberArray)` | 取最小值 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `char[] addAll(char[]... arrays)` | 将多个数组合并在一起 忽略null的数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `char[] remove(char[] array,int index)` | 移除数组中对应位置的元素 copy from commons-lang |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `char[] removeEle(char[] array,char element)` | 移除数组中指定的元素 只会移除匹配到的第一个元素 copy from commons-lang |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `char[] reverse(char[] array)` | 反转数组，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `char[] reverse(char[] array,final int startIndexInclusive,final int endIndexExclusive)` | 反转数组，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `char[] shuffle(char[] array)` | 打乱数组顺序，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `char[] shuffle(char[] array,Random random)` | 打乱数组顺序，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `char[] sub(char[] array,int start,int end)` | 获取子数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `char[] swap(char[] array,int index1,int index2)` | 交换数组中两个位置的值 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `char[] unWrap(Character... values)` | 包装类数组转为原始类型数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `double max(double... numberArray)` | 取最大值 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `double min(double... numberArray)` | 取最小值 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `double[] addAll(double[]... arrays)` | 将多个数组合并在一起 忽略null的数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `double[] remove(double[] array,int index)` | 移除数组中对应位置的元素 copy from commons-lang |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `double[] removeEle(double[] array,double element)` | 移除数组中指定的元素 只会移除匹配到的第一个元素 copy from commons-lang |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `double[] reverse(double[] array)` | 反转数组，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `double[] reverse(double[] array,final int startIndexInclusive,final int endIndexExclusive)` | 反转数组，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `double[] shuffle(double[] array)` | 打乱数组顺序，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `double[] shuffle(double[] array,Random random)` | 打乱数组顺序，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `double[] sub(double[] array,int start,int end)` | 获取子数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `double[] swap(double[] array,int index1,int index2)` | 交换数组中两个位置的值 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `double[] unWrap(Double... values)` | 包装类数组转为原始类型数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `float max(float... numberArray)` | 取最大值 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `float min(float... numberArray)` | 取最小值 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `float[] addAll(float[]... arrays)` | 将多个数组合并在一起 忽略null的数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `float[] remove(float[] array,int index)` | 移除数组中对应位置的元素 copy from commons-lang |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `float[] removeEle(float[] array,float element)` | 移除数组中指定的元素 只会移除匹配到的第一个元素 copy from commons-lang |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `float[] reverse(float[] array)` | 反转数组，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `float[] reverse(float[] array,final int startIndexInclusive,final int endIndexExclusive)` | 反转数组，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `float[] shuffle(float[] array)` | 打乱数组顺序，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `float[] shuffle(float[] array,Random random)` | 打乱数组顺序，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `float[] sub(float[] array,int start,int end)` | 获取子数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `float[] swap(float[] array,int index1,int index2)` | 交换数组中两个位置的值 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `float[] unWrap(Float... values)` | 包装类数组转为原始类型数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int indexOf(boolean[] array,boolean value)` | 返回数组中指定元素所在位置，未找到返回#INDEX_NOT_FOUND |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int indexOf(byte[] array,byte value)` | 返回数组中指定元素所在位置，未找到返回#INDEX_NOT_FOUND |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int indexOf(char[] array,char value)` | 返回数组中指定元素所在位置，未找到返回#INDEX_NOT_FOUND |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int indexOf(double[] array,double value)` | 返回数组中指定元素所在位置，未找到返回#INDEX_NOT_FOUND |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int indexOf(float[] array,float value)` | 返回数组中指定元素所在位置，未找到返回#INDEX_NOT_FOUND |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int indexOf(int[] array,int value)` | 返回数组中指定元素所在位置，未找到返回#INDEX_NOT_FOUND |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int indexOf(long[] array,long value)` | 返回数组中指定元素所在位置，未找到返回#INDEX_NOT_FOUND |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int indexOf(short[] array,short value)` | 返回数组中指定元素所在位置，未找到返回#INDEX_NOT_FOUND |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int lastIndexOf(boolean[] array,boolean value)` | 返回数组中指定元素所在最后的位置，未找到返回#INDEX_NOT_FOUND |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int lastIndexOf(byte[] array,byte value)` | 返回数组中指定元素所在最后的位置，未找到返回#INDEX_NOT_FOUND |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int lastIndexOf(char[] array,char value)` | 返回数组中指定元素所在最后的位置，未找到返回#INDEX_NOT_FOUND |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int lastIndexOf(double[] array,double value)` | 返回数组中指定元素所在最后的位置，未找到返回#INDEX_NOT_FOUND |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int lastIndexOf(float[] array,float value)` | 返回数组中指定元素所在最后的位置，未找到返回#INDEX_NOT_FOUND |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int lastIndexOf(int[] array,int value)` | 返回数组中指定元素所在最后的位置，未找到返回#INDEX_NOT_FOUND |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int lastIndexOf(long[] array,long value)` | 返回数组中指定元素所在最后的位置，未找到返回#INDEX_NOT_FOUND |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int lastIndexOf(short[] array,short value)` | 返回数组中指定元素所在最后的位置，未找到返回#INDEX_NOT_FOUND |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int max(int... numberArray)` | 取最大值 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int min(int... numberArray)` | 取最小值 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int[] addAll(int[]... arrays)` | 将多个数组合并在一起 忽略null的数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int[] range(int excludedEnd)` | 生成一个从0开始的数字列表 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int[] range(int includedStart,int excludedEnd)` | 生成一个数字列表 自动判定正序反序 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int[] range(int includedStart,int excludedEnd,int step)` | 生成一个数字列表 自动判定正序反序 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int[] remove(int[] array,int index)` | 移除数组中对应位置的元素 copy from commons-lang |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int[] removeEle(int[] array,int element)` | 移除数组中指定的元素 只会移除匹配到的第一个元素 copy from commons-lang |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int[] reverse(int[] array)` | 反转数组，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int[] reverse(int[] array,final int startIndexInclusive,final int endIndexExclusive)` | 反转数组，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int[] shuffle(int[] array)` | 打乱数组顺序，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int[] shuffle(int[] array,Random random)` | 打乱数组顺序，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int[] sub(int[] array,int start,int end)` | 获取子数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int[] swap(int[] array,int index1,int index2)` | 交换数组中两个位置的值 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `int[] unWrap(Integer... values)` | 包装类数组转为原始类型数组，null转为0 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `long max(long... numberArray)` | 取最大值 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `long min(long... numberArray)` | 取最小值 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `long[] addAll(long[]... arrays)` | 将多个数组合并在一起 忽略null的数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `long[] remove(long[] array,int index)` | 移除数组中对应位置的元素 copy from commons-lang |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `long[] removeEle(long[] array,long element)` | 移除数组中指定的元素 只会移除匹配到的第一个元素 copy from commons-lang |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `long[] reverse(long[] array)` | 反转数组，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `long[] reverse(long[] array,final int startIndexInclusive,final int endIndexExclusive)` | 反转数组，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `long[] shuffle(long[] array)` | 打乱数组顺序，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `long[] shuffle(long[] array,Random random)` | 打乱数组顺序，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `long[] sub(long[] array,int start,int end)` | 获取子数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `long[] swap(long[] array,int index1,int index2)` | 交换数组中两个位置的值 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `long[] unWrap(Long... values)` | 包装类数组转为原始类型数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `short max(short... numberArray)` | 取最大值 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `short min(short... numberArray)` | 取最小值 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `short[] addAll(short[]... arrays)` | 将多个数组合并在一起 忽略null的数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `short[] remove(short[] array,int index)` | 移除数组中对应位置的元素 copy from commons-lang |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `short[] removeEle(short[] array,short element)` | 移除数组中指定的元素 只会移除匹配到的第一个元素 copy from commons-lang |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `short[] reverse(short[] array)` | 反转数组，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `short[] reverse(short[] array,final int startIndexInclusive,final int endIndexExclusive)` | 反转数组，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `short[] shuffle(short[] array)` | 打乱数组顺序，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `short[] shuffle(short[] array,Random random)` | 打乱数组顺序，会变更原数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `short[] sub(short[] array,int start,int end)` | 获取子数组 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `short[] swap(short[] array,int index1,int index2)` | 交换数组中两个位置的值 |
| `cn.hutool.core.util.PrimitiveArrayUtil` | `short[] unWrap(Short... values)` | 包装类数组转为原始类型数组 |
| `cn.hutool.core.util.RadixUtil` | `String encode(String radixs,int num)` | 把一个整型数值转换成自己定义的进制 长度即进制 encode("AB",10) 51转换成2进制，A=0;B=1 。 二进制1010，结果 BABA encode("VIP",21) 21转换成3进制，V=0;I=1;P=2 ，三进制210 ,得到结果PIV |
| `cn.hutool.core.util.RadixUtil` | `String encode(String radixs,long num)` | 把一个长整型数值转换成自己定义的进制 |
| `cn.hutool.core.util.RadixUtil` | `int decodeToInt(String radixs,String encodeStr)` | 把转换后的进制字符还原成int 值 |
| `cn.hutool.core.util.RadixUtil` | `long decode(String radixs,String encodeStr)` | 把转换后进制的字符还原成long 值 |
| `cn.hutool.core.util.RandomUtil` | `BigDecimal randomBigDecimal()` | 获得指定范围内的随机数[0, 1) |
| `cn.hutool.core.util.RandomUtil` | `BigDecimal randomBigDecimal(final BigDecimal limit)` | 获得指定范围内的随机数 [0,limit) |
| `cn.hutool.core.util.RandomUtil` | `BigDecimal randomBigDecimal(final BigDecimal minInclude,final BigDecimal maxExclude)` | 获得指定范围内的随机数 |
| `cn.hutool.core.util.RandomUtil` | `DateTime randomDate(Date baseDate,final DateField dateField,final int min,final int max)` | 以给定日期为基准，随机产生一个日期 |
| `cn.hutool.core.util.RandomUtil` | `DateTime randomDay(final int min,final int max)` | 以当天为基准，随机产生一个日期 |
| `cn.hutool.core.util.RandomUtil` | `List<T> randomEleList(final List<T> source,final int count)` | 随机获得列表中的一定量的元素，返回List 此方法与#randomEles(List, int) 不同点在于，不会获取重复位置的元素 |
| `cn.hutool.core.util.RandomUtil` | `List<T> randomEles(final List<T> list,final int count)` | 随机获得列表中的一定量元素 |
| `cn.hutool.core.util.RandomUtil` | `Random getRandom(final boolean isSecure)` | 获取随机数产生器 |
| `cn.hutool.core.util.RandomUtil` | `SecureRandom createSecureRandom(final byte[] seed)` | 创建SecureRandom，类提供加密的强随机数生成器 (RNG) |
| `cn.hutool.core.util.RandomUtil` | `SecureRandom getSHA1PRNGRandom(final byte[] seed)` | 获取SHA1PRNG的SecureRandom，类提供加密的强随机数生成器 (RNG) 注意：此方法获取的是伪随机序列发生器PRNG（pseudo-random number generator）,在Linux下噪声生成时可能造成较长时间停顿。 see: http://ifeve.com/jvm-random-and-entropy-source/ 相关说明见：https://stackoverflow.com/questions/137212/how-to-solve-slow-java-securerandom |
| `cn.hutool.core.util.RandomUtil` | `SecureRandom getSecureRandom()` | 获取SHA1PRNG的SecureRandom，类提供加密的强随机数生成器 (RNG) 注意：此方法获取的是伪随机序列发生器PRNG（pseudo-random number generator） 相关说明见：https://stackoverflow.com/questions/137212/how-to-solve-slow-java-securerandom |
| `cn.hutool.core.util.RandomUtil` | `SecureRandom getSecureRandom(final byte[] seed)` | 获取SHA1PRNG的SecureRandom，类提供加密的强随机数生成器 (RNG) 注意：此方法获取的是伪随机序列发生器PRNG（pseudo-random number generator） 相关说明见：https://stackoverflow.com/questions/137212/how-to-solve-slow-java-securerandom |
| `cn.hutool.core.util.RandomUtil` | `SecureRandom getSecureRandomStrong()` | 获取algorithms/providers中提供的强安全随机生成器 注意：此方法可能造成阻塞或性能问题 |
| `cn.hutool.core.util.RandomUtil` | `Set<T> randomEleSet(final Collection<T> collection,final int count)` | 随机获得列表中的一定量的不重复元素，返回Set |
| `cn.hutool.core.util.RandomUtil` | `String randomNumbers(final int length)` | 获得一个只包含数字的字符串 |
| `cn.hutool.core.util.RandomUtil` | `String randomString(final String baseString,int length)` | 获得一个随机的字符串 |
| `cn.hutool.core.util.RandomUtil` | `String randomString(final int length)` | 获得一个随机的字符串（只包含数字和字符） |
| `cn.hutool.core.util.RandomUtil` | `String randomStringLower(final int length)` | 获得一个随机的字符串（只包含数字和小写字母） |
| `cn.hutool.core.util.RandomUtil` | `String randomStringLowerWithoutStr(final int length,final String elemData)` | 获得一个随机的字符串（只包含数字和小写字母） 并排除指定字符串 |
| `cn.hutool.core.util.RandomUtil` | `String randomStringUpper(final int length)` | 获得一个随机的字符串（只包含数字和大写字符） |
| `cn.hutool.core.util.RandomUtil` | `String randomStringWithoutStr(final int length,final String elemData)` | 获得一个随机的字符串（只包含数字和字母） 并排除指定字符串 |
| `cn.hutool.core.util.RandomUtil` | `T randomEle(final List<T> list)` | 随机获得列表中的元素 |
| `cn.hutool.core.util.RandomUtil` | `T randomEle(final List<T> list,int limit)` | 随机获得列表中的元素 |
| `cn.hutool.core.util.RandomUtil` | `T randomEle(final T[] array)` | 随机获得数组中的元素 |
| `cn.hutool.core.util.RandomUtil` | `T randomEle(final T[] array,int limit)` | 随机获得数组中的元素 |
| `cn.hutool.core.util.RandomUtil` | `ThreadLocalRandom getRandom()` | 获取随机数生成器对象 ThreadLocalRandom是JDK 7之后提供并发产生随机数，能够解决多个线程发生的竞争争夺。 注意：此方法返回的ThreadLocalRandom不可以在多线程环境下共享对象，否则有重复随机数问题。 见：https://www.jianshu.com/p/89dfe990295c |
| `cn.hutool.core.util.RandomUtil` | `WeightRandom<T> weightRandom(final Iterable<WeightObj<T>> weightObjs)` | 带有权重的随机生成器 |
| `cn.hutool.core.util.RandomUtil` | `WeightRandom<T> weightRandom(final WeightObj<T>[] weightObjs)` | 带有权重的随机生成器 |
| `cn.hutool.core.util.RandomUtil` | `boolean randomBoolean()` | 获得随机Boolean值 |
| `cn.hutool.core.util.RandomUtil` | `byte[] randomBytes(final int length)` | 随机bytes |
| `cn.hutool.core.util.RandomUtil` | `char randomChar()` | 随机字母或数字，小写 |
| `cn.hutool.core.util.RandomUtil` | `char randomChar(final String baseString)` | 随机字符 |
| `cn.hutool.core.util.RandomUtil` | `char randomChinese()` | 随机汉字（'一'-'鿿'） |
| `cn.hutool.core.util.RandomUtil` | `char randomNumber()` | 随机数字，数字为0~9单个数字 |
| `cn.hutool.core.util.RandomUtil` | `double randomDouble()` | 获得随机数[0, 1) |
| `cn.hutool.core.util.RandomUtil` | `double randomDouble(final double limit)` | 获得指定范围内的随机数 [0,limit) |
| `cn.hutool.core.util.RandomUtil` | `double randomDouble(final double limit,final int scale,final RoundingMode roundingMode)` | 获得指定范围内的随机数 |
| `cn.hutool.core.util.RandomUtil` | `double randomDouble(final double minInclude,final double maxExclude)` | 获得指定范围内的随机数 |
| `cn.hutool.core.util.RandomUtil` | `double randomDouble(final double minInclude,final double maxExclude,final int scale,final RoundingMode roundingMode)` | 获得指定范围内的随机数 |
| `cn.hutool.core.util.RandomUtil` | `double randomDouble(final int scale,final RoundingMode roundingMode)` | 获得指定范围内的随机数 |
| `cn.hutool.core.util.RandomUtil` | `float randomFloat()` | 获得随机数[0, 1) |
| `cn.hutool.core.util.RandomUtil` | `float randomFloat(final float limitExclude)` | 获得指定范围内的随机数 [0,limit) |
| `cn.hutool.core.util.RandomUtil` | `float randomFloat(final float minInclude,final float maxExclude)` | 获得指定范围内的随机数[min, max) |
| `cn.hutool.core.util.RandomUtil` | `int randomInt()` | 获得随机数int值 |
| `cn.hutool.core.util.RandomUtil` | `int randomInt(final int limitExclude)` | 获得指定范围内的随机数 [0,limit) |
| `cn.hutool.core.util.RandomUtil` | `int randomInt(final int minInclude,final int maxExclude)` | 获得指定范围内的随机数 |
| `cn.hutool.core.util.RandomUtil` | `int randomInt(int min,int max,final boolean includeMin,final boolean includeMax)` | 获得指定范围内的随机数 |
| `cn.hutool.core.util.RandomUtil` | `int[] randomInts(final int length)` | 创建指定长度的随机索引 |
| `cn.hutool.core.util.RandomUtil` | `long randomLong()` | 获得随机数 |
| `cn.hutool.core.util.RandomUtil` | `long randomLong(final long limitExclude)` | 获得指定范围内的随机数 [0,limit) |
| `cn.hutool.core.util.RandomUtil` | `long randomLong(final long minInclude,final long maxExclude)` | 获得指定范围内的随机数[min, max) |
| `cn.hutool.core.util.RandomUtil` | `long randomLong(long min,long max,final boolean includeMin,final boolean includeMax)` | 获得指定范围内的随机数 |
| `cn.hutool.core.util.ReUtil` | `Integer getFirstNumber(CharSequence StringWithNumber)` | 从字符串中获得第一个整数 |
| `cn.hutool.core.util.ReUtil` | `List<String> findAll(Pattern pattern,CharSequence content,int group)` | 取得内容中匹配的所有结果 |
| `cn.hutool.core.util.ReUtil` | `List<String> findAll(String regex,CharSequence content,int group)` | 取得内容中匹配的所有结果 |
| `cn.hutool.core.util.ReUtil` | `List<String> findAllGroup0(Pattern pattern,CharSequence content)` | 取得内容中匹配的所有结果，获得匹配的所有结果中正则对应分组0的内容 |
| `cn.hutool.core.util.ReUtil` | `List<String> findAllGroup0(String regex,CharSequence content)` | 取得内容中匹配的所有结果，获得匹配的所有结果中正则对应分组0的内容 |
| `cn.hutool.core.util.ReUtil` | `List<String> findAllGroup1(Pattern pattern,CharSequence content)` | 取得内容中匹配的所有结果，获得匹配的所有结果中正则对应分组1的内容 |
| `cn.hutool.core.util.ReUtil` | `List<String> findAllGroup1(String regex,CharSequence content)` | 取得内容中匹配的所有结果，获得匹配的所有结果中正则对应分组1的内容 |
| `cn.hutool.core.util.ReUtil` | `List<String> getAllGroups(Pattern pattern,CharSequence content)` | 获得匹配的字符串匹配到的所有分组 |
| `cn.hutool.core.util.ReUtil` | `List<String> getAllGroups(Pattern pattern,CharSequence content,boolean withGroup0)` | 获得匹配的字符串匹配到的所有分组 |
| `cn.hutool.core.util.ReUtil` | `List<String> getAllGroups(Pattern pattern,CharSequence content,boolean withGroup0,boolean findAll)` | 获得匹配的字符串匹配到的所有分组 |
| `cn.hutool.core.util.ReUtil` | `Map<String, String> getAllGroupNames(Pattern pattern,CharSequence content)` | 根据给定正则查找字符串中的匹配项，返回所有匹配的分组名对应分组值 |
| `cn.hutool.core.util.ReUtil` | `MatchResult indexOf(Pattern pattern,CharSequence content)` | 找到指定模式匹配到字符串的开始位置 |
| `cn.hutool.core.util.ReUtil` | `MatchResult indexOf(String regex,CharSequence content)` | 找到指定正则匹配到字符串的开始位置 |
| `cn.hutool.core.util.ReUtil` | `MatchResult lastIndexOf(Pattern pattern,CharSequence content)` | 找到指定模式匹配到最后一个字符串的位置 |
| `cn.hutool.core.util.ReUtil` | `MatchResult lastIndexOf(String regex,CharSequence content)` | 找到指定正则匹配到第一个字符串的位置 |
| `cn.hutool.core.util.ReUtil` | `String delAll(Pattern pattern,CharSequence content)` | 删除匹配的全部内容 |
| `cn.hutool.core.util.ReUtil` | `String delAll(String regex,CharSequence content)` | 删除匹配的全部内容 |
| `cn.hutool.core.util.ReUtil` | `String delFirst(Pattern pattern,CharSequence content)` | 删除匹配的第一个内容 |
| `cn.hutool.core.util.ReUtil` | `String delFirst(String regex,CharSequence content)` | 删除匹配的第一个内容 |
| `cn.hutool.core.util.ReUtil` | `String delLast(Pattern pattern,CharSequence str)` | 删除匹配的最后一个内容 |
| `cn.hutool.core.util.ReUtil` | `String delLast(String regex,CharSequence str)` | 删除匹配的最后一个内容 |
| `cn.hutool.core.util.ReUtil` | `String delPre(Pattern pattern,CharSequence content)` | 删除正则匹配到的内容之前的字符 如果没有找到，则返回原文 |
| `cn.hutool.core.util.ReUtil` | `String delPre(String regex,CharSequence content)` | 删除正则匹配到的内容之前的字符 如果没有找到，则返回原文 |
| `cn.hutool.core.util.ReUtil` | `String escape(CharSequence content)` | 转义字符串，将正则的关键字转义 |
| `cn.hutool.core.util.ReUtil` | `String escape(char c)` | 转义字符，将正则的关键字转义 |
| `cn.hutool.core.util.ReUtil` | `String extractMulti(Pattern pattern,CharSequence content,String template)` | 从content中匹配出多个值并根据template生成新的字符串 例如： content 2013年5月 pattern (.*?)年(.*?)月 template： $1-$2 return 2013-5 |
| `cn.hutool.core.util.ReUtil` | `String extractMulti(String regex,CharSequence content,String template)` | 从content中匹配出多个值并根据template生成新的字符串 匹配结束后会删除匹配内容之前的内容（包括匹配内容） 例如： content 2013年5月 pattern (.*?)年(.*?)月 template： $1-$2 return 2013-5 |
| `cn.hutool.core.util.ReUtil` | `String extractMultiAndDelPre(Pattern pattern,Mutable<CharSequence> contentHolder,String template)` | 从content中匹配出多个值并根据template生成新的字符串 匹配结束后会删除匹配内容之前的内容（包括匹配内容） 例如： content 2013年5月 pattern (.*?)年(.*?)月 template： $1-$2 return 2013-5 |
| `cn.hutool.core.util.ReUtil` | `String extractMultiAndDelPre(String regex,Mutable<CharSequence> contentHolder,String template)` | 从content中匹配出多个值并根据template生成新的字符串 例如： content 2013年5月 pattern (.*?)年(.*?)月 template： $1-$2 return 2013-5 |
| `cn.hutool.core.util.ReUtil` | `String get(Pattern pattern,CharSequence content,String groupName)` | 获得匹配的字符串 |
| `cn.hutool.core.util.ReUtil` | `String get(Pattern pattern,CharSequence content,int groupIndex)` | 获得匹配的字符串，对应分组0表示整个匹配内容，1表示第一个括号分组内容，依次类推 |
| `cn.hutool.core.util.ReUtil` | `String get(String regex,CharSequence content,String groupName)` | 获得匹配的字符串 |
| `cn.hutool.core.util.ReUtil` | `String get(String regex,CharSequence content,int groupIndex)` | 获得匹配的字符串 |
| `cn.hutool.core.util.ReUtil` | `String getGroup0(Pattern pattern,CharSequence content)` | 获得匹配的字符串，获得正则中分组0的内容 |
| `cn.hutool.core.util.ReUtil` | `String getGroup0(String regex,CharSequence content)` | 获得匹配的字符串，获得正则中分组0的内容 |
| `cn.hutool.core.util.ReUtil` | `String getGroup1(Pattern pattern,CharSequence content)` | 获得匹配的字符串，获得正则中分组1的内容 |
| `cn.hutool.core.util.ReUtil` | `String getGroup1(String regex,CharSequence content)` | 获得匹配的字符串，获得正则中分组1的内容 |
| `cn.hutool.core.util.ReUtil` | `String replaceAll(CharSequence content,Pattern pattern,String replacementTemplate)` | 正则替换指定值 通过正则查找到字符串，然后把匹配到的字符串加入到replacementTemplate中，$1表示分组1的字符串 |
| `cn.hutool.core.util.ReUtil` | `String replaceAll(CharSequence content,String regex,String replacementTemplate)` | 正则替换指定值 通过正则查找到字符串，然后把匹配到的字符串加入到replacementTemplate中，$1表示分组1的字符串 例如：原字符串是：中文1234，我想把1234换成(1234)，则可以： |
| `cn.hutool.core.util.ReUtil` | `String replaceAll(CharSequence str,Pattern pattern,Func1<Matcher, String> replaceFun)` | 替换所有正则匹配的文本，并使用自定义函数决定如何替换 replaceFun可以通过Matcher提取出匹配到的内容的不同部分，然后经过重新处理、组装变成新的内容放回原位。 |
| `cn.hutool.core.util.ReUtil` | `String replaceAll(CharSequence str,String regex,Func1<Matcher, String> replaceFun)` | 替换所有正则匹配的文本，并使用自定义函数决定如何替换 replaceFun可以通过Matcher提取出匹配到的内容的不同部分，然后经过重新处理、组装变成新的内容放回原位。 |
| `cn.hutool.core.util.ReUtil` | `String replaceFirst(Pattern pattern,CharSequence content,String replacement)` | 替换匹配的第一个内容 |
| `cn.hutool.core.util.ReUtil` | `T findAll(Pattern pattern,CharSequence content,int group,T collection)` | 取得内容中匹配的所有结果 |
| `cn.hutool.core.util.ReUtil` | `T findAll(String regex,CharSequence content,int group,T collection)` | 取得内容中匹配的所有结果 |
| `cn.hutool.core.util.ReUtil` | `boolean contains(Pattern pattern,CharSequence content)` | 指定内容中是否有表达式匹配的内容 |
| `cn.hutool.core.util.ReUtil` | `boolean contains(String regex,CharSequence content)` | 指定内容中是否有表达式匹配的内容 |
| `cn.hutool.core.util.ReUtil` | `boolean isMatch(Pattern pattern,CharSequence content)` | 给定内容是否匹配正则 |
| `cn.hutool.core.util.ReUtil` | `boolean isMatch(String regex,CharSequence content)` | 给定内容是否匹配正则 |
| `cn.hutool.core.util.ReUtil` | `int count(Pattern pattern,CharSequence content)` | 计算指定字符串中，匹配pattern的个数 |
| `cn.hutool.core.util.ReUtil` | `int count(String regex,CharSequence content)` | 计算指定字符串中，匹配pattern的个数 |
| `cn.hutool.core.util.ReUtil` | `void findAll(Pattern pattern,CharSequence content,Consumer<Matcher> consumer)` | 取得内容中匹配的所有结果，使用Consumer完成匹配结果处理 |
| `cn.hutool.core.util.ReUtil` | `void get(Pattern pattern,CharSequence content,Consumer<Matcher> consumer)` | 在给定字符串中查找给定规则的字符，如果找到则使用Consumer处理之 如果内容中有多个匹配项，则只处理找到的第一个结果。 |
| `cn.hutool.core.util.ReferenceUtil` | `Reference<T> create(ReferenceType type,T referent)` | 获得引用 |
| `cn.hutool.core.util.ReferenceUtil` | `Reference<T> create(ReferenceType type,T referent,ReferenceQueue<T> queue)` | 获得引用 |
| `cn.hutool.core.util.ReferenceUtil` | `T get(final Ref<T> obj)` | null安全的解包获取原始对象 |
| `cn.hutool.core.util.ReferenceUtil` | `T get(final Reference<T> obj)` | null全的解包获取原始对象 |
| `cn.hutool.core.util.ReflectUtil` | `Constructor<?>[] getConstructorsDirectly(Class<?> beanClass)` | 获得一个类中所有构造列表，直接反射获取，无缓存 |
| `cn.hutool.core.util.ReflectUtil` | `Constructor<T> getConstructor(Class<T> clazz,Class<?>... parameterTypes)` | 查找类中的指定参数的构造方法，如果找到构造方法，会自动设置可访问为true |
| `cn.hutool.core.util.ReflectUtil` | `Constructor<T>[] getConstructors(Class<T> beanClass)` | 获得一个类中所有构造列表 |
| `cn.hutool.core.util.ReflectUtil` | `Field getField(Class<?> beanClass,String name)` | 查找指定类中的指定name的字段（包括非public字段），也包括父类和Object类的字段， 字段不存在则返回null |
| `cn.hutool.core.util.ReflectUtil` | `Field[] getFields(Class<?> beanClass)` | 获得一个类中所有字段列表，包括其父类中的字段 如果子类与父类中存在同名字段，则这两个字段同时存在，子类字段在前，父类字段在后。 |
| `cn.hutool.core.util.ReflectUtil` | `Field[] getFields(Class<?> beanClass,Filter<Field> fieldFilter)` | 获得一个类中所有满足条件的字段列表，包括其父类中的字段 如果子类与父类中存在同名字段，则这两个字段同时存在，子类字段在前，父类字段在后。 |
| `cn.hutool.core.util.ReflectUtil` | `Field[] getFieldsDirectly(Class<?> beanClass,boolean withSuperClassFields)` | 获得一个类中所有字段列表，直接反射获取，无缓存 如果子类与父类中存在同名字段，则这两个字段同时存在，子类字段在前，父类字段在后。 |
| `cn.hutool.core.util.ReflectUtil` | `List<Method> getPublicMethods(Class<?> clazz,Filter<Method> filter)` | 获得指定类过滤后的Public方法列表 TODO 6.x此方法更改返回Method[] |
| `cn.hutool.core.util.ReflectUtil` | `List<Method> getPublicMethods(Class<?> clazz,Method... excludeMethods)` | 获得指定类过滤后的Public方法列表 |
| `cn.hutool.core.util.ReflectUtil` | `List<Method> getPublicMethods(Class<?> clazz,String... excludeMethodNames)` | 获得指定类过滤后的Public方法列表 |
| `cn.hutool.core.util.ReflectUtil` | `Map<String, Field> getFieldMap(Class<?> beanClass)` | 获取指定类中字段名和字段对应的有序Map，包括其父类中的字段 如果子类与父类中存在同名字段，则后者覆盖前者。 |
| `cn.hutool.core.util.ReflectUtil` | `Method getMethod(Class<?> clazz,String methodName,Class<?>... paramTypes)` | 查找指定方法 如果找不到对应的方法则返回null 此方法为精准获取方法名，即方法名和参数数量和类型必须一致，否则返回null。 |
| `cn.hutool.core.util.ReflectUtil` | `Method getMethod(Class<?> clazz,boolean ignoreCase,String methodName,Class<?>... paramTypes)` | 查找指定方法 如果找不到对应的方法则返回null 此方法为精准获取方法名，即方法名和参数数量和类型必须一致，否则返回null。 如果查找的方法有多个同参数类型重载，查找第一个找到的方法 |
| `cn.hutool.core.util.ReflectUtil` | `Method getMethodByName(Class<?> clazz,String methodName)` | 按照方法名查找指定方法名的方法，只返回匹配到的第一个方法，如果找不到对应的方法则返回null 此方法只检查方法名是否一致，并不检查参数的一致性。 |
| `cn.hutool.core.util.ReflectUtil` | `Method getMethodByName(Class<?> clazz,boolean ignoreCase,String methodName)` | 按照方法名查找指定方法名的方法，只返回匹配到的第一个方法，如果找不到对应的方法则返回null 此方法只检查方法名是否一致，并不检查参数的一致性。 |
| `cn.hutool.core.util.ReflectUtil` | `Method getMethodByNameIgnoreCase(Class<?> clazz,String methodName)` | 按照方法名查找指定方法名的方法，只返回匹配到的第一个方法，如果找不到对应的方法则返回null 此方法只检查方法名是否一致（忽略大小写），并不检查参数的一致性。 |
| `cn.hutool.core.util.ReflectUtil` | `Method getMethodIgnoreCase(Class<?> clazz,String methodName,Class<?>... paramTypes)` | 忽略大小写查找指定方法，如果找不到对应的方法则返回null 此方法为精准获取方法名，即方法名和参数数量和类型必须一致，否则返回null。 |
| `cn.hutool.core.util.ReflectUtil` | `Method getMethodOfObj(Object obj,String methodName,Object... args)` | 查找指定对象中的所有方法（包括非public方法），也包括父对象和Object类的方法 此方法为精准获取方法名，即方法名和参数数量和类型必须一致，否则返回null。 |
| `cn.hutool.core.util.ReflectUtil` | `Method getPublicMethod(Class<?> clazz,String methodName,Class<?>... paramTypes)` | 查找指定Public方法 如果找不到对应的方法或方法不为public的则返回null |
| `cn.hutool.core.util.ReflectUtil` | `Method[] getMethods(Class<?> beanClass)` | 获得一个类中所有方法列表，包括其父类中的方法 |
| `cn.hutool.core.util.ReflectUtil` | `Method[] getMethods(Class<?> clazz,Filter<Method> filter)` | 获得指定类过滤后的方法列表 |
| `cn.hutool.core.util.ReflectUtil` | `Method[] getMethodsDirectly(Class<?> beanClass,boolean withSupers,boolean withMethodFromObject)` | 获得一个类中所有方法列表，直接反射获取，无缓存 接口获取方法和默认方法，获取的方法包括： 本类中的所有方法（包括static方法） 父类中的所有方法（包括static方法） Object中（包括static方法） |
| `cn.hutool.core.util.ReflectUtil` | `Method[] getPublicMethods(Class<?> clazz)` | 获得本类及其父类所有Public方法 |
| `cn.hutool.core.util.ReflectUtil` | `Object getFieldValue(Object obj,Field field)` | 获取字段值 |
| `cn.hutool.core.util.ReflectUtil` | `Object getFieldValue(Object obj,String fieldName)` | 获取字段值 |
| `cn.hutool.core.util.ReflectUtil` | `Object getStaticFieldValue(Field field)` | 获取静态字段值 |
| `cn.hutool.core.util.ReflectUtil` | `Object[] getFieldsValue(Object obj)` | 获取所有字段的值 |
| `cn.hutool.core.util.ReflectUtil` | `Object[] getFieldsValue(Object obj,Filter<Field> filter)` | 获取所有字段的值 |
| `cn.hutool.core.util.ReflectUtil` | `Set<String> getMethodNames(Class<?> clazz)` | 获得指定类中的方法名 去重重载的方法 |
| `cn.hutool.core.util.ReflectUtil` | `Set<String> getPublicMethodNames(Class<?> clazz)` | 获得指定类本类及其父类中的Public方法名 去重重载的方法 |
| `cn.hutool.core.util.ReflectUtil` | `String getFieldName(Field field)` | 获取字段名，如果存在Alias注解，读取注解的值作为名称 |
| `cn.hutool.core.util.ReflectUtil` | `T invoke(Object obj,Method method,Object... args)` | 执行方法 对于用户传入参数会做必要检查，包括： |
| `cn.hutool.core.util.ReflectUtil` | `T invoke(Object obj,String methodName,Object... args)` | 执行对象中指定方法 如果需要传递的参数为null,请使用NullWrapperBean来传递,不然会丢失类型信息 |
| `cn.hutool.core.util.ReflectUtil` | `T invokeRaw(Object obj,Method method,Object... args)` | 执行方法 对于用户传入参数会做必要检查，包括： |
| `cn.hutool.core.util.ReflectUtil` | `T invokeStatic(Method method,Object... args)` | 执行静态方法 |
| `cn.hutool.core.util.ReflectUtil` | `T invokeWithCheck(Object obj,Method method,Object... args)` | 执行方法 执行前要检查给定参数： |
| `cn.hutool.core.util.ReflectUtil` | `T newInstance(Class<T> clazz,Object... params)` | 实例化对象 |
| `cn.hutool.core.util.ReflectUtil` | `T newInstance(String clazz)` | 实例化对象 |
| `cn.hutool.core.util.ReflectUtil` | `T newInstanceIfPossible(Class<T> type)` | 尝试遍历并调用此类的所有构造方法，直到构造成功并返回 对于某些特殊的接口，按照其默认实现实例化，例如： |
| `cn.hutool.core.util.ReflectUtil` | `T setAccessible(T accessibleObject)` | 设置方法为可访问（私有方法可以被外部调用） |
| `cn.hutool.core.util.ReflectUtil` | `boolean hasField(Class<?> beanClass,String name)` | 查找指定类中是否包含指定名称对应的字段，包括所有字段（包括非public字段），也包括父类和Object类的字段 |
| `cn.hutool.core.util.ReflectUtil` | `boolean isEmptyParam(Method method)` | 是否为无参数方法 |
| `cn.hutool.core.util.ReflectUtil` | `boolean isEqualsMethod(Method method)` | 是否为equals方法 |
| `cn.hutool.core.util.ReflectUtil` | `boolean isGetterOrSetter(Method method,boolean ignoreCase)` | 检查给定方法是否为Getter或者Setter方法，规则为： 方法参数必须为0个或1个 方法名称不能是getClass 如果是无参方法，则判断是否以“get”或“is”开头 如果方法参数1个，则判断是否以“set”开头 |
| `cn.hutool.core.util.ReflectUtil` | `boolean isGetterOrSetterIgnoreCase(Method method)` | 检查给定方法是否为Getter或者Setter方法，规则为： 方法参数必须为0个或1个 如果是无参方法，则判断是否以“get”或“is”开头 如果方法参数1个，则判断是否以“set”开头 |
| `cn.hutool.core.util.ReflectUtil` | `boolean isHashCodeMethod(Method method)` | 是否为hashCode方法 |
| `cn.hutool.core.util.ReflectUtil` | `boolean isOuterClassField(Field field)` | 是否为父类引用字段 当字段所在类是对象子类时（对象中定义的非static的class），会自动生成一个以"this$0"为名称的字段，指向父类对象 |
| `cn.hutool.core.util.ReflectUtil` | `boolean isToStringMethod(Method method)` | 是否为toString方法 |
| `cn.hutool.core.util.ReflectUtil` | `void removeFinalModify(Field field)` | 设置final的field字段可以被修改 只要不会被编译器内联优化的 final 属性就可以通过反射有效的进行修改 -- 修改后代码中可使用到新的值; 以下属性，编译器会内联优化，无法通过反射修改： 基本类型 byte, char, short, int, long, float, double, boolean Literal String 类型(直接双引号字符串) 以下属性，可以通过反射修改： 基本类型的包装类 Byte、Character、Short、Long、Float、Double、Boolean 字符串，通过 new String("")实例化 自定义java类 |
| `cn.hutool.core.util.ReflectUtil` | `void setFieldValue(Object obj,Field field,Object value)` | 设置字段值 若值类型与字段类型不一致，则会尝试通过 Convert 进行转换 若字段类型是原始类型而传入的值是 null，则会将字段设置为对应原始类型的默认值（见 ClassUtil#getDefaultValue(Class)） 如果是final字段，setFieldValue，调用这可以先调用 ReflectUtil#removeFinalModify(Field)方法去除final修饰符 |
| `cn.hutool.core.util.ReflectUtil` | `void setFieldValue(Object obj,String fieldName,Object value)` | 设置字段值 若值类型与字段类型不一致，则会尝试通过 Convert 进行转换 若字段类型是原始类型而传入的值是 null，则会将字段设置为对应原始类型的默认值（见 ClassUtil#getDefaultValue(Class)） 如果是final字段，setFieldValue，调用这可以先调用 ReflectUtil#removeFinalModify(Field)方法去除final修饰符 |
| `cn.hutool.core.util.RuntimeUtil` | `List<String> execForLines(Charset charset,String... cmds)` | 执行系统命令，使用传入的 Charset charset 编码 |
| `cn.hutool.core.util.RuntimeUtil` | `List<String> execForLines(String... cmds)` | 执行系统命令，使用系统默认编码 |
| `cn.hutool.core.util.RuntimeUtil` | `List<String> getResultLines(Process process)` | 获取命令执行结果，使用系统默认编码，获取后销毁进程 |
| `cn.hutool.core.util.RuntimeUtil` | `List<String> getResultLines(Process process,Charset charset)` | 获取命令执行结果，使用传入的 Charset charset 编码，获取后销毁进程 |
| `cn.hutool.core.util.RuntimeUtil` | `Process exec(String... cmds)` | 执行命令 命令带参数时参数可作为其中一个参数，也可以将命令和参数组合为一个字符串传入 |
| `cn.hutool.core.util.RuntimeUtil` | `Process exec(String[] envp,File dir,String... cmds)` | 执行命令 命令带参数时参数可作为其中一个参数，也可以将命令和参数组合为一个字符串传入 |
| `cn.hutool.core.util.RuntimeUtil` | `Process exec(String[] envp,String... cmds)` | 执行命令 命令带参数时参数可作为其中一个参数，也可以将命令和参数组合为一个字符串传入 |
| `cn.hutool.core.util.RuntimeUtil` | `String execForStr(Charset charset,String... cmds)` | 执行系统命令，使用传入的 Charset charset 编码 |
| `cn.hutool.core.util.RuntimeUtil` | `String execForStr(String... cmds)` | 执行系统命令，使用系统默认编码 |
| `cn.hutool.core.util.RuntimeUtil` | `String getErrorResult(Process process)` | 获取命令执行异常结果，使用系统默认编码，获取后销毁进程 |
| `cn.hutool.core.util.RuntimeUtil` | `String getErrorResult(Process process,Charset charset)` | 获取命令执行异常结果，获取后销毁进程 |
| `cn.hutool.core.util.RuntimeUtil` | `String getResult(Process process)` | 获取命令执行结果，使用系统默认编码，获取后销毁进程 |
| `cn.hutool.core.util.RuntimeUtil` | `String getResult(Process process,Charset charset)` | 获取命令执行结果，获取后销毁进程 |
| `cn.hutool.core.util.RuntimeUtil` | `int getPid()` | 获取当前进程ID，首先获取进程名称，读取@前的ID值，如果不存在，则读取进程名的hash值 |
| `cn.hutool.core.util.RuntimeUtil` | `int getProcessorCount()` | 获得JVM可用的处理器数量（一般为CPU核心数） 这里做一个特殊的处理,在特殊的CPU上面，会有获取不到CPU数量的情况，所以这里做一个保护; 默认给一个7，真实的CPU基本都是偶数，方便区分。 如果不做处理，会出现创建线程池时ThreadPoolExecutor，抛出异常：IllegalArgumentException |
| `cn.hutool.core.util.RuntimeUtil` | `long getFreeMemory()` | 获得JVM中剩余的内存数，单位byte |
| `cn.hutool.core.util.RuntimeUtil` | `long getMaxMemory()` | 获得JVM中可以从系统中获取的最大的内存数，单位byte，以-Xmx参数为准 |
| `cn.hutool.core.util.RuntimeUtil` | `long getTotalMemory()` | 获得JVM已经从系统中获取到的总共的内存数，单位byte |
| `cn.hutool.core.util.RuntimeUtil` | `long getUsableMemory()` | 获得JVM最大可用内存，计算方法为： 最大内存-总内存+剩余内存 |
| `cn.hutool.core.util.RuntimeUtil` | `void addShutdownHook(Runnable hook)` | 增加一个JVM关闭后的钩子，用于在JVM关闭时执行某些操作 |
| `cn.hutool.core.util.RuntimeUtil` | `void destroy(Process process)` | 销毁进程 |
| `cn.hutool.core.util.SerializeUtil` | `T clone(T obj)` | 序列化后拷贝流的方式克隆 对象必须实现Serializable接口 |
| `cn.hutool.core.util.SerializeUtil` | `T deserialize(byte[] bytes,Class<?>... acceptClasses)` | 反序列化 对象必须实现Serializable接口 注意！！！ 此方法不会检查反序列化安全，可能存在反序列化漏洞风险！！！ |
| `cn.hutool.core.util.SerializeUtil` | `byte[] serialize(T obj)` | 序列化 对象必须实现Serializable接口 |
| `cn.hutool.core.util.ServiceLoaderUtil` | `List<T> loadList(Class<T> clazz)` | 加载服务 并已list列表返回 |
| `cn.hutool.core.util.ServiceLoaderUtil` | `List<T> loadList(Class<T> clazz,ClassLoader loader)` | 加载服务 并已list列表返回 |
| `cn.hutool.core.util.ServiceLoaderUtil` | `ServiceLoader<T> load(Class<T> clazz)` | 加载服务 |
| `cn.hutool.core.util.ServiceLoaderUtil` | `ServiceLoader<T> load(Class<T> clazz,ClassLoader loader)` | 加载服务 |
| `cn.hutool.core.util.ServiceLoaderUtil` | `T loadFirst(Class<T> clazz)` | 加载第一个服务，如果用户定义了多个接口实现类，只获取第一个。 |
| `cn.hutool.core.util.ServiceLoaderUtil` | `T loadFirstAvailable(Class<T> clazz)` | 加载第一个可用的 Service 实现。 为兼容 JDK 24+ 中 ServiceLoader 在加载服务实现时可能抛出的 NoClassDefFoundError， 此方法在调用 hasNext() 和 next() 时安全忽略异常。 当遇到依赖缺失或配置错误的实现时会自动跳过，并返回第一个可用的非空实例。 |
| `cn.hutool.core.util.StrUtil` | `StrBuilder strBuilder()` | 创建StrBuilder对象 |
| `cn.hutool.core.util.StrUtil` | `StrBuilder strBuilder(int capacity)` | 创建StrBuilder对象 |
| `cn.hutool.core.util.StrUtil` | `String fill(String str,char filledChar,int len,boolean isPre)` | 将已有字符串填充为规定长度，如果已有字符串超过这个长度则返回这个字符串 |
| `cn.hutool.core.util.StrUtil` | `String fillAfter(String str,char filledChar,int len)` | 将已有字符串填充为规定长度，如果已有字符串超过这个长度则返回这个字符串 字符填充于字符串后 |
| `cn.hutool.core.util.StrUtil` | `String fillBefore(String str,char filledChar,int len)` | 将已有字符串填充为规定长度，如果已有字符串超过这个长度则返回这个字符串 字符填充于字符串前 |
| `cn.hutool.core.util.StrUtil` | `String format(CharSequence template,Map<?, ?> map)` | 格式化文本，使用 {varName} 占位 map = {a: "aValue", b: "bValue"} format("{a} and {b}", map) ---=》 aValue and bValue |
| `cn.hutool.core.util.StrUtil` | `String format(CharSequence template,Map<?, ?> map,boolean ignoreNull)` | 格式化文本，使用 {varName} 占位 map = {a: "aValue", b: "bValue"} format("{a} and {b}", map) ---=》 aValue and bValue |
| `cn.hutool.core.util.StrUtil` | `String reverse(final String str)` | 反转字符串 例如：abcd =》dcba |
| `cn.hutool.core.util.StrUtil` | `String reverseByCodePoint(String str)` | 反转字符串 例如：abcd =》dcba 该方法按Unicode code point进行反转，支持Unicode字符的正确反转 确保复杂字符不会被拆分，如表情符号等多字节字符 |
| `cn.hutool.core.util.StrUtil` | `String similar(String str1,String str2,int scale)` | 计算两个字符串的相似度百分比 |
| `cn.hutool.core.util.StrUtil` | `String str(ByteBuffer data,Charset charset)` | 将编码的byteBuffer数据转换为字符串 |
| `cn.hutool.core.util.StrUtil` | `String str(ByteBuffer data,String charset)` | 将编码的byteBuffer数据转换为字符串 |
| `cn.hutool.core.util.StrUtil` | `String str(Byte[] bytes,String charset)` | 将Byte数组转为字符串 |
| `cn.hutool.core.util.StrUtil` | `String str(Byte[] data,Charset charset)` | 解码字节码 |
| `cn.hutool.core.util.StrUtil` | `String str(Object obj,Charset charset)` | 将对象转为字符串 |
| `cn.hutool.core.util.StrUtil` | `String str(Object obj,String charsetName)` | 将对象转为字符串 |
| `cn.hutool.core.util.StrUtil` | `String str(byte[] bytes,String charset)` | 将byte数组转为字符串 |
| `cn.hutool.core.util.StrUtil` | `String str(byte[] data,Charset charset)` | 解码字节码 |
| `cn.hutool.core.util.StrUtil` | `String toString(Object obj)` | 调用对象的toString方法，null会返回“null” |
| `cn.hutool.core.util.StrUtil` | `String toStringOrEmpty(Object obj)` | 调用对象的toString方法，null会返回空字符串 "" |
| `cn.hutool.core.util.StrUtil` | `String toStringOrNull(Object obj)` | 调用对象的toString方法，null会返回null |
| `cn.hutool.core.util.StrUtil` | `String truncateByByteLength(String str,Charset charset,int maxBytesLength,int factor,boolean appendDots)` | 截断字符串，使用其按照指定编码为字节后不超过maxBytes长度 此方法用于截取总bytes数不超过指定长度，如果字符出没有超出原样输出，如果超出了，则截取掉超出部分，并可选添加...， 但是添加“...”后总长度也不超过限制长度。 |
| `cn.hutool.core.util.StrUtil` | `String truncateUtf8(String str,int maxBytes)` | 截断字符串，使用其按照UTF-8编码为字节后不超过maxBytes长度。截断后自动追加省略号(...) 用于存储数据库varchar且编码为UTF-8的字段 |
| `cn.hutool.core.util.StrUtil` | `String utf8Str(Object obj)` | 将对象转为字符串 |
| `cn.hutool.core.util.StrUtil` | `String uuid()` | 生成随机UUID |
| `cn.hutool.core.util.StrUtil` | `StringBuilder builder()` | 创建StringBuilder对象 |
| `cn.hutool.core.util.StrUtil` | `StringBuilder builder(int capacity)` | 创建StringBuilder对象 |
| `cn.hutool.core.util.StrUtil` | `StringReader getReader(CharSequence str)` | 获得StringReader |
| `cn.hutool.core.util.StrUtil` | `StringWriter getWriter()` | 获得StringWriter |
| `cn.hutool.core.util.StrUtil` | `boolean isBlankIfStr(Object obj)` | 如果对象是字符串是否为空白，空白的定义如下： null 空字符串："" 空格、全角空格、制表符、换行符，等不可见字符 例： StrUtil.isBlankIfStr(null) // true StrUtil.isBlankIfStr("") // true StrUtil.isBlankIfStr(" \t\n") // true StrUtil.isBlankIfStr("abc") // false 注意：该方法与 #isEmptyIfStr(Object) 的区别是： 该方法会校验空白字符，且性能相对于 #isEmptyIfStr(Object) 略慢。 |
| `cn.hutool.core.util.StrUtil` | `boolean isEmptyIfStr(Object obj)` | 如果对象是字符串是否为空串，空的定义如下： null 空字符串："" 例： StrUtil.isEmptyIfStr(null) // true StrUtil.isEmptyIfStr("") // true StrUtil.isEmptyIfStr(" \t\n") // false StrUtil.isEmptyIfStr("abc") // false 注意：该方法与 #isBlankIfStr(Object) 的区别是：该方法不校验空白字符。 |
| `cn.hutool.core.util.StrUtil` | `double similar(String str1,String str2)` | 计算两个字符串的相似度 |
| `cn.hutool.core.util.StrUtil` | `void trim(String[] strs)` | 给定字符串数组全部做去首尾空格 |
| `cn.hutool.core.util.SystemPropsUtil` | `Properties getProps()` | @return 属性列表 |
| `cn.hutool.core.util.SystemPropsUtil` | `String get(String key)` | 获得System属性 |
| `cn.hutool.core.util.SystemPropsUtil` | `String get(String name,String defaultValue)` | 取得系统属性，如果因为Java安全的限制而失败，则将错误打在Log中，然后返回 defaultValue |
| `cn.hutool.core.util.SystemPropsUtil` | `String get(String name,boolean quiet)` | 取得系统属性，如果因为Java安全的限制而失败，则将错误打在Log中，然后返回 null |
| `cn.hutool.core.util.SystemPropsUtil` | `boolean getBoolean(String key,boolean defaultValue)` | 获得boolean类型值 |
| `cn.hutool.core.util.SystemPropsUtil` | `int getInt(String key,int defaultValue)` | 获得int类型值 |
| `cn.hutool.core.util.SystemPropsUtil` | `long getLong(String key,long defaultValue)` | 获得long类型值 |
| `cn.hutool.core.util.SystemPropsUtil` | `void set(String key,String value)` | 设置系统属性，value为null表示移除此属性 |
| `cn.hutool.core.util.TypeUtil` | `Class<?> getClass(Field field)` | 获得Field对应的原始类 |
| `cn.hutool.core.util.TypeUtil` | `Class<?> getClass(Type type)` | 获得Type对应的原始类 |
| `cn.hutool.core.util.TypeUtil` | `Class<?> getFirstParamClass(Method method)` | 获取方法的第一个参数类 |
| `cn.hutool.core.util.TypeUtil` | `Class<?> getParamClass(Method method,int index)` | 获取方法的参数类 |
| `cn.hutool.core.util.TypeUtil` | `Class<?> getReturnClass(Method method)` | 解析方法的返回类型类列表 |
| `cn.hutool.core.util.TypeUtil` | `Class<?>[] getParamClasses(Method method)` | 解析方法的参数类型列表 依赖jre\lib\rt.jar |
| `cn.hutool.core.util.TypeUtil` | `Map<Type, Type> getTypeMap(Class<?> clazz)` | 获取泛型变量和泛型实际类型的对应关系Map，例如： |
| `cn.hutool.core.util.TypeUtil` | `ParameterizedType toParameterizedType(final Type type)` | 将Type 转换为ParameterizedType ParameterizedType用于获取当前类或父类中泛型参数化后的类型 一般用于获取泛型参数具体的参数类型，例如： |
| `cn.hutool.core.util.TypeUtil` | `ParameterizedType toParameterizedType(final Type type,final int interfaceIndex)` | 将Type 转换为ParameterizedType ParameterizedType用于获取当前类或父类中泛型参数化后的类型 一般用于获取泛型参数具体的参数类型，例如： |
| `cn.hutool.core.util.TypeUtil` | `ParameterizedType[] getGenerics(final Class<?> clazz)` | 获取指定类所有泛型父类和泛型接口 |
| `cn.hutool.core.util.TypeUtil` | `Type getActualType(Type type,Field field)` | 获得泛型字段对应的泛型实际类型，如果此变量没有对应的实际类型，返回null |
| `cn.hutool.core.util.TypeUtil` | `Type getActualType(Type type,ParameterizedType parameterizedType)` | 获得泛型变量对应的泛型实际类型，如果此变量没有对应的实际类型，返回null 此方法可以处理复杂的泛型化对象，类似于Map<User, Key<Long>> |
| `cn.hutool.core.util.TypeUtil` | `Type getActualType(Type type,Type typeVariable)` | 获得泛型变量对应的泛型实际类型，如果此变量没有对应的实际类型，返回null 此方法可以处理： |
| `cn.hutool.core.util.TypeUtil` | `Type getFieldType(Class<?> clazz,String fieldName)` | 获得字段的泛型类型 |
| `cn.hutool.core.util.TypeUtil` | `Type getFirstParamType(Method method)` | 获取方法的第一个参数类型 优先获取方法的GenericParameterTypes，如果获取不到，则获取ParameterTypes |
| `cn.hutool.core.util.TypeUtil` | `Type getParamType(Method method,int index)` | 获取方法的参数类型 优先获取方法的GenericParameterTypes，如果获取不到，则获取ParameterTypes |
| `cn.hutool.core.util.TypeUtil` | `Type getReturnType(Method method)` | 获取方法的返回值类型 获取方法的GenericReturnType |
| `cn.hutool.core.util.TypeUtil` | `Type getType(Field field)` | 获取字段对应的Type类型 方法优先获取GenericType，获取不到则获取Type |
| `cn.hutool.core.util.TypeUtil` | `Type getTypeArgument(Type type)` | 获得给定类的第一个泛型参数 |
| `cn.hutool.core.util.TypeUtil` | `Type getTypeArgument(Type type,int index)` | 获得给定类的泛型参数 |
| `cn.hutool.core.util.TypeUtil` | `Type[] getActualTypes(Type type,Type... typeVariables)` | 获得泛型变量对应的泛型实际类型，如果此变量没有对应的实际类型，返回null |
| `cn.hutool.core.util.TypeUtil` | `Type[] getParamTypes(Method method)` | 获取方法的参数类型列表 优先获取方法的GenericParameterTypes，如果获取不到，则获取ParameterTypes |
| `cn.hutool.core.util.TypeUtil` | `Type[] getTypeArguments(Type type)` | 获得指定类型中所有泛型参数类型，例如： |
| `cn.hutool.core.util.TypeUtil` | `boolean hasTypeVariable(Type... types)` | 指定泛型数组中是否含有泛型变量 |
| `cn.hutool.core.util.TypeUtil` | `boolean isUnknown(Type type)` | 是否未知类型 type为null或者TypeVariable 都视为未知类型 |
| `cn.hutool.core.util.URLUtil` | `BufferedReader getReader(URL url,Charset charset)` | 获得Reader |
| `cn.hutool.core.util.URLUtil` | `InputStream getStream(URL url)` | 从URL中获取流 |
| `cn.hutool.core.util.URLUtil` | `JarFile getJarFile(URL url)` | 从URL中获取JarFile |
| `cn.hutool.core.util.URLUtil` | `String buildQuery(Map<String, ?> paramMap,Charset charset)` | 将Map形式的Form表单数据转换为Url参数形式 paramMap中如果key为空（null和""）会被忽略，如果value为null，会被做为空白符（""） 会自动url编码键和值 |
| `cn.hutool.core.util.URLUtil` | `String completeUrl(String baseUrl,String relativePath)` | 补全相对路径 |
| `cn.hutool.core.util.URLUtil` | `String decode(String content,Charset charset)` | 解码application/x-www-form-urlencoded字符 将%开头的16进制表示的内容解码。 规则见：https://url.spec.whatwg.org/#urlencoded-parsing |
| `cn.hutool.core.util.URLUtil` | `String decode(String content,Charset charset,boolean isPlusToSpace)` | 解码application/x-www-form-urlencoded字符 将%开头的16进制表示的内容解码。 |
| `cn.hutool.core.util.URLUtil` | `String decode(String content,String charset)` | 解码application/x-www-form-urlencoded字符 将%开头的16进制表示的内容解码。 |
| `cn.hutool.core.util.URLUtil` | `String decode(String url)` | 解码URL 将%开头的16进制表示的内容解码。 |
| `cn.hutool.core.util.URLUtil` | `String encodeBlank(CharSequence urlStr)` | 单独编码URL中的空白符，空白符编码为%20 |
| `cn.hutool.core.util.URLUtil` | `String getDataUri(String mimeType,Charset charset,String encoding,String data)` | Data URI Scheme封装。data URI scheme 允许我们使用内联（inline-code）的方式在网页中包含数据， 目的是将一些小的数据，直接嵌入到网页中，从而不用再从外部文件载入。常用于将图片嵌入网页。 Data URI的格式规范： |
| `cn.hutool.core.util.URLUtil` | `String getDataUri(String mimeType,String encoding,String data)` | Data URI Scheme封装。data URI scheme 允许我们使用内联（inline-code）的方式在网页中包含数据， 目的是将一些小的数据，直接嵌入到网页中，从而不用再从外部文件载入。常用于将图片嵌入网页。 Data URI的格式规范： |
| `cn.hutool.core.util.URLUtil` | `String getDataUriBase64(String mimeType,String data)` | Data URI Scheme封装，数据格式为Base64。data URI scheme 允许我们使用内联（inline-code）的方式在网页中包含数据， 目的是将一些小的数据，直接嵌入到网页中，从而不用再从外部文件载入。常用于将图片嵌入网页。 Data URI的格式规范： |
| `cn.hutool.core.util.URLUtil` | `String getDecodedPath(URL url)` | 从URL对象中获取不被编码的路径Path 对于本地路径，URL对象的getPath方法对于包含中文或空格时会被编码，导致本读路径读取错误。 此方法将URL转为URI后获取路径用于解决路径被编码的问题 |
| `cn.hutool.core.util.URLUtil` | `String getPath(String uriStr)` | 获得path部分 |
| `cn.hutool.core.util.URLUtil` | `String normalize(String url)` | 标准化URL字符串，包括： 自动补齐“http://”头 去除开头的\或者/ 替换\为/ |
| `cn.hutool.core.util.URLUtil` | `String normalize(String url,boolean isEncodePath)` | 标准化URL字符串，包括： 自动补齐“http://”头 去除开头的\或者/ 替换\为/ |
| `cn.hutool.core.util.URLUtil` | `String normalize(String url,boolean isEncodePath,boolean replaceSlash)` | 标准化URL字符串，包括： 自动补齐“http://”头 去除开头的\或者/ 替换\为/ 如果replaceSlash为true，则替换多个/为一个 |
| `cn.hutool.core.util.URLUtil` | `URI getHost(URL url)` | 获取URL中域名部分，只保留URL中的协议（Protocol）、Host，其它为null。 |
| `cn.hutool.core.util.URLUtil` | `URI getStringURI(CharSequence content)` | 获取string协议的URL，类似于string:///xxxxx |
| `cn.hutool.core.util.URLUtil` | `URI toURI(String location)` | 转字符串为URI |
| `cn.hutool.core.util.URLUtil` | `URI toURI(String location,boolean isEncode)` | 转字符串为URI |
| `cn.hutool.core.util.URLUtil` | `URI toURI(URL url)` | 转URL为URI |
| `cn.hutool.core.util.URLUtil` | `URI toURI(URL url,boolean isEncode)` | 转URL为URI |
| `cn.hutool.core.util.URLUtil` | `URL getURL(File file)` | 获得URL，常用于使用绝对路径时的情况 |
| `cn.hutool.core.util.URLUtil` | `URL getURL(String path,Class<?> clazz)` | 获得URL |
| `cn.hutool.core.util.URLUtil` | `URL getURL(String pathBaseClassLoader)` | 获得URL |
| `cn.hutool.core.util.URLUtil` | `URL toUrlForHttp(String urlStr)` | 将URL字符串转换为URL对象，并做必要验证 |
| `cn.hutool.core.util.URLUtil` | `URL toUrlForHttp(String urlStr,URLStreamHandler handler)` | 将URL字符串转换为URL对象，并做必要验证 |
| `cn.hutool.core.util.URLUtil` | `URL url(String url)` | 通过一个字符串形式的URL地址创建URL对象 |
| `cn.hutool.core.util.URLUtil` | `URL url(String url,URLStreamHandler handler)` | 通过一个字符串形式的URL地址创建URL对象 |
| `cn.hutool.core.util.URLUtil` | `URL url(URI uri)` | 将URI转换为URL |
| `cn.hutool.core.util.URLUtil` | `URL[] getURLs(File... files)` | 获得URL，常用于使用绝对路径时的情况 |
| `cn.hutool.core.util.URLUtil` | `boolean isFileURL(URL url)` | 提供的URL是否为文件 文件协议包括"file", "vfsfile" 或 "vfs". |
| `cn.hutool.core.util.URLUtil` | `boolean isJarFileURL(URL url)` | 提供的URL是否为Jar文件URL 判断依据为file协议且扩展名为.jar |
| `cn.hutool.core.util.URLUtil` | `boolean isJarURL(URL url)` | 提供的URL是否为jar包URL 协议包括： "jar", "zip", "vfszip" 或 "wsjar". |
| `cn.hutool.core.util.URLUtil` | `long getContentLength(URL url)` | 获取指定URL对应资源的内容长度，对于Http，其长度使用Content-Length头决定。 |
| `cn.hutool.core.util.URLUtil` | `long size(final URL url)` | 获取URL对应数据长度 如果URL为文件，转换为文件获取文件长度。 其它情况获取URLConnection#getContentLengthLong() |
| `cn.hutool.core.util.URLUtil` | `void useCachesIfNecessary(final URLConnection con)` | 如果连接为JNLP方式，则打开缓存 |
| `cn.hutool.core.util.VersionUtil` | `boolean anyMatch(String currentVersion,Collection<String> compareVersions)` | 是否匹配任意一个版本 |
| `cn.hutool.core.util.VersionUtil` | `boolean anyMatch(String currentVersion,String... compareVersions)` | 是否匹配任意一个版本 |
| `cn.hutool.core.util.VersionUtil` | `boolean isGreaterThan(String currentVersion,String compareVersion)` | 当前版本大于待比较版本 |
| `cn.hutool.core.util.VersionUtil` | `boolean isGreaterThanOrEqual(String currentVersion,String compareVersion)` | 当前版本大于等于待比较版本 |
| `cn.hutool.core.util.VersionUtil` | `boolean isLessThan(String currentVersion,String compareVersion)` | 当前版本小于待比较版本 |
| `cn.hutool.core.util.VersionUtil` | `boolean isLessThanOrEqual(String currentVersion,String compareVersion)` | 当前版本小于等于待比较版本 |
| `cn.hutool.core.util.VersionUtil` | `boolean matchEl(String currentVersion,String versionEl)` | 当前版本是否满足版本表达式 |
| `cn.hutool.core.util.VersionUtil` | `boolean matchEl(String currentVersion,String versionEl,String versionsDelimiter)` | 当前版本是否满足版本表达式 |
| `cn.hutool.core.util.XmlUtil` | `Document beanToXml(Object bean)` | 将Bean转换为XML |
| `cn.hutool.core.util.XmlUtil` | `Document beanToXml(Object bean,String namespace)` | 将Bean转换为XML |
| `cn.hutool.core.util.XmlUtil` | `Document beanToXml(Object bean,String namespace,boolean ignoreNull)` | 将Bean转换为XML |
| `cn.hutool.core.util.XmlUtil` | `Document createXml()` | 创建XML文档 创建的XML默认是utf8编码，修改编码的过程是在toStr和toFile方法里，即XML在转为文本的时候才定义编码 |
| `cn.hutool.core.util.XmlUtil` | `Document createXml(String rootElementName)` | 创建XML文档 创建的XML默认是utf8编码，修改编码的过程是在toStr和toFile方法里，即XML在转为文本的时候才定义编码 |
| `cn.hutool.core.util.XmlUtil` | `Document createXml(String rootElementName,String namespace)` | 创建XML文档 创建的XML默认是utf8编码，修改编码的过程是在toStr和toFile方法里，即XML在转为文本的时候才定义编码 |
| `cn.hutool.core.util.XmlUtil` | `Document getOwnerDocument(Node node)` | 获取节点所在的Document |
| `cn.hutool.core.util.XmlUtil` | `Document mapToXml(Map<?, ?> data,String rootName)` | 将Map转换为XML |
| `cn.hutool.core.util.XmlUtil` | `Document mapToXml(Map<?, ?> data,String rootName,String namespace)` | 将Map转换为XML |
| `cn.hutool.core.util.XmlUtil` | `Document parseXml(String xmlStr)` | 将String类型的XML转换为XML文档 |
| `cn.hutool.core.util.XmlUtil` | `Document readXML(File file)` | 读取解析XML文件 |
| `cn.hutool.core.util.XmlUtil` | `Document readXML(InputSource source)` | 读取解析XML文件 编码在XML中定义 |
| `cn.hutool.core.util.XmlUtil` | `Document readXML(InputStream inputStream)` | 读取解析XML文件 编码在XML中定义 |
| `cn.hutool.core.util.XmlUtil` | `Document readXML(Reader reader)` | 读取解析XML文件 |
| `cn.hutool.core.util.XmlUtil` | `Document readXML(String pathOrContent)` | 读取解析XML文件 如果给定内容以“<”开头，表示这是一个XML内容，直接读取，否则按照路径处理 路径可以为相对路径，也可以是绝对路径，相对路径相对于ClassPath |
| `cn.hutool.core.util.XmlUtil` | `DocumentBuilder createDocumentBuilder()` | 创建 DocumentBuilder |
| `cn.hutool.core.util.XmlUtil` | `DocumentBuilderFactory createDocumentBuilderFactory()` | 创建DocumentBuilderFactory 默认使用"com.sun.org.apache.xerces.internal.jaxp.DocumentBuilderFactoryImpl" 如果使用第三方实现，请调用#disableDefaultDocumentBuilderFactory() |
| `cn.hutool.core.util.XmlUtil` | `Element appendChild(Node node,String tagName)` | 在已有节点上创建子节点 |
| `cn.hutool.core.util.XmlUtil` | `Element appendChild(Node node,String tagName,String namespace)` | 在已有节点上创建子节点 |
| `cn.hutool.core.util.XmlUtil` | `Element getElement(Element element,String tagName)` | 根据节点名获得第一个子节点 |
| `cn.hutool.core.util.XmlUtil` | `Element getElementByXPath(String expression,Object source)` | 通过XPath方式读取XML节点等信息 Xpath相关文章：https://www.ibm.com/developerworks/cn/xml/x-javaxpathapi.html |
| `cn.hutool.core.util.XmlUtil` | `Element getRootElement(Document doc)` | 获得XML文档根节点 |
| `cn.hutool.core.util.XmlUtil` | `List<Element> getElements(Element element,String tagName)` | 根据节点名获得子节点列表 |
| `cn.hutool.core.util.XmlUtil` | `List<Element> transElements(Element parentEle,NodeList nodeList)` | 将NodeList转换为Element列表 非Element节点将被忽略 |
| `cn.hutool.core.util.XmlUtil` | `List<Element> transElements(NodeList nodeList)` | 将NodeList转换为Element列表 |
| `cn.hutool.core.util.XmlUtil` | `Map<String, Object> xmlToMap(Node node)` | XML格式字符串转换为Map |
| `cn.hutool.core.util.XmlUtil` | `Map<String, Object> xmlToMap(Node node,Map<String, Object> result)` | XML节点转换为Map |
| `cn.hutool.core.util.XmlUtil` | `Map<String, Object> xmlToMap(String xmlStr)` | XML格式字符串转换为Map |
| `cn.hutool.core.util.XmlUtil` | `Map<String, Object> xmlToMap(String xmlStr,Map<String, Object> result)` | XML格式字符串转换为Map 只支持第一级别的XML，不支持多级XML |
| `cn.hutool.core.util.XmlUtil` | `Node appendText(Node node,CharSequence text)` | 创建文本子节点 |
| `cn.hutool.core.util.XmlUtil` | `Node getNodeByXPath(String expression,Object source)` | 通过XPath方式读取XML节点等信息 Xpath相关文章：https://www.ibm.com/developerworks/cn/xml/x-javaxpathapi.html |
| `cn.hutool.core.util.XmlUtil` | `NodeList getNodeListByXPath(String expression,Object source)` | 通过XPath方式读取XML的NodeList Xpath相关文章：https://www.ibm.com/developerworks/cn/xml/x-javaxpathapi.html |
| `cn.hutool.core.util.XmlUtil` | `Object getByXPath(String expression,Object source,QName returnType)` | 通过XPath方式读取XML节点等信息 Xpath相关文章：https://www.ibm.com/developerworks/cn/xml/x-javaxpathapi.html |
| `cn.hutool.core.util.XmlUtil` | `Object getByXPath(String expression,Object source,QName returnType,NamespaceContext nsContext)` | 通过XPath方式读取XML节点等信息 Xpath相关文章： https://www.ibm.com/developerworks/cn/xml/x-javaxpathapi.html https://www.ibm.com/developerworks/cn/xml/x-nmspccontext/ |
| `cn.hutool.core.util.XmlUtil` | `String cleanComment(String xmlContent)` | 去除XML文本中的注释内容 |
| `cn.hutool.core.util.XmlUtil` | `String cleanInvalid(String xmlContent)` | 去除XML文本中的无效字符 |
| `cn.hutool.core.util.XmlUtil` | `String elementText(Element element,String tagName)` | 根据节点名获得第一个子节点 |
| `cn.hutool.core.util.XmlUtil` | `String elementText(Element element,String tagName,String defaultValue)` | 根据节点名获得第一个子节点 |
| `cn.hutool.core.util.XmlUtil` | `String escape(String string)` | 转义XML特殊字符: |
| `cn.hutool.core.util.XmlUtil` | `String format(Document doc)` | 格式化XML输出 |
| `cn.hutool.core.util.XmlUtil` | `String format(String xmlStr)` | 格式化XML输出 |
| `cn.hutool.core.util.XmlUtil` | `String mapToXmlStr(Map<?, ?> data)` | 将Map转换为XML格式的字符串 |
| `cn.hutool.core.util.XmlUtil` | `String mapToXmlStr(Map<?, ?> data,String rootName)` | 将Map转换为XML格式的字符串 |
| `cn.hutool.core.util.XmlUtil` | `String mapToXmlStr(Map<?, ?> data,String rootName,String namespace)` | 将Map转换为XML格式的字符串 |
| `cn.hutool.core.util.XmlUtil` | `String mapToXmlStr(Map<?, ?> data,String rootName,String namespace,String charset,boolean isPretty,boolean omitXmlDeclaration)` | 将Map转换为XML格式的字符串 |
| `cn.hutool.core.util.XmlUtil` | `String mapToXmlStr(Map<?, ?> data,String rootName,String namespace,boolean isPretty,boolean omitXmlDeclaration)` | 将Map转换为XML格式的字符串 |
| `cn.hutool.core.util.XmlUtil` | `String mapToXmlStr(Map<?, ?> data,String rootName,String namespace,boolean omitXmlDeclaration)` | 将Map转换为XML格式的字符串 |
| `cn.hutool.core.util.XmlUtil` | `String mapToXmlStr(Map<?, ?> data,boolean omitXmlDeclaration)` | 将Map转换为XML格式的字符串 |
| `cn.hutool.core.util.XmlUtil` | `String toStr(Document doc)` | 将XML文档转换为String 字符编码使用XML文档中的编码，获取不到则使用UTF-8 默认非格式化输出，若想格式化请使用#format(Document) |
| `cn.hutool.core.util.XmlUtil` | `String toStr(Document doc,String charset,boolean isPretty)` | 将XML文档转换为String 字符编码使用XML文档中的编码，获取不到则使用UTF-8 |
| `cn.hutool.core.util.XmlUtil` | `String toStr(Document doc,boolean isPretty)` | 将XML文档转换为String 字符编码使用XML文档中的编码，获取不到则使用UTF-8 |
| `cn.hutool.core.util.XmlUtil` | `String toStr(Node doc)` | 将XML文档转换为String 字符编码使用XML文档中的编码，获取不到则使用UTF-8 默认非格式化输出，若想格式化请使用#format(Document) |
| `cn.hutool.core.util.XmlUtil` | `String toStr(Node doc,String charset,boolean isPretty)` | 将XML文档转换为String 字符编码使用XML文档中的编码，获取不到则使用UTF-8 |
| `cn.hutool.core.util.XmlUtil` | `String toStr(Node doc,String charset,boolean isPretty,boolean omitXmlDeclaration)` | 将XML文档转换为String 字符编码使用XML文档中的编码，获取不到则使用UTF-8 |
| `cn.hutool.core.util.XmlUtil` | `String toStr(Node doc,boolean isPretty)` | 将XML文档转换为String 字符编码使用XML文档中的编码，获取不到则使用UTF-8 |
| `cn.hutool.core.util.XmlUtil` | `String unescape(String string)` | 反转义XML特殊字符: |
| `cn.hutool.core.util.XmlUtil` | `T xmlToBean(Node node,Class<T> bean)` | XML转Java Bean |
| `cn.hutool.core.util.XmlUtil` | `T xmlToBean(Node node,Class<T> bean,CopyOptions copyOptions)` | XML转Java Bean |
| `cn.hutool.core.util.XmlUtil` | `XPath createXPath()` | 创建XPath Xpath相关文章：https://www.ibm.com/developerworks/cn/xml/x-javaxpathapi.html |
| `cn.hutool.core.util.XmlUtil` | `boolean isElement(Node node)` | 给定节点是否为Element 类型节点 |
| `cn.hutool.core.util.XmlUtil` | `void append(Node node,Object data)` | 追加数据子节点，可以是Map、集合、文本 |
| `cn.hutool.core.util.XmlUtil` | `void disableDefaultDocumentBuilderFactory()` | 禁用默认的DocumentBuilderFactory，禁用后如果有第三方的实现（如oracle的xdb包中的xmlparse），将会自动加载实现。 |
| `cn.hutool.core.util.XmlUtil` | `void readBySax(File file,ContentHandler contentHandler)` | 使用Sax方式读取指定的XML 如果用户传入的contentHandler为DefaultHandler，则其接口都会被处理 |
| `cn.hutool.core.util.XmlUtil` | `void readBySax(InputSource source,ContentHandler contentHandler)` | 使用Sax方式读取指定的XML 如果用户传入的contentHandler为DefaultHandler，则其接口都会被处理 |
| `cn.hutool.core.util.XmlUtil` | `void readBySax(InputStream source,ContentHandler contentHandler)` | 使用Sax方式读取指定的XML 如果用户传入的contentHandler为DefaultHandler，则其接口都会被处理 |
| `cn.hutool.core.util.XmlUtil` | `void readBySax(Reader reader,ContentHandler contentHandler)` | 使用Sax方式读取指定的XML 如果用户传入的contentHandler为DefaultHandler，则其接口都会被处理 |
| `cn.hutool.core.util.XmlUtil` | `void setNamespaceAware(boolean isNamespaceAware)` | 设置是否打开命名空间支持，默认打开 |
| `cn.hutool.core.util.XmlUtil` | `void toFile(Document doc,String absolutePath)` | 将XML文档写入到文件 使用Document中的编码 |
| `cn.hutool.core.util.XmlUtil` | `void toFile(Document doc,String path,String charsetName)` | 将XML文档写入到文件 |
| `cn.hutool.core.util.XmlUtil` | `void transform(Source source,Result result,String charset,int indent)` | 将XML文档写出 格式化输出逻辑参考：https://stackoverflow.com/questions/139076/how-to-pretty-print-xml-from-java |
| `cn.hutool.core.util.XmlUtil` | `void transform(Source source,Result result,String charset,int indent,boolean omitXmlDeclaration)` | 将XML文档写出 格式化输出逻辑参考：https://stackoverflow.com/questions/139076/how-to-pretty-print-xml-from-java |
| `cn.hutool.core.util.XmlUtil` | `void write(Node node,OutputStream out,String charset,int indent)` | 将XML文档写出 |
| `cn.hutool.core.util.XmlUtil` | `void write(Node node,OutputStream out,String charset,int indent,boolean omitXmlDeclaration)` | 将XML文档写出 |
| `cn.hutool.core.util.XmlUtil` | `void write(Node node,Writer writer,String charset,int indent)` | 将XML文档写出 |
| `cn.hutool.core.util.XmlUtil` | `void write(Node node,Writer writer,String charset,int indent,boolean omitXmlDeclaration)` | 将XML文档写出 |
| `cn.hutool.core.util.XmlUtil` | `void writeObjectAsXml(File dest,Object bean)` | 将可序列化的对象转换为XML写入文件，已经存在的文件将被覆盖 Writes serializable object to a XML file. Existing file will be overwritten |
| `cn.hutool.core.util.XmlUtil$UniversalNamespaceCache` | `Iterator<String> getPrefixes(String namespaceURI)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.util.XmlUtil$UniversalNamespaceCache` | `String getNamespaceURI(String prefix)` | 【原文待译】This method is called by XPath. It returns the default namespace, if the prefix is null or "". |
| `cn.hutool.core.util.XmlUtil$UniversalNamespaceCache` | `String getPrefix(String namespaceURI)` | 【原文待译】This method is not needed in this context, but can be implemented in a similar way. |
| `cn.hutool.core.util.ZipUtil` | `File unzip(File zipFile)` | 解压到文件名相同的目录中，使用UTF-8编码 |
| `cn.hutool.core.util.ZipUtil` | `File unzip(File zipFile,Charset charset)` | 解压到文件名相同的目录中 |
| `cn.hutool.core.util.ZipUtil` | `File unzip(File zipFile,File outFile)` | 解压，默认使用UTF-8编码 |
| `cn.hutool.core.util.ZipUtil` | `File unzip(File zipFile,File outFile,Charset charset)` | 解压 |
| `cn.hutool.core.util.ZipUtil` | `File unzip(InputStream in,File outFile,Charset charset)` | 解压 ZIP条目不使用高速缓冲。 |
| `cn.hutool.core.util.ZipUtil` | `File unzip(String zipFilePath)` | 解压到文件名相同的目录中，默认编码UTF-8 |
| `cn.hutool.core.util.ZipUtil` | `File unzip(String zipFilePath,Charset charset)` | 解压到文件名相同的目录中 |
| `cn.hutool.core.util.ZipUtil` | `File unzip(String zipFilePath,String outFileDir)` | 解压，默认UTF-8编码 |
| `cn.hutool.core.util.ZipUtil` | `File unzip(String zipFilePath,String outFileDir,Charset charset)` | 解压 |
| `cn.hutool.core.util.ZipUtil` | `File unzip(ZipFile zipFile,File outFile)` | 解压 |
| `cn.hutool.core.util.ZipUtil` | `File unzip(ZipFile zipFile,File outFile,long limit)` | 限制解压后文件大小 |
| `cn.hutool.core.util.ZipUtil` | `File unzip(ZipInputStream zipStream,File outFile)` | 解压 ZIP条目不使用高速缓冲。 |
| `cn.hutool.core.util.ZipUtil` | `File zip(File srcFile)` | 打包到当前目录，使用默认编码UTF-8 |
| `cn.hutool.core.util.ZipUtil` | `File zip(File srcFile,Charset charset)` | 打包到当前目录 |
| `cn.hutool.core.util.ZipUtil` | `File zip(File zipFile,Charset charset,Resource... resources)` | 对流中的数据加入到压缩文件 路径列表和流列表长度必须一致 |
| `cn.hutool.core.util.ZipUtil` | `File zip(File zipFile,Charset charset,boolean withSrcDir,File... srcFiles)` | 对文件或文件目录进行压缩 |
| `cn.hutool.core.util.ZipUtil` | `File zip(File zipFile,Charset charset,boolean withSrcDir,FileFilter filter,File... srcFiles)` | 对文件或文件目录进行压缩 |
| `cn.hutool.core.util.ZipUtil` | `File zip(File zipFile,String path,InputStream in)` | 对流中的数据加入到压缩文件 使用默认编码UTF-8 |
| `cn.hutool.core.util.ZipUtil` | `File zip(File zipFile,String path,InputStream in,Charset charset)` | 对流中的数据加入到压缩文件 |
| `cn.hutool.core.util.ZipUtil` | `File zip(File zipFile,String path,String data)` | 对流中的数据加入到压缩文件，使用默认UTF-8编码 |
| `cn.hutool.core.util.ZipUtil` | `File zip(File zipFile,String path,String data,Charset charset)` | 对流中的数据加入到压缩文件 |
| `cn.hutool.core.util.ZipUtil` | `File zip(File zipFile,String[] paths,InputStream[] ins)` | 对流中的数据加入到压缩文件 路径列表和流列表长度必须一致 |
| `cn.hutool.core.util.ZipUtil` | `File zip(File zipFile,String[] paths,InputStream[] ins,Charset charset)` | 对流中的数据加入到压缩文件 路径列表和流列表长度必须一致 |
| `cn.hutool.core.util.ZipUtil` | `File zip(File zipFile,boolean withSrcDir,File... srcFiles)` | 对文件或文件目录进行压缩 使用默认UTF-8编码 |
| `cn.hutool.core.util.ZipUtil` | `File zip(String srcPath)` | 打包到当前目录，使用默认编码UTF-8 |
| `cn.hutool.core.util.ZipUtil` | `File zip(String srcPath,Charset charset)` | 打包到当前目录 |
| `cn.hutool.core.util.ZipUtil` | `File zip(String srcPath,String zipPath)` | 对文件或文件目录进行压缩 不包含被打包目录 |
| `cn.hutool.core.util.ZipUtil` | `File zip(String srcPath,String zipPath,Charset charset,boolean withSrcDir)` | 对文件或文件目录进行压缩 |
| `cn.hutool.core.util.ZipUtil` | `File zip(String srcPath,String zipPath,boolean withSrcDir)` | 对文件或文件目录进行压缩 |
| `cn.hutool.core.util.ZipUtil` | `InputStream get(File zipFile,Charset charset,String path)` | 获取压缩包中的指定文件流 |
| `cn.hutool.core.util.ZipUtil` | `InputStream get(ZipFile zipFile,String path)` | 获取压缩包中的指定文件流 |
| `cn.hutool.core.util.ZipUtil` | `InputStream getStream(ZipFile zipFile,ZipEntry zipEntry)` | 获取指定ZipEntry的流，用于读取这个entry的内容 此处使用LimitedInputStream 限制最大写出大小，避免ZIP bomb漏洞 |
| `cn.hutool.core.util.ZipUtil` | `List<String> listFileNames(ZipFile zipFile,String dir)` | 获取Zip文件中指定目录下的所有文件，只显示文件，不显示目录 此方法并不会关闭ZipFile。 |
| `cn.hutool.core.util.ZipUtil` | `String unGzip(byte[] buf,String charset)` | Gzip解压缩处理 |
| `cn.hutool.core.util.ZipUtil` | `String unZlib(byte[] buf,String charset)` | Zlib解压缩处理 |
| `cn.hutool.core.util.ZipUtil` | `ZipFile toZipFile(File file,Charset charset)` | 将Zip文件转换为ZipFile |
| `cn.hutool.core.util.ZipUtil` | `ZipOutputStream getZipOutputStream(OutputStream out,Charset charset)` | 获得 ZipOutputStream |
| `cn.hutool.core.util.ZipUtil` | `byte[] gzip(File file)` | Gzip压缩文件 |
| `cn.hutool.core.util.ZipUtil` | `byte[] gzip(InputStream in)` | Gzip压缩文件 |
| `cn.hutool.core.util.ZipUtil` | `byte[] gzip(InputStream in,int length)` | Gzip压缩文件 |
| `cn.hutool.core.util.ZipUtil` | `byte[] gzip(String content,String charset)` | Gzip压缩处理 |
| `cn.hutool.core.util.ZipUtil` | `byte[] gzip(byte[] buf)` | Gzip压缩处理 |
| `cn.hutool.core.util.ZipUtil` | `byte[] unGzip(InputStream in)` | Gzip解压处理 |
| `cn.hutool.core.util.ZipUtil` | `byte[] unGzip(InputStream in,int length)` | Gzip解压处理 |
| `cn.hutool.core.util.ZipUtil` | `byte[] unGzip(byte[] buf)` | Gzip解压处理 |
| `cn.hutool.core.util.ZipUtil` | `byte[] unZlib(InputStream in)` | 解压缩zlib |
| `cn.hutool.core.util.ZipUtil` | `byte[] unZlib(InputStream in,int length)` | 解压缩zlib |
| `cn.hutool.core.util.ZipUtil` | `byte[] unZlib(byte[] buf)` | 解压缩zlib |
| `cn.hutool.core.util.ZipUtil` | `byte[] unzipFileBytes(File zipFile,Charset charset,String name)` | 从Zip文件中提取指定的文件为bytes |
| `cn.hutool.core.util.ZipUtil` | `byte[] unzipFileBytes(File zipFile,String name)` | 从Zip文件中提取指定的文件为bytes |
| `cn.hutool.core.util.ZipUtil` | `byte[] unzipFileBytes(String zipFilePath,Charset charset,String name)` | 从Zip文件中提取指定的文件为bytes |
| `cn.hutool.core.util.ZipUtil` | `byte[] unzipFileBytes(String zipFilePath,String name)` | 从Zip文件中提取指定的文件为bytes |
| `cn.hutool.core.util.ZipUtil` | `byte[] zlib(File file,int level)` | Zlib压缩文件 |
| `cn.hutool.core.util.ZipUtil` | `byte[] zlib(InputStream in,int level)` | 打成Zlib压缩包 |
| `cn.hutool.core.util.ZipUtil` | `byte[] zlib(InputStream in,int level,int length)` | 打成Zlib压缩包 |
| `cn.hutool.core.util.ZipUtil` | `byte[] zlib(String content,String charset,int level)` | Zlib压缩处理 |
| `cn.hutool.core.util.ZipUtil` | `byte[] zlib(byte[] buf,int level)` | 打成Zlib压缩包 |
| `cn.hutool.core.util.ZipUtil` | `void append(Path zipPath,Path appendFilePath,CopyOption... options)` | 在zip文件中添加新文件或目录 新文件添加在zip根目录，文件夹包括其本身和内容 如果待添加文件夹是系统根路径（如/或c:/），则只复制文件夹下的内容 |
| `cn.hutool.core.util.ZipUtil` | `void read(ZipFile zipFile,Consumer<ZipEntry> consumer)` | 读取并处理Zip文件中的每一个ZipEntry |
| `cn.hutool.core.util.ZipUtil` | `void read(ZipInputStream zipStream,Consumer<ZipEntry> consumer)` | 读取并处理Zip流中的每一个ZipEntry |
| `cn.hutool.core.util.ZipUtil` | `void zip(OutputStream out,Charset charset,boolean withSrcDir,FileFilter filter,File... srcFiles)` | 对文件或文件目录进行压缩 |
| `cn.hutool.core.util.ZipUtil` | `void zip(OutputStream out,String[] paths,InputStream[] ins)` | 将文件流压缩到目标流中 |
| `cn.hutool.core.util.ZipUtil` | `void zip(ZipOutputStream zipOutputStream,String[] paths,InputStream[] ins)` | 将文件流压缩到目标流中 |
| `cn.hutool.core.util.ZipUtil` | `void zip(ZipOutputStream zipOutputStream,boolean withSrcDir,FileFilter filter,File... srcFiles)` | 对文件或文件目录进行压缩 |
