# cn.hutool.core.lang

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.lang.Assert` | `Number checkBetween(Number value,Number min,Number max)` | 检查值是否在指定范围内 |
| `cn.hutool.core.lang.Assert` | `String notContain(String textToSearch,String substring)` | 断言给定字符串是否不被另一个字符串包含（即是否为子串） |
| `cn.hutool.core.lang.Assert` | `String notContain(String textToSearch,String substring,String errorMsgTemplate,Object... params)` | 断言给定字符串是否不被另一个字符串包含（即是否为子串） |
| `cn.hutool.core.lang.Assert` | `T isInstanceOf(Class<?> type,T obj)` | 断言给定对象是否是给定类的实例 |
| `cn.hutool.core.lang.Assert` | `T isInstanceOf(Class<?> type,T obj,String errorMsgTemplate,Object... params)` | 断言给定对象是否是给定类的实例 |
| `cn.hutool.core.lang.Assert` | `T notBlank(T text)` | 检查给定字符串是否为空白（null、空串或只包含空白符），为空抛出 IllegalArgumentException |
| `cn.hutool.core.lang.Assert` | `T notBlank(T text,String errorMsgTemplate,Object... params)` | 检查给定字符串是否为空白（null、空串或只包含空白符），为空抛出 IllegalArgumentException |
| `cn.hutool.core.lang.Assert` | `T notBlank(T text,Supplier<X> errorMsgSupplier)` | 检查给定字符串是否为空白（null、空串或只包含空白符），为空抛出自定义异常。 并使用指定的函数获取错误信息返回 |
| `cn.hutool.core.lang.Assert` | `T notContain(CharSequence textToSearch,T substring,Supplier<X> errorSupplier)` | 断言给定字符串是否不被另一个字符串包含（即是否为子串） 并使用指定的函数获取错误信息返回 |
| `cn.hutool.core.lang.Assert` | `T notEmpty(T collection)` | 断言给定集合非空 |
| `cn.hutool.core.lang.Assert` | `T notEmpty(T collection,String errorMsgTemplate,Object... params)` | 断言给定集合非空 |
| `cn.hutool.core.lang.Assert` | `T notEmpty(T collection,Supplier<X> errorSupplier)` | 断言给定集合非空 并使用指定的函数获取错误信息返回 |
| `cn.hutool.core.lang.Assert` | `T notEmpty(T map)` | 断言给定Map非空 |
| `cn.hutool.core.lang.Assert` | `T notEmpty(T map,String errorMsgTemplate,Object... params)` | 断言给定Map非空 |
| `cn.hutool.core.lang.Assert` | `T notEmpty(T map,Supplier<X> errorSupplier)` | 断言给定Map非空 并使用指定的函数获取错误信息返回 |
| `cn.hutool.core.lang.Assert` | `T notEmpty(T text)` | 检查给定字符串是否为空，为空抛出 IllegalArgumentException |
| `cn.hutool.core.lang.Assert` | `T notEmpty(T text,String errorMsgTemplate,Object... params)` | 检查给定字符串是否为空，为空抛出 IllegalArgumentException |
| `cn.hutool.core.lang.Assert` | `T notEmpty(T text,Supplier<X> errorSupplier)` | 检查给定字符串是否为空，为空抛出自定义异常，并使用指定的函数获取错误信息返回。 |
| `cn.hutool.core.lang.Assert` | `T notNull(T object)` | 断言对象是否不为null ，如果为null 抛出IllegalArgumentException 异常 |
| `cn.hutool.core.lang.Assert` | `T notNull(T object,String errorMsgTemplate,Object... params)` | 断言对象是否不为null ，如果为null 抛出IllegalArgumentException 异常 Assert that an object is not null . |
| `cn.hutool.core.lang.Assert` | `T notNull(T object,Supplier<X> errorSupplier)` | 断言对象是否不为null ，如果为null 抛出指定类型异常 并使用指定的函数获取错误信息返回 |
| `cn.hutool.core.lang.Assert` | `T[] noNullElements(T[] array)` | 断言给定数组是否不包含null元素，如果数组为空或 null将被认为不包含 |
| `cn.hutool.core.lang.Assert` | `T[] noNullElements(T[] array,String errorMsgTemplate,Object... params)` | 断言给定数组是否不包含null元素，如果数组为空或 null将被认为不包含 |
| `cn.hutool.core.lang.Assert` | `T[] noNullElements(T[] array,Supplier<X> errorSupplier)` | 断言给定数组是否不包含null元素，如果数组为空或 null将被认为不包含 并使用指定的函数获取错误信息返回 |
| `cn.hutool.core.lang.Assert` | `T[] notEmpty(T[] array)` | 断言给定数组是否包含元素，数组必须不为 null 且至少包含一个元素 |
| `cn.hutool.core.lang.Assert` | `T[] notEmpty(T[] array,String errorMsgTemplate,Object... params)` | 断言给定数组是否包含元素，数组必须不为 null 且至少包含一个元素 |
| `cn.hutool.core.lang.Assert` | `T[] notEmpty(T[] array,Supplier<X> errorSupplier)` | 断言给定数组是否包含元素，数组必须不为 null 且至少包含一个元素 并使用指定的函数获取错误信息返回 |
| `cn.hutool.core.lang.Assert` | `double checkBetween(double value,double min,double max)` | 检查值是否在指定范围内 |
| `cn.hutool.core.lang.Assert` | `double checkBetween(double value,double min,double max,String errorMsgTemplate,Object... params)` | 检查值是否在指定范围内 |
| `cn.hutool.core.lang.Assert` | `double checkBetween(double value,double min,double max,Supplier<? extends X> errorSupplier)` | 检查值是否在指定范围内 |
| `cn.hutool.core.lang.Assert` | `int checkBetween(int value,int min,int max)` | 检查值是否在指定范围内 |
| `cn.hutool.core.lang.Assert` | `int checkBetween(int value,int min,int max,String errorMsgTemplate,Object... params)` | 检查值是否在指定范围内 |
| `cn.hutool.core.lang.Assert` | `int checkBetween(int value,int min,int max,Supplier<? extends X> errorSupplier)` | 检查值是否在指定范围内 |
| `cn.hutool.core.lang.Assert` | `int checkIndex(int index,int size)` | 检查下标（数组、集合、字符串）是否符合要求，下标必须满足： |
| `cn.hutool.core.lang.Assert` | `int checkIndex(int index,int size,String errorMsgTemplate,Object... params)` | 检查下标（数组、集合、字符串）是否符合要求，下标必须满足： |
| `cn.hutool.core.lang.Assert` | `long checkBetween(long value,long min,long max)` | 检查值是否在指定范围内 |
| `cn.hutool.core.lang.Assert` | `long checkBetween(long value,long min,long max,String errorMsgTemplate,Object... params)` | 检查值是否在指定范围内 |
| `cn.hutool.core.lang.Assert` | `long checkBetween(long value,long min,long max,Supplier<? extends X> errorSupplier)` | 检查值是否在指定范围内 |
| `cn.hutool.core.lang.Assert` | `void empty(T collection)` | 断言给定集合为空 |
| `cn.hutool.core.lang.Assert` | `void empty(T collection,String errorMsgTemplate,Object... params)` | 断言给定集合为空 |
| `cn.hutool.core.lang.Assert` | `void empty(T collection,Supplier<X> errorSupplier)` | 断言给定集合为空 并使用指定的函数获取错误信息返回 |
| `cn.hutool.core.lang.Assert` | `void equals(Object obj1,Object obj2)` | 断言两个对象是否相等,如果两个对象不相等 抛出IllegalArgumentException 异常 |
| `cn.hutool.core.lang.Assert` | `void equals(Object obj1,Object obj2,String errorMsgTemplate,Object... params)` | 断言两个对象是否相等,如果两个对象不相等 抛出IllegalArgumentException 异常 |
| `cn.hutool.core.lang.Assert` | `void equals(Object obj1,Object obj2,Supplier<X> errorSupplier)` | 断言两个对象是否相等,如果两个对象不相等,抛出指定类型异常,并使用指定的函数获取错误信息返回 |
| `cn.hutool.core.lang.Assert` | `void isAssignable(Class<?> superType,Class<?> subType)` | 断言 superType.isAssignableFrom(subType) 是否为 true. |
| `cn.hutool.core.lang.Assert` | `void isAssignable(Class<?> superType,Class<?> subType,String errorMsgTemplate,Object... params)` | 断言 superType.isAssignableFrom(subType) 是否为 true. |
| `cn.hutool.core.lang.Assert` | `void isFalse(boolean expression)` | 断言是否为假，如果为 true 抛出 IllegalArgumentException 异常 |
| `cn.hutool.core.lang.Assert` | `void isFalse(boolean expression,String errorMsgTemplate,Object... params)` | 断言是否为假，如果为 true 抛出 IllegalArgumentException 异常 |
| `cn.hutool.core.lang.Assert` | `void isFalse(boolean expression,Supplier<X> errorSupplier)` | 断言是否为假，如果为 true 抛出指定类型异常 并使用指定的函数获取错误信息返回 |
| `cn.hutool.core.lang.Assert` | `void isNull(Object object)` | 断言对象是否为null ，如果不为null 抛出IllegalArgumentException 异常 |
| `cn.hutool.core.lang.Assert` | `void isNull(Object object,String errorMsgTemplate,Object... params)` | 断言对象是否为null ，如果不为null 抛出IllegalArgumentException 异常 |
| `cn.hutool.core.lang.Assert` | `void isNull(Object object,Supplier<X> errorSupplier)` | 断言对象是否为null ，如果不为null 抛出指定类型异常 并使用指定的函数获取错误信息返回 |
| `cn.hutool.core.lang.Assert` | `void isTrue(boolean expression)` | 断言是否为真，如果为 false 抛出 IllegalArgumentException 异常 |
| `cn.hutool.core.lang.Assert` | `void isTrue(boolean expression,String errorMsgTemplate,Object... params)` | 断言是否为真，如果为 false 抛出 IllegalArgumentException 异常 |
| `cn.hutool.core.lang.Assert` | `void isTrue(boolean expression,Supplier<? extends X> supplier)` | 断言是否为真，如果为 false 抛出给定的异常 |
| `cn.hutool.core.lang.Assert` | `void notEquals(Object obj1,Object obj2)` | 断言两个对象是否不相等,如果两个对象相等 抛出IllegalArgumentException 异常 |
| `cn.hutool.core.lang.Assert` | `void notEquals(Object obj1,Object obj2,String errorMsgTemplate,Object... params)` | 断言两个对象是否不相等,如果两个对象相等 抛出IllegalArgumentException 异常 |
| `cn.hutool.core.lang.Assert` | `void notEquals(Object obj1,Object obj2,Supplier<X> errorSupplier)` | 断言两个对象是否不相等,如果两个对象相等,抛出指定类型异常,并使用指定的函数获取错误信息返回 |
| `cn.hutool.core.lang.Assert` | `void state(boolean expression)` | 检查boolean表达式，当检查结果为false时抛出 IllegalStateException。 |
| `cn.hutool.core.lang.Assert` | `void state(boolean expression,String errorMsgTemplate,Object... params)` | 检查boolean表达式，当检查结果为false时抛出 IllegalStateException。 |
| `cn.hutool.core.lang.Assert` | `void state(boolean expression,Supplier<String> errorMsgSupplier)` | 检查boolean表达式，当检查结果为false时抛出 IllegalStateException。 并使用指定的函数获取错误信息返回 |
| `cn.hutool.core.lang.Chain` | `T addChain(E element)` | 加入责任链 |
| `cn.hutool.core.lang.ClassScanner` | `ClassScanner setIgnoreLoadError(boolean ignoreLoadError)` | 设置是否忽略loadClass时的错误 |
| `cn.hutool.core.lang.ClassScanner` | `Set<Class<?>> scan()` | 扫描包路径下满足class过滤器条件的所有class文件 此方法首先扫描指定包名下的资源目录，如果未扫描到，则扫描整个classpath中所有加载的类 |
| `cn.hutool.core.lang.ClassScanner` | `Set<Class<?>> scan(boolean forceScanJavaClassPaths)` | 扫描包路径下满足class过滤器条件的所有class文件 |
| `cn.hutool.core.lang.ClassScanner` | `Set<Class<?>> scanAllPackage()` | 扫描该包路径下所有class文件，包括其他加载的jar或者类 |
| `cn.hutool.core.lang.ClassScanner` | `Set<Class<?>> scanAllPackage(String packageName,Filter<Class<?>> classFilter)` | 扫描包路径下和所有在classpath中加载的类，满足class过滤器条件的所有class文件， 如果包路径为 com.abs + A.class 但是输入 abs会产生classNotFoundException 因为className 应该为 com.abs.A 现在却成为abs.A,此工具类对该异常进行忽略处理 |
| `cn.hutool.core.lang.ClassScanner` | `Set<Class<?>> scanAllPackageByAnnotation(String packageName,Class<? extends Annotation> annotationClass)` | 扫描指定包路径下所有包含指定注解的类，包括其他加载的jar或者类 |
| `cn.hutool.core.lang.ClassScanner` | `Set<Class<?>> scanAllPackageBySuper(String packageName,Class<?> superClass)` | 扫描指定包路径下所有指定类或接口的子类或实现类，不包括指定父类本身，包括其他加载的jar或者类 |
| `cn.hutool.core.lang.ClassScanner` | `Set<Class<?>> scanPackage()` | 扫描classpath下所有class文件，如果classpath下已经有类，不再扫描其他加载的jar或者类 |
| `cn.hutool.core.lang.ClassScanner` | `Set<Class<?>> scanPackage(String packageName)` | 扫描该包路径下所有class文件 |
| `cn.hutool.core.lang.ClassScanner` | `Set<Class<?>> scanPackage(String packageName,Filter<Class<?>> classFilter)` | 扫描包路径下满足class过滤器条件的所有class文件， 如果包路径为 com.abs + A.class 但是输入 abs会产生classNotFoundException 因为className 应该为 com.abs.A 现在却成为abs.A,此工具类对该异常进行忽略处理 |
| `cn.hutool.core.lang.ClassScanner` | `Set<Class<?>> scanPackageByAnnotation(String packageName,Class<? extends Annotation> annotationClass)` | 扫描指定包路径下所有包含指定注解的类 如果classpath下已经有类，不再扫描其他加载的jar或者类 |
| `cn.hutool.core.lang.ClassScanner` | `Set<Class<?>> scanPackageBySuper(String packageName,Class<?> superClass)` | 扫描指定包路径下所有指定类或接口的子类或实现类，不包括指定父类本身 如果classpath下已经有类，不再扫描其他加载的jar或者类 |
| `cn.hutool.core.lang.ClassScanner` | `Set<String> getClassesOfLoadError()` | 忽略加载错误扫描后，可以获得之前扫描时加载错误的类名字集合 |
| `cn.hutool.core.lang.ClassScanner` | `void setClassLoader(ClassLoader classLoader)` | 设置自定义的类加载器 |
| `cn.hutool.core.lang.ClassScanner` | `void setInitialize(boolean initialize)` | 设置是否在扫描到类时初始化类 |
| `cn.hutool.core.lang.ConsistentHash` | `T get(Object key)` | 获得一个最近的顺时针节点 |
| `cn.hutool.core.lang.ConsistentHash` | `void add(T node)` | 增加节点 每增加一个节点，就会在闭环上增加给定复制节点数 例如复制节点数是2，则每调用此方法一次，增加两个虚拟节点，这两个节点指向同一Node 由于hash算法会调用node的toString方法，故按照toString去重 |
| `cn.hutool.core.lang.ConsistentHash` | `void remove(T node)` | 移除节点的同时移除相应的虚拟节点 |
| `cn.hutool.core.lang.Console` | `Integer lineNumber()` | 返回当前行号 (不支持Lambda、内部类、递归内使用) |
| `cn.hutool.core.lang.Console` | `Scanner scanner()` | 创建从控制台读取内容的Scanner |
| `cn.hutool.core.lang.Console` | `String input()` | 读取用户输入的内容（在控制台敲回车前的内容） |
| `cn.hutool.core.lang.Console` | `String where()` | 返回当前位置+行号 (不支持Lambda、内部类、递归内使用) |
| `cn.hutool.core.lang.Console` | `void error()` | 同 System.err.println()方法，打印控制台日志 |
| `cn.hutool.core.lang.Console` | `void error(Object obj)` | 同 System.err.println()方法，打印控制台日志 |
| `cn.hutool.core.lang.Console` | `void error(Object obj1,Object... otherObjs)` | 同 System.out.println()方法，打印控制台日志 如果传入打印对象为Throwable对象，那么同时打印堆栈 |
| `cn.hutool.core.lang.Console` | `void error(String template,Object... values)` | 同 System.err.println()方法，打印控制台日志 |
| `cn.hutool.core.lang.Console` | `void error(Throwable t,String template,Object... values)` | 同 System.err.println()方法，打印控制台日志 |
| `cn.hutool.core.lang.Console` | `void log()` | 同 System.out.println()方法，打印控制台日志 |
| `cn.hutool.core.lang.Console` | `void log(Object obj)` | 同 System.out.println()方法，打印控制台日志 如果传入打印对象为Throwable对象，那么同时打印堆栈 |
| `cn.hutool.core.lang.Console` | `void log(Object obj1,Object... otherObjs)` | 同 System.out.println()方法，打印控制台日志 如果传入打印对象为Throwable对象，那么同时打印堆栈 |
| `cn.hutool.core.lang.Console` | `void log(String template,Object... values)` | 同 System.out.println()方法，打印控制台日志 当传入template无"{}"时，被认为非模板，直接打印多个参数以空格分隔 |
| `cn.hutool.core.lang.Console` | `void log(Throwable t,String template,Object... values)` | 同 System.out.println()方法，打印控制台日志 |
| `cn.hutool.core.lang.Console` | `void print(Object obj)` | 同 System.out.print()方法，打印控制台日志 |
| `cn.hutool.core.lang.Console` | `void print(Object obj1,Object... otherObjs)` | 同 System.out.println()方法，打印控制台日志 如果传入打印对象为Throwable对象，那么同时打印堆栈 |
| `cn.hutool.core.lang.Console` | `void print(String template,Object... values)` | 同 System.out.print()方法，打印控制台日志 |
| `cn.hutool.core.lang.Console` | `void printProgress(char showChar,int len)` | 打印进度条 |
| `cn.hutool.core.lang.Console` | `void printProgress(char showChar,int totalLen,double rate)` | 打印进度条 |
| `cn.hutool.core.lang.Console` | `void table(ConsoleTable consoleTable)` | 打印表格到控制台 |
| `cn.hutool.core.lang.ConsoleTable` | `ConsoleTable addBody(String... values)` | 添加体信息 |
| `cn.hutool.core.lang.ConsoleTable` | `ConsoleTable addHeader(String... titles)` | 添加头信息 |
| `cn.hutool.core.lang.ConsoleTable` | `ConsoleTable create()` | 创建ConsoleTable对象 |
| `cn.hutool.core.lang.ConsoleTable` | `ConsoleTable setSBCMode(boolean isSBCMode)` | 设置是否使用全角模式 当包含中文字符时，输出的表格可能无法对齐，因此当设置为全角模式时，全部字符转为全角。 |
| `cn.hutool.core.lang.ConsoleTable` | `String toString()` | 获取表格字符串 |
| `cn.hutool.core.lang.ConsoleTable` | `void print()` | 打印到控制台 |
| `cn.hutool.core.lang.DefaultSegment` | `T getEndIndex()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.DefaultSegment` | `T getStartIndex()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Dict` | `BigDecimal getBigDecimal(String attr)` | @param attr 字段名 |
| `cn.hutool.core.lang.Dict` | `BigInteger getBigInteger(String attr)` | @param attr 字段名 |
| `cn.hutool.core.lang.Dict` | `Boolean getBool(String attr)` | @param attr 字段名 |
| `cn.hutool.core.lang.Dict` | `Byte getByte(String attr)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Dict` | `Character getChar(String attr)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Dict` | `Date getDate(String attr)` | @param attr 字段名 |
| `cn.hutool.core.lang.Dict` | `Dict clone()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Dict` | `Dict create()` | 创建Dict |
| `cn.hutool.core.lang.Dict` | `Dict filter(String... keys)` | 过滤Map保留指定键值对，如果键不存在跳过 |
| `cn.hutool.core.lang.Dict` | `Dict of(Object... keysAndValues)` | 根据给定的键值对数组创建Dict对象，传入参数必须为key,value,key,value... 奇数参数必须为key，key最后会转换为String类型。 偶数参数必须为value，可以为任意类型。 |
| `cn.hutool.core.lang.Dict` | `Dict of(Pair<String, Object>... pairs)` | 根据给定的Pair数组创建Dict对象 |
| `cn.hutool.core.lang.Dict` | `Dict parse(T bean)` | 将PO对象转为Dict |
| `cn.hutool.core.lang.Dict` | `Dict parseBean(T bean)` | 将值对象转换为Dict 类名会被当作表名，小写第一个字母 |
| `cn.hutool.core.lang.Dict` | `Dict parseBean(T bean,boolean isToUnderlineCase,boolean ignoreNullValue)` | 将值对象转换为Dict 类名会被当作表名，小写第一个字母 |
| `cn.hutool.core.lang.Dict` | `Dict set(String attr,Object value)` | 设置列 |
| `cn.hutool.core.lang.Dict` | `Dict setFields(Func0<?>... fields)` | 通过lambda批量设置值 实际使用时，可以使用getXXX的方法引用来完成键值对的赋值： |
| `cn.hutool.core.lang.Dict` | `Dict setIgnoreNull(String attr,Object value)` | 设置列，当键或值为null时忽略 |
| `cn.hutool.core.lang.Dict` | `Double getDouble(String attr)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Dict` | `E getEnum(Class<E> clazz,String key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Dict` | `Float getFloat(String attr)` | @param attr 字段名 |
| `cn.hutool.core.lang.Dict` | `Integer getInt(String attr)` | @param attr 字段名 |
| `cn.hutool.core.lang.Dict` | `Long getLong(String attr)` | @param attr 字段名 |
| `cn.hutool.core.lang.Dict` | `Number getNumber(String attr)` | @param attr 字段名 |
| `cn.hutool.core.lang.Dict` | `Object compute(final String key,final BiFunction<? super String, ? super Object, ?> remappingFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Dict` | `Object computeIfAbsent(String key,Function<? super String, ?> mappingFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Dict` | `Object computeIfPresent(final String key,final BiFunction<? super String, ? super Object, ?> remappingFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Dict` | `Object get(Object key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Dict` | `Object getObj(String key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Dict` | `Object getOrDefault(Object key,Object defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Dict` | `Object merge(final String key,final Object value,final BiFunction<? super Object, ? super Object, ?> remappingFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Dict` | `Object put(String key,Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Dict` | `Object putIfAbsent(String key,Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Dict` | `Object remove(Object key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Dict` | `Object replace(String key,Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Dict` | `Short getShort(String attr)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Dict` | `String getStr(String attr)` | @param attr 字段名 |
| `cn.hutool.core.lang.Dict` | `T get(String attr,T defaultValue)` | 获得特定类型值 |
| `cn.hutool.core.lang.Dict` | `T getBean(String attr)` | 获得特定类型值 |
| `cn.hutool.core.lang.Dict` | `T getByPath(String expression)` | 通过表达式获取JSON中嵌套的对象 .表达式，可以获取Bean对象中的属性（字段）值或者Map中key对应的值 []表达式，可以获取集合等对象中对应index的值 表达式栗子： |
| `cn.hutool.core.lang.Dict` | `T getByPath(String expression,Class<T> resultType)` | 通过表达式获取JSON中嵌套的对象 .表达式，可以获取Bean对象中的属性（字段）值或者Map中key对应的值 []表达式，可以获取集合等对象中对应index的值 表达式栗子： |
| `cn.hutool.core.lang.Dict` | `T toBean(Class<T> clazz)` | 填充Value Object对象 |
| `cn.hutool.core.lang.Dict` | `T toBean(T bean)` | 转换为Bean对象 |
| `cn.hutool.core.lang.Dict` | `T toBean(T bean,boolean isToCamelCase)` | 转换为Bean对象 |
| `cn.hutool.core.lang.Dict` | `T toBeanIgnoreCase(Class<T> clazz)` | 填充Value Object对象，忽略大小写 |
| `cn.hutool.core.lang.Dict` | `T toBeanIgnoreCase(T bean)` | 转换为Bean对象 |
| `cn.hutool.core.lang.Dict` | `T toBeanWithCamelCase(T bean)` | 转换为Bean对象,并使用驼峰法模式转换 |
| `cn.hutool.core.lang.Dict` | `Time getTime(String attr)` | @param attr 字段名 |
| `cn.hutool.core.lang.Dict` | `Timestamp getTimestamp(String attr)` | @param attr 字段名 |
| `cn.hutool.core.lang.Dict` | `boolean containsKey(Object key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Dict` | `boolean remove(Object key,Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Dict` | `boolean replace(String key,Object oldValue,Object newValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Dict` | `byte[] getBytes(String attr)` | @param attr 字段名 |
| `cn.hutool.core.lang.Dict` | `void putAll(Map<? extends String, ?> m)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Dict` | `void removeEqual(T dict,String... withoutNames)` | 与给定实体对比并去除相同的部分 此方法用于在更新操作时避免所有字段被更新，跳过不需要更新的字段 version from 2.0.0 |
| `cn.hutool.core.lang.Editor` | `T edit(T t)` | 修改过滤后的结果 |
| `cn.hutool.core.lang.EnumItem` | `E fromInt(Integer intVal)` | 通过int类型值查找兄弟其他枚举 |
| `cn.hutool.core.lang.EnumItem` | `E fromStr(String strVal)` | 通过String类型的值转换，根据实现可以用name/text |
| `cn.hutool.core.lang.EnumItem` | `E[] items()` | 获取所有枚举对象 |
| `cn.hutool.core.lang.EnumItem` | `String name()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.EnumItem` | `String text()` | 在中文语境下，多数时间枚举会配合一个中文说明 |
| `cn.hutool.core.lang.EnumItem` | `int intVal()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Filter` | `boolean accept(T t)` | 是否接受对象 |
| `cn.hutool.core.lang.JarClassLoader` | `JarClassLoader addJar(File jarFileOrDir)` | 加载Jar文件，或者加载目录 |
| `cn.hutool.core.lang.JarClassLoader` | `JarClassLoader addURL(File dir)` | 增加class所在目录或文件 如果为目录，此目录用于搜索class文件，如果为文件，需为jar文件 |
| `cn.hutool.core.lang.JarClassLoader` | `JarClassLoader load(File dir)` | 加载Jar到ClassPath |
| `cn.hutool.core.lang.JarClassLoader` | `JarClassLoader loadJar(File jarFile)` | 加载Jar到ClassPath |
| `cn.hutool.core.lang.JarClassLoader` | `URLClassLoader loadJarToSystemClassLoader(File jarFile)` | 加载Jar文件到System ClassLoader中 |
| `cn.hutool.core.lang.JarClassLoader` | `void addURL(URL url)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.JarClassLoader` | `void loadJar(URLClassLoader loader,File jarFile)` | 加载Jar文件到指定loader中 |
| `cn.hutool.core.lang.Matcher` | `boolean match(T t)` | 给定对象是否匹配 |
| `cn.hutool.core.lang.ObjectId` | `String next()` | 获取一个objectId用下划线分割 |
| `cn.hutool.core.lang.ObjectId` | `String next(boolean withHyphen)` | 获取一个objectId |
| `cn.hutool.core.lang.ObjectId` | `boolean isValid(String s)` | 给定的字符串是否为有效的ObjectId |
| `cn.hutool.core.lang.ObjectId` | `byte[] nextBytes()` | 获取一个objectId的bytes表现形式 |
| `cn.hutool.core.lang.Opt` | `Exception getException()` | 获取异常 当调用 #ofTry(Func0)时，异常信息不会抛出，而是保存，调用此方法获取抛出的异常 |
| `cn.hutool.core.lang.Opt` | `Opt<R> ofEmptyAble(R value)` | 返回一个包裹里List集合可能为空的Opt，额外判断了集合内元素为空的情况 |
| `cn.hutool.core.lang.Opt` | `Opt<T> empty()` | 返回一个空的Opt |
| `cn.hutool.core.lang.Opt` | `Opt<T> filter(Predicate<? super T> predicate)` | 判断包裹里的值存在并且与给定的条件是否满足 (Predicate#test执行结果是否为true) 如果满足条件则返回本身 不满足条件或者元素本身为空时返回一个返回一个空的Opt |
| `cn.hutool.core.lang.Opt` | `Opt<T> ifFail(final Consumer<? super Throwable> action)` | 如果包裹内容失败了，则执行传入的操作(Consumer#accept) 例如执行有异常就打印结果 |
| `cn.hutool.core.lang.Opt` | `Opt<T> ifPresent(Consumer<? super T> action)` | 如果包裹里的值存在，就执行传入的操作(Consumer#accept) 例如如果值存在就打印结果 |
| `cn.hutool.core.lang.Opt` | `Opt<T> ifPresentOrElse(Consumer<? super T> action,VoidFunc0 emptyAction)` | 如果包裹里的值存在，就执行传入的值存在时的操作(Consumer#accept) 否则执行传入的值不存在时的操作(VoidFunc0中的VoidFunc0#call()) 例如值存在就打印对应的值，不存在则用Console.error打印另一句字符串 |
| `cn.hutool.core.lang.Opt` | `Opt<T> of(T value)` | 返回一个包裹里元素不可能为空的Opt |
| `cn.hutool.core.lang.Opt` | `Opt<T> ofBlankAble(T value)` | 返回一个包裹里元素可能为空的Opt，额外判断了空字符串的情况 |
| `cn.hutool.core.lang.Opt` | `Opt<T> ofNullable(T value)` | 返回一个包裹里元素可能为空的Opt |
| `cn.hutool.core.lang.Opt` | `Opt<T> ofTry(Func0<T> supplier)` | @param supplier 操作 |
| `cn.hutool.core.lang.Opt` | `Opt<T> or(Supplier<? extends Opt<? extends T>> supplier)` | 如果包裹里元素的值存在，就返回本身，如果不存在，则使用传入的操作执行后获得的 Opt |
| `cn.hutool.core.lang.Opt` | `Opt<T> peek(Consumer<T> action)` | 如果包裹里元素的值存在，就执行对应的操作，并返回本身 如果不存在，返回一个空的Opt 属于 #ifPresent的链式拓展 |
| `cn.hutool.core.lang.Opt` | `Opt<T> peeks(Consumer<T>... actions)` | 如果包裹里元素的值存在，就执行对应的操作集，并返回本身 如果不存在，返回一个空的Opt 属于 #ifPresent的链式拓展 属于 #peek(Consumer)的动态拓展 |
| `cn.hutool.core.lang.Opt` | `Opt<U> flatMap(Function<? super T, ? extends Opt<? extends U>> mapper)` | 如果包裹里的值存在，就执行传入的操作(Function#apply)并返回该操作返回值 如果不存在，返回一个空的Opt 和 Opt#map的区别为 传入的操作返回值必须为 Opt |
| `cn.hutool.core.lang.Opt` | `Opt<U> flattedMap(Function<? super T, ? extends Optional<? extends U>> mapper)` | 如果包裹里的值存在，就执行传入的操作(Function#apply)并返回该操作返回值 如果不存在，返回一个空的Opt 和 Opt#map的区别为 传入的操作返回值必须为 Optional |
| `cn.hutool.core.lang.Opt` | `Opt<U> map(Function<? super T, ? extends U> mapper)` | 如果包裹里的值存在，就执行传入的操作(Function#apply)并返回一个包裹了该操作返回值的Opt 如果不存在，返回一个空的Opt |
| `cn.hutool.core.lang.Opt` | `Opt<U> mapOrElse(Function<? super T, ? extends U> mapper,VoidFunc0 emptyAction)` | 如果包裹里的值存在，就执行传入的值存在时的操作(Function#apply(Object))支持链式调用、转换为其他类型 否则执行传入的值不存在时的操作(VoidFunc0中的VoidFunc0#call()) 如果值存在就转换为大写，否则用Console.error打印另一句字符串 |
| `cn.hutool.core.lang.Opt` | `Optional<T> toOptional()` | 转换为 Optional对象 |
| `cn.hutool.core.lang.Opt` | `Stream<T> stream()` | 如果包裹里元素的值存在，就返回一个包含该元素的 Stream, 否则返回一个空元素的 Stream 该方法能将 Opt 中的元素传递给 Stream |
| `cn.hutool.core.lang.Opt` | `String toString()` | 返回包裹内元素调用toString()的结果，不存在则返回null |
| `cn.hutool.core.lang.Opt` | `T exceptionOrElse(T other)` | 异常则返回另一个可选值 |
| `cn.hutool.core.lang.Opt` | `T get()` | 返回包裹里的元素，取不到则为null，注意！！！此处和java.util.Optional#get()不同的一点是本方法并不会抛出NoSuchElementException 如果元素为空，则返回null，如果需要一个绝对不能为null的值，则使用#orElseThrow() 如果需要一个绝对不能为 null的值，则使用#orElseThrow() 做此处修改的原因是，有时候我们确实需要返回一个null给前端，并且这样的时候并不少见 而使用 .orElse(null)需要写整整12个字符，用.get()就只需要6个啦 |
| `cn.hutool.core.lang.Opt` | `T orElse(T other)` | 如果包裹里元素的值存在，则返回该值，否则返回传入的other |
| `cn.hutool.core.lang.Opt` | `T orElseGet(Supplier<? extends T> supplier)` | 如果包裹里元素的值存在，则返回该值，否则返回传入的操作执行后的返回值 |
| `cn.hutool.core.lang.Opt` | `T orElseThrow()` | 如果包裹里的值存在，则返回该值，否则抛出 NoSuchElementException |
| `cn.hutool.core.lang.Opt` | `T orElseThrow(Function<String, ? extends X> exceptionFunction,String message)` | 如果包裹里的值存在，则返回该值，否则执行传入的操作，获取异常类型的返回值并抛出 往往是一个包含 自定义消息 构造器的异常 例如 |
| `cn.hutool.core.lang.Opt` | `T orElseThrow(Supplier<? extends X> exceptionSupplier)` | 如果包裹里的值存在，则返回该值，否则执行传入的操作，获取异常类型的返回值并抛出 往往是一个包含无参构造器的异常 例如传入IllegalStateException::new |
| `cn.hutool.core.lang.Opt` | `boolean equals(Object obj)` | 判断传入参数是否与 Opt相等 在以下情况下返回true 它也是一个 Opt 并且 它们包裹住的元素都为空 或者 它们包裹住的元素之间相互 equals() |
| `cn.hutool.core.lang.Opt` | `boolean isEmpty()` | 判断包裹里元素的值是否不存在，不存在为 true，否则为false |
| `cn.hutool.core.lang.Opt` | `boolean isFail()` | 是否失败 当调用 #ofTry(Func0)时，抛出异常则表示失败 |
| `cn.hutool.core.lang.Opt` | `boolean isPresent()` | 判断包裹里元素的值是否存在，存在为 true，否则为false |
| `cn.hutool.core.lang.Opt` | `int hashCode()` | 如果包裹内元素为空，则返回0，否则返回元素的 hashcode |
| `cn.hutool.core.lang.Pair` | `K getKey()` | 获取键 |
| `cn.hutool.core.lang.Pair` | `Pair<K, V> of(K key,V value)` | 构建Pair对象 |
| `cn.hutool.core.lang.Pair` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Pair` | `V getValue()` | 获取值 |
| `cn.hutool.core.lang.Pair` | `boolean equals(Object o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Pair` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.ParameterizedTypeImpl` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.ParameterizedTypeImpl` | `Type getOwnerType()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.ParameterizedTypeImpl` | `Type getRawType()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.ParameterizedTypeImpl` | `Type[] getActualTypeArguments()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.PatternPool` | `Pattern get(String regex)` | 先从Pattern池中查找正则对应的Pattern，找不到则编译正则表达式并入池。 |
| `cn.hutool.core.lang.PatternPool` | `Pattern get(String regex,int flags)` | 先从Pattern池中查找正则对应的Pattern，找不到则编译正则表达式并入池。 |
| `cn.hutool.core.lang.PatternPool` | `Pattern remove(String regex,int flags)` | 移除缓存 |
| `cn.hutool.core.lang.PatternPool` | `void clear()` | 清空缓存池 |
| `cn.hutool.core.lang.Pid` | `int get()` | 获取PID值 |
| `cn.hutool.core.lang.Range` | `Iterator<T> iterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Range` | `Range<T> disableLock()` | 禁用锁，调用此方法后不再使用锁保护 |
| `cn.hutool.core.lang.Range` | `Range<T> reset()` | 重置Range |
| `cn.hutool.core.lang.Range` | `T next()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Range` | `boolean hasNext()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Range` | `void remove()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Range$Stepper` | `T step(T current,T end,int index)` | 增加步进 增加步进后的返回值如果为null则表示步进结束 用户需根据end参数自行定义边界，当达到边界时返回null表示结束，否则Range中边界对象无效，会导致无限循环 |
| `cn.hutool.core.lang.Replacer` | `T replace(T t)` | 替换指定类型为目标类型 |
| `cn.hutool.core.lang.ResourceClassLoader` | `ResourceClassLoader<T> addResource(T resource)` | 增加需要加载的类资源 |
| `cn.hutool.core.lang.Segment` | `T getEndIndex()` | 获取结束位置 |
| `cn.hutool.core.lang.Segment` | `T getStartIndex()` | 获取起始位置 |
| `cn.hutool.core.lang.Segment` | `T length()` | 片段长度，默认计算方法为abs(#getEndIndex() - #getEndIndex()) |
| `cn.hutool.core.lang.SimpleCache` | `Iterator<Map.Entry<K, V>> iterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.SimpleCache` | `V get(K key)` | 从缓存池中查找值 |
| `cn.hutool.core.lang.SimpleCache` | `V get(K key,Func0<V> supplier)` | 从缓存中获得对象，当对象不在缓存中或已经过期返回Func0回调产生的对象 |
| `cn.hutool.core.lang.SimpleCache` | `V get(K key,Predicate<V> validPredicate,Func0<V> supplier)` | 从缓存中获得对象，当对象不在缓存中或已经过期返回Func0回调产生的对象 |
| `cn.hutool.core.lang.SimpleCache` | `V put(K key,V value)` | 放入缓存 |
| `cn.hutool.core.lang.SimpleCache` | `V remove(K key)` | 移除缓存 |
| `cn.hutool.core.lang.SimpleCache` | `void clear()` | 清空缓存池 |
| `cn.hutool.core.lang.Singleton` | `Set<Class<?>> getExistClass()` | 获取单例池中存在的所有类 |
| `cn.hutool.core.lang.Singleton` | `T get(Class<T> clazz,Object... params)` | 获得指定类的单例对象 对象存在于池中返回，否则创建，每次调用此方法获得的对象为同一个对象 注意：单例针对的是类和参数，也就是说只有类、参数一致才会返回同一个对象 |
| `cn.hutool.core.lang.Singleton` | `T get(String className,Object... params)` | 获得指定类的单例对象 对象存在于池中返回，否则创建，每次调用此方法获得的对象为同一个对象 |
| `cn.hutool.core.lang.Singleton` | `T get(String key,Func0<T> supplier)` | 获得指定类的单例对象 对象存在于池中返回，否则创建，每次调用此方法获得的对象为同一个对象 |
| `cn.hutool.core.lang.Singleton` | `boolean exists(Class<?> clazz,Object... params)` | 判断某个类的对象是否存在 |
| `cn.hutool.core.lang.Singleton` | `void destroy()` | 清除所有Singleton对象 |
| `cn.hutool.core.lang.Singleton` | `void put(Object obj)` | 将已有对象放入单例中，其Class做为键 |
| `cn.hutool.core.lang.Singleton` | `void put(String key,Object obj)` | 将已有对象放入单例中，key做为键 |
| `cn.hutool.core.lang.Singleton` | `void remove(Class<?> clazz)` | 移除指定Singleton对象 |
| `cn.hutool.core.lang.Singleton` | `void remove(String key)` | 移除指定Singleton对象 |
| `cn.hutool.core.lang.Snowflake` | `Pair<Long, Long> getIdScopeByTimestamp(long timestampStart,long timestampEnd)` | 根据传入时间戳-计算ID起终点 |
| `cn.hutool.core.lang.Snowflake` | `Pair<Long, Long> getIdScopeByTimestamp(long timestampStart,long timestampEnd,boolean ignoreCenterAndWorker)` | 根据传入时间戳-计算ID起终点 Gitee/issues/I60M14 |
| `cn.hutool.core.lang.Snowflake` | `String nextIdStr()` | 下一个ID（字符串形式） |
| `cn.hutool.core.lang.Snowflake` | `long getDataCenterId(long id)` | 根据Snowflake的ID，获取数据中心id |
| `cn.hutool.core.lang.Snowflake` | `long getGenerateDateTime(long id)` | 根据Snowflake的ID，获取生成时间 |
| `cn.hutool.core.lang.Snowflake` | `long getWorkerId(long id)` | 根据Snowflake的ID，获取机器id |
| `cn.hutool.core.lang.Snowflake` | `long nextId()` | 下一个ID |
| `cn.hutool.core.lang.Tuple` | `Iterator<Object> iterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Tuple` | `List<Object> toList()` | 将元组转换成列表 |
| `cn.hutool.core.lang.Tuple` | `Object[] getMembers()` | 获得所有元素 |
| `cn.hutool.core.lang.Tuple` | `Spliterator<Object> spliterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Tuple` | `Stream<Object> parallelStream()` | 将元组转成并行流 |
| `cn.hutool.core.lang.Tuple` | `Stream<Object> stream()` | 将元组转成流 |
| `cn.hutool.core.lang.Tuple` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Tuple` | `T get(int index)` | 获取指定位置元素 |
| `cn.hutool.core.lang.Tuple` | `Tuple setCacheHash(boolean cacheHash)` | 缓存Hash值，当为true时，此对象的hash值只被计算一次，常用于Tuple中的值不变时使用。 注意：当为true时，member变更对象后，hash值不会变更。 |
| `cn.hutool.core.lang.Tuple` | `Tuple sub(final int start,final int end)` | 截取元组指定部分 |
| `cn.hutool.core.lang.Tuple` | `boolean contains(Object value)` | 判断元组中是否包含某元素 |
| `cn.hutool.core.lang.Tuple` | `boolean equals(Object obj)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Tuple` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Tuple` | `int size()` | 得到元组的大小 |
| `cn.hutool.core.lang.TypeReference` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.TypeReference` | `Type getType()` | 获取用户定义的泛型参数 |
| `cn.hutool.core.lang.UUID` | `String toString()` | 返回此UUID 的字符串表现形式。 UUID 的字符串表示形式由此 BNF 描述： |
| `cn.hutool.core.lang.UUID` | `String toString(boolean isSimple)` | 返回此UUID 的字符串表现形式。 UUID 的字符串表示形式由此 BNF 描述： |
| `cn.hutool.core.lang.UUID` | `UUID fastUUID()` | 获取类型 4（伪随机生成的）UUID 的静态工厂。 使用加密的本地线程伪随机数生成器生成该 UUID。 |
| `cn.hutool.core.lang.UUID` | `UUID fromString(String name)` | 根据 #toString() 方法中描述的字符串标准表示形式创建UUID。 |
| `cn.hutool.core.lang.UUID` | `UUID nameUUIDFromBytes(byte[] name)` | 根据指定的字节数组获取类型 3（基于名称的）UUID 的静态工厂。 |
| `cn.hutool.core.lang.UUID` | `UUID randomUUID()` | 获取类型 4（伪随机生成的）UUID 的静态工厂。 使用加密的强伪随机数生成器生成该 UUID。 |
| `cn.hutool.core.lang.UUID` | `UUID randomUUID(boolean isSecure)` | 获取类型 4（伪随机生成的）UUID 的静态工厂。 使用加密的强伪随机数生成器生成该 UUID。 |
| `cn.hutool.core.lang.UUID` | `boolean equals(Object obj)` | 将此对象与指定对象比较。 当且仅当参数不为 null、而是一个 UUID 对象、具有与此 UUID 相同的 varriant、包含相同的值（每一位均相同）时，结果才为 true。 |
| `cn.hutool.core.lang.UUID` | `int clockSequence()` | 与此 UUID 相关联的时钟序列值。 14 位的时钟序列值根据此 UUID 的 clock_seq 字段构造。clock_seq 字段用于保证在基于时间的 UUID 中的时间唯一性。 clockSequence 值仅在基于时间的 UUID（其 version 类型为 1）中才有意义。 如果此 UUID 不是基于时间的 UUID，则此方法抛出 UnsupportedOperationException。 |
| `cn.hutool.core.lang.UUID` | `int compareTo(UUID val)` | 将此 UUID 与指定的 UUID 比较。 如果两个 UUID 不同，且第一个 UUID 的最高有效字段大于第二个 UUID 的对应字段，则第一个 UUID 大于第二个 UUID。 |
| `cn.hutool.core.lang.UUID` | `int hashCode()` | 返回此 UUID 的哈希码。 |
| `cn.hutool.core.lang.UUID` | `int variant()` | 与此 UUID 相关联的变体号。变体号描述 UUID 的布局。 变体号具有以下含意： 0 为 NCS 向后兼容保留 2 IETF RFC 4122 (Leach-Salz), 用于此类 6 保留，微软向后兼容 7 保留供以后定义使用 |
| `cn.hutool.core.lang.UUID` | `int version()` | 与此 UUID 相关联的版本号. 版本号描述此 UUID 是如何生成的。 版本号具有以下含意: 1 基于时间的 UUID 2 DCE 安全 UUID 3 基于名称的 UUID 4 随机生成的 UUID |
| `cn.hutool.core.lang.UUID` | `long getLeastSignificantBits()` | 返回此 UUID 的 128 位值中的最低有效 64 位。 |
| `cn.hutool.core.lang.UUID` | `long getMostSignificantBits()` | 返回此 UUID 的 128 位值中的最高有效 64 位。 |
| `cn.hutool.core.lang.UUID` | `long node()` | 与此 UUID 相关的节点值。 48 位的节点值根据此 UUID 的 node 字段构造。此字段旨在用于保存机器的 IEEE 802 地址，该地址用于生成此 UUID 以保证空间唯一性。 节点值仅在基于时间的 UUID（其 version 类型为 1）中才有意义。 如果此 UUID 不是基于时间的 UUID，则此方法抛出 UnsupportedOperationException。 |
| `cn.hutool.core.lang.UUID` | `long timestamp()` | 与此 UUID 相关联的时间戳值。 60 位的时间戳值根据此 UUID 的 time_low、time_mid 和 time_hi 字段构造。 所得到的时间戳以 100 毫微秒为单位，从 UTC（通用协调时间） 1582 年 10 月 15 日零时开始。 时间戳值仅在在基于时间的 UUID（其 version 类型为 1）中才有意义。 如果此 UUID 不是基于时间的 UUID，则此方法抛出 UnsupportedOperationException。 |
| `cn.hutool.core.lang.Validator` | `Object validateEqual(Object t1,Object t2,String errorMsg)` | 验证是否相等，不相等抛出异常 |
| `cn.hutool.core.lang.Validator` | `String validateNumber(String value,String errorMsg)` | 验证是否为数字 |
| `cn.hutool.core.lang.Validator` | `T validateBirthday(T value,String errorMsg)` | 验证验证是否为生日 |
| `cn.hutool.core.lang.Validator` | `T validateCarDrivingLicence(T value,String errorMsg)` | 验证是否为驾驶证 别名：驾驶证档案编号、行驶证编号 |
| `cn.hutool.core.lang.Validator` | `T validateCarVin(T value,String errorMsg)` | 验证是否为车架号；别名：行驶证编号 车辆识别代号 车辆识别码 |
| `cn.hutool.core.lang.Validator` | `T validateChinese(T value,String errorMsg)` | 验证是否为汉字 |
| `cn.hutool.core.lang.Validator` | `T validateCitizenIdNumber(T value,String errorMsg)` | 验证是否为身份证号码（支持18位、15位和港澳台的10位） |
| `cn.hutool.core.lang.Validator` | `T validateEmail(T value,String errorMsg)` | 验证是否为可用邮箱地址 |
| `cn.hutool.core.lang.Validator` | `T validateEmpty(T value,String errorMsg)` | 验证是否为空，非空时抛出异常 对于String类型判定是否为empty(null 或 "") |
| `cn.hutool.core.lang.Validator` | `T validateGeneral(T value,String errorMsg)` | 验证是否为英文字母 、数字和下划线 |
| `cn.hutool.core.lang.Validator` | `T validateGeneral(T value,int min,String errorMsg)` | 验证是否为给定最小长度的英文字母 、数字和下划线 |
| `cn.hutool.core.lang.Validator` | `T validateGeneral(T value,int min,int max,String errorMsg)` | 验证是否为给定长度范围的英文字母 、数字和下划线 |
| `cn.hutool.core.lang.Validator` | `T validateGeneralWithChinese(T value,String errorMsg)` | 验证是否为中文字、英文字母、数字和下划线 |
| `cn.hutool.core.lang.Validator` | `T validateHex(T value,String errorMsg)` | 验证是否为Hex（16进制）字符串 |
| `cn.hutool.core.lang.Validator` | `T validateIpv4(T value,String errorMsg)` | 验证是否为IPV4地址 |
| `cn.hutool.core.lang.Validator` | `T validateIpv6(T value,String errorMsg)` | 验证是否为IPV6地址 |
| `cn.hutool.core.lang.Validator` | `T validateLetter(T value,String errorMsg)` | 验证是否全部为字母组成，包括大写和小写字母和汉字 |
| `cn.hutool.core.lang.Validator` | `T validateLowerCase(T value,String errorMsg)` | 验证字符串是否全部为小写字母 |
| `cn.hutool.core.lang.Validator` | `T validateMac(T value,String errorMsg)` | 验证是否为MAC地址 |
| `cn.hutool.core.lang.Validator` | `T validateMatchRegex(String regex,T value,String errorMsg)` | 通过正则表达式验证 不符合正则抛出ValidateException 异常 |
| `cn.hutool.core.lang.Validator` | `T validateMobile(T value,String errorMsg)` | 验证是否为手机号码（中国） |
| `cn.hutool.core.lang.Validator` | `T validateMoney(T value,String errorMsg)` | 验证是否为货币 |
| `cn.hutool.core.lang.Validator` | `T validateNotEmpty(T value,String errorMsg)` | 验证是否为非空，为空时抛出异常 对于String类型判定是否为empty(null 或 "") |
| `cn.hutool.core.lang.Validator` | `T validateNotNull(T value,String errorMsgTemplate,Object... params)` | 检查指定值是否非null |
| `cn.hutool.core.lang.Validator` | `T validateNull(T value,String errorMsgTemplate,Object... params)` | 检查指定值是否为null |
| `cn.hutool.core.lang.Validator` | `T validatePlateNumber(T value,String errorMsg)` | 验证是否为中国车牌号 |
| `cn.hutool.core.lang.Validator` | `T validateUUID(T value,String errorMsg)` | 验证是否为UUID 包括带横线标准格式和不带横线的简单模式 |
| `cn.hutool.core.lang.Validator` | `T validateUpperCase(T value,String errorMsg)` | 验证字符串是否全部为大写字母 |
| `cn.hutool.core.lang.Validator` | `T validateUrl(T value,String errorMsg)` | 验证是否为URL |
| `cn.hutool.core.lang.Validator` | `T validateWord(T value,String errorMsg)` | 验证是否为字母（包括大写和小写字母） |
| `cn.hutool.core.lang.Validator` | `T validateZipCode(T value,String errorMsg)` | 验证是否为邮政编码（中国） |
| `cn.hutool.core.lang.Validator` | `boolean equal(Object t1,Object t2)` | 验证是否相等 当两值都为null返回true |
| `cn.hutool.core.lang.Validator` | `boolean hasChinese(CharSequence value)` | 验证是否包含汉字 |
| `cn.hutool.core.lang.Validator` | `boolean hasNumber(CharSequence value)` | 是否包含数字 |
| `cn.hutool.core.lang.Validator` | `boolean isBetween(Number value,Number min,Number max)` | 检查给定的数字是否在指定范围内 |
| `cn.hutool.core.lang.Validator` | `boolean isBirthday(CharSequence value)` | 验证是否为生日 只支持以下几种格式： yyyyMMdd yyyy-MM-dd yyyy/MM/dd yyyy.MM.dd yyyy年MM月dd日 |
| `cn.hutool.core.lang.Validator` | `boolean isBirthday(int year,int month,int day)` | 验证是否为生日 |
| `cn.hutool.core.lang.Validator` | `boolean isCarDrivingLicence(CharSequence value)` | 验证是否为驾驶证 别名：驾驶证档案编号、行驶证编号 仅限：中国驾驶证档案编号 |
| `cn.hutool.core.lang.Validator` | `boolean isCarVin(CharSequence value)` | 验证是否为车架号；别名：行驶证编号 车辆识别代号 车辆识别码 |
| `cn.hutool.core.lang.Validator` | `boolean isChinese(CharSequence value)` | 验证是否都为汉字 |
| `cn.hutool.core.lang.Validator` | `boolean isChineseName(CharSequence value)` | 是否是中文姓名 维吾尔族姓名里面的点是 · 输入法中文状态下，键盘左上角数字1前面的那个符号； 错误字符：．.。．. 正确维吾尔族姓名： |
| `cn.hutool.core.lang.Validator` | `boolean isCitizenId(CharSequence value)` | 验证是否为身份证号码（支持18位、15位和港澳台的10位） |
| `cn.hutool.core.lang.Validator` | `boolean isCreditCode(CharSequence creditCode)` | 是否是有效的统一社会信用代码 |
| `cn.hutool.core.lang.Validator` | `boolean isEmail(CharSequence value)` | 验证是否为可用邮箱地址 |
| `cn.hutool.core.lang.Validator` | `boolean isEmail(CharSequence value,boolean includChinese)` | 验证是否为可用邮箱地址（兼容中文邮箱地址） |
| `cn.hutool.core.lang.Validator` | `boolean isEmpty(Object value)` | 验证是否为空 对于String类型判定是否为empty(null 或 "") |
| `cn.hutool.core.lang.Validator` | `boolean isFalse(boolean value)` | 给定值是否不为false |
| `cn.hutool.core.lang.Validator` | `boolean isGeneral(CharSequence value)` | 验证是否为英文字母 、数字和下划线 |
| `cn.hutool.core.lang.Validator` | `boolean isGeneral(CharSequence value,int min)` | 验证是否为给定最小长度的英文字母 、数字和下划线 |
| `cn.hutool.core.lang.Validator` | `boolean isGeneral(CharSequence value,int min,int max)` | 验证是否为给定长度范围的英文字母 、数字和下划线 |
| `cn.hutool.core.lang.Validator` | `boolean isGeneralWithChinese(CharSequence value)` | 验证是否为中文字、英文字母、数字和下划线 |
| `cn.hutool.core.lang.Validator` | `boolean isHex(CharSequence value)` | 验证是否为Hex（16进制）字符串 |
| `cn.hutool.core.lang.Validator` | `boolean isIpv4(CharSequence value)` | 验证是否为IPV4地址 |
| `cn.hutool.core.lang.Validator` | `boolean isIpv6(CharSequence value)` | 验证是否为IPV6地址 |
| `cn.hutool.core.lang.Validator` | `boolean isLetter(CharSequence value)` | 判断字符串是否全部为字母组成，包括大写和小写字母和汉字 |
| `cn.hutool.core.lang.Validator` | `boolean isLowerCase(CharSequence value)` | 判断字符串是否全部为小写字母 |
| `cn.hutool.core.lang.Validator` | `boolean isMac(CharSequence value)` | 验证是否为MAC地址 |
| `cn.hutool.core.lang.Validator` | `boolean isMatchRegex(Pattern pattern,CharSequence value)` | 通过正则表达式验证 |
| `cn.hutool.core.lang.Validator` | `boolean isMatchRegex(String regex,CharSequence value)` | 通过正则表达式验证 |
| `cn.hutool.core.lang.Validator` | `boolean isMobile(CharSequence value)` | 验证是否为手机号码（中国） |
| `cn.hutool.core.lang.Validator` | `boolean isMoney(CharSequence value)` | 验证是否为货币 |
| `cn.hutool.core.lang.Validator` | `boolean isNotEmpty(Object value)` | 验证是否为非空 对于String类型判定是否为empty(null 或 "") |
| `cn.hutool.core.lang.Validator` | `boolean isNotNull(Object value)` | 给定值是否不为null |
| `cn.hutool.core.lang.Validator` | `boolean isNull(Object value)` | 给定值是否为null |
| `cn.hutool.core.lang.Validator` | `boolean isNumber(CharSequence value)` | 验证该字符串是否是数字 |
| `cn.hutool.core.lang.Validator` | `boolean isPlateNumber(CharSequence value)` | 验证是否为中国车牌号 |
| `cn.hutool.core.lang.Validator` | `boolean isTrue(boolean value)` | 给定值是否为true |
| `cn.hutool.core.lang.Validator` | `boolean isUUID(CharSequence value)` | 验证是否为UUID 包括带横线标准格式和不带横线的简单模式 |
| `cn.hutool.core.lang.Validator` | `boolean isUpperCase(CharSequence value)` | 判断字符串是否全部为大写字母 |
| `cn.hutool.core.lang.Validator` | `boolean isUrl(CharSequence value)` | 验证是否为URL |
| `cn.hutool.core.lang.Validator` | `boolean isWord(CharSequence value)` | 验证该字符串是否是字母（包括大写和小写字母） |
| `cn.hutool.core.lang.Validator` | `boolean isZipCode(CharSequence value)` | 验证是否为邮政编码（中国） |
| `cn.hutool.core.lang.Validator` | `boolean validateFalse(boolean value,String errorMsgTemplate,Object... params)` | 检查指定值是否为false |
| `cn.hutool.core.lang.Validator` | `boolean validateTrue(boolean value,String errorMsgTemplate,Object... params)` | 检查指定值是否为true |
| `cn.hutool.core.lang.Validator` | `void checkIndexLimit(final int index,final int size)` | 检查给定的index是否超出长度限制，默认检查超出倍数（10倍），此方法主要用于内部，检查包括： 数组调用setOrPadding时，最多允许padding的长度 List调用setOrPadding时，最多允许padding的长度 JSONArray调用setOrPadding时，最多允许padding的长度 |
| `cn.hutool.core.lang.Validator` | `void validateBetween(Number value,Number min,Number max,String errorMsg)` | 检查给定的数字是否在指定范围内 |
| `cn.hutool.core.lang.Validator` | `void validateNotEmptyAndEqual(Object t1,Object t2,String errorMsg)` | 验证是否非空且与指定值相等 当数据为空时抛出验证异常 当两值不等时抛出异常 |
| `cn.hutool.core.lang.Validator` | `void validateNotEmptyAndNotEqual(Object t1,Object t2,String errorMsg)` | 验证是否非空且与指定值相等 当数据为空时抛出验证异常 当两值相等时抛出异常 |
| `cn.hutool.core.lang.Validator` | `void validateNotEqual(Object t1,Object t2,String errorMsg)` | 验证是否不等，相等抛出异常 |
| `cn.hutool.core.lang.Version` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Version` | `Version of(final String v)` | 解析版本字符串为Version对象 |
| `cn.hutool.core.lang.Version` | `boolean equals(final Object ob)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Version` | `int compareTo(final Version that)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.Version` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.WeightListRandom` | `E next()` | 随机出一个元素 |
| `cn.hutool.core.lang.WeightListRandom` | `E randomByWeight(double weight)` | 按照给定的总权重随机出一个元素 |
| `cn.hutool.core.lang.WeightListRandom` | `boolean isEmpty()` | 判断随机池是否为空 |
| `cn.hutool.core.lang.WeightListRandom` | `boolean remove(E e)` | 移除元素 |
| `cn.hutool.core.lang.WeightListRandom` | `void add(E e,double weight)` | 添加元素 |
| `cn.hutool.core.lang.WeightRandom` | `T next()` | 下一个随机对象 |
| `cn.hutool.core.lang.WeightRandom` | `WeightRandom<T> add(T obj,double weight)` | 增加对象 |
| `cn.hutool.core.lang.WeightRandom` | `WeightRandom<T> add(WeightObj<T> weightObj)` | 增加对象权重 |
| `cn.hutool.core.lang.WeightRandom` | `WeightRandom<T> clear()` | 清空权重表 |
| `cn.hutool.core.lang.WeightRandom` | `WeightRandom<T> create()` | 创建权重随机获取器 |
| `cn.hutool.core.lang.WeightRandom$WeightObj` | `T getObj()` | 获取对象 |
| `cn.hutool.core.lang.WeightRandom$WeightObj` | `boolean equals(Object obj)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.WeightRandom$WeightObj` | `double getWeight()` | 获取权重 |
| `cn.hutool.core.lang.WeightRandom$WeightObj` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.WeightRandom$WeightObj` | `void setObj(T obj)` | 设置对象 |
