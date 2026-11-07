# cn.hutool.core.bean

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.bean.BeanDesc` | `Collection<PropDesc> getProps()` | 获取字段属性列表 |
| `cn.hutool.core.bean.BeanDesc` | `Field getField(String fieldName)` | 获得字段名对应的字段对象，如果不存在返回null |
| `cn.hutool.core.bean.BeanDesc` | `Map<String, PropDesc> getPropMap(boolean ignoreCase)` | 获取字段名-字段属性Map |
| `cn.hutool.core.bean.BeanDesc` | `Method getGetter(String fieldName)` | 获取Getter方法，如果不存在返回null |
| `cn.hutool.core.bean.BeanDesc` | `Method getSetter(String fieldName)` | 获取Setter方法，如果不存在返回null |
| `cn.hutool.core.bean.BeanDesc` | `PropDesc getProp(String fieldName)` | 获取属性，如果不存在返回null |
| `cn.hutool.core.bean.BeanDesc` | `String getName()` | 获取Bean的全类名 |
| `cn.hutool.core.bean.BeanDesc` | `String getSimpleName()` | 获取Bean的简单类名 |
| `cn.hutool.core.bean.BeanDescCache` | `BeanDesc getBeanDesc(Class<?> beanClass,Func0<BeanDesc> supplier)` | 获得属性名和BeanDescMap映射 |
| `cn.hutool.core.bean.BeanDescCache` | `void clear()` | 清空全局的Bean属性缓存 |
| `cn.hutool.core.bean.BeanInfoCache` | `Map<String, PropertyDescriptor> getPropertyDescriptorMap(Class<?> beanClass,boolean ignoreCase)` | 获得属性名和PropertyDescriptorMap映射 |
| `cn.hutool.core.bean.BeanInfoCache` | `Map<String, PropertyDescriptor> getPropertyDescriptorMap(Class<?> beanClass,boolean ignoreCase,Func0<Map<String, PropertyDescriptor>> supplier)` | 获得属性名和PropertyDescriptorMap映射 |
| `cn.hutool.core.bean.BeanInfoCache` | `void clear()` | 清空缓存 |
| `cn.hutool.core.bean.BeanInfoCache` | `void putPropertyDescriptorMap(Class<?> beanClass,Map<String, PropertyDescriptor> fieldNamePropertyDescriptorMap,boolean ignoreCase)` | 加入缓存 |
| `cn.hutool.core.bean.BeanPath` | `BeanPath create(final String expression)` | 解析Bean路径表达式为Bean模式 Bean表达式，用于获取多层嵌套Bean中的字段值或Bean对象 根据给定的表达式，查找Bean中对应的属性值对象。 表达式分为两种： .表达式，可以获取Bean对象中的属性（字段）值或者Map中key对应的值 []表达式，可以获取集合等对象中对应index的值 表达式栗子： |
| `cn.hutool.core.bean.BeanPath` | `List<String> getPatternParts()` | 获取表达式解析后的分段列表 |
| `cn.hutool.core.bean.BeanPath` | `Object get(final Object bean)` | 获取Bean中对应表达式的值 |
| `cn.hutool.core.bean.BeanPath` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.bean.BeanPath` | `void set(final Object bean,final Object value)` | 设置表达式指定位置（或filed对应）的值 若表达式指向一个List则设置其坐标对应位置的值，若指向Map则put对应key的值，Bean则设置字段的值 注意： |
| `cn.hutool.core.bean.BeanUtil` | `BeanDesc getBeanDesc(Class<?> clazz)` | 获取BeanDesc Bean描述信息 |
| `cn.hutool.core.bean.BeanUtil` | `DynaBean createDynaBean(Object bean)` | 创建动态Bean |
| `cn.hutool.core.bean.BeanUtil` | `List<T> copyToList(Collection<?> collection,Class<T> targetType)` | 复制集合中的Bean属性 此方法遍历集合中每个Bean，复制其属性后加入一个新的List中。 |
| `cn.hutool.core.bean.BeanUtil` | `List<T> copyToList(Collection<?> collection,Class<T> targetType,CopyOptions copyOptions)` | 复制集合中的Bean属性 此方法遍历集合中每个Bean，复制其属性后加入一个新的List中。 |
| `cn.hutool.core.bean.BeanUtil` | `Map<String, Object> beanToMap(Object bean,Map<String, Object> targetMap,CopyOptions copyOptions)` | 对象转Map 通过自定义CopyOptions 完成抓换选项，以便实现： |
| `cn.hutool.core.bean.BeanUtil` | `Map<String, Object> beanToMap(Object bean,Map<String, Object> targetMap,boolean ignoreNullValue,Editor<String> keyEditor)` | 对象转Map 通过实现Editor 可以自定义字段值，如果这个Editor返回null则忽略这个字段，以便实现： |
| `cn.hutool.core.bean.BeanUtil` | `Map<String, Object> beanToMap(Object bean,Map<String, Object> targetMap,final boolean isToUnderlineCase,boolean ignoreNullValue)` | 对象转Map |
| `cn.hutool.core.bean.BeanUtil` | `Map<String, Object> beanToMap(Object bean,String... properties)` | 将bean的部分属性转换成map 可选拷贝哪些属性值，默认是不忽略值为null的值的。 |
| `cn.hutool.core.bean.BeanUtil` | `Map<String, Object> beanToMap(Object bean,boolean isToUnderlineCase,boolean ignoreNullValue)` | 对象转Map |
| `cn.hutool.core.bean.BeanUtil` | `Map<String, PropertyDescriptor> getPropertyDescriptorMap(Class<?> clazz,boolean ignoreCase)` | 获得字段名和字段描述Map，获得的结果会缓存在 BeanInfoCache中 |
| `cn.hutool.core.bean.BeanUtil` | `Object getFieldValue(Object bean,String fieldNameOrIndex)` | 获得字段值，通过反射直接获得字段值，并不调用getXXX方法 对象同样支持Map类型，fieldNameOrIndex即为key Map: fieldNameOrIndex需为key，获取对应value Collection: fieldNameOrIndex当为数字，返回index对应值，非数字遍历集合返回子bean对应name值 Array: fieldNameOrIndex当为数字，返回index对应值，非数字遍历数组返回子bean对应name值 |
| `cn.hutool.core.bean.BeanUtil` | `Object setFieldValue(Object bean,String fieldNameOrIndex,Object value)` | 设置字段值，通过反射设置字段值，并不调用setXXX方法 对象同样支持Map类型，fieldNameOrIndex即为key，支持： Map List Bean |
| `cn.hutool.core.bean.BeanUtil` | `PropertyDescriptor getPropertyDescriptor(Class<?> clazz,final String fieldName)` | 获得Bean类属性描述，大小写敏感 |
| `cn.hutool.core.bean.BeanUtil` | `PropertyDescriptor getPropertyDescriptor(Class<?> clazz,final String fieldName,boolean ignoreCase)` | 获得Bean类属性描述 |
| `cn.hutool.core.bean.BeanUtil` | `PropertyDescriptor[] getPropertyDescriptors(Class<?> clazz)` | 获得Bean字段描述数组 |
| `cn.hutool.core.bean.BeanUtil` | `PropertyEditor findEditor(Class<?> type)` | 查找类型转换器 PropertyEditor |
| `cn.hutool.core.bean.BeanUtil` | `String getFieldName(String getterOrSetterName)` | 获取Getter或Setter方法名对应的字段名称，规则如下： getXxxx获取为xxxx，如getName得到name。 setXxxx获取为xxxx，如setName得到name。 isXxxx获取为xxxx，如isName得到name。 其它不满足规则的方法名抛出IllegalArgumentException |
| `cn.hutool.core.bean.BeanUtil` | `T copyProperties(Object source,Class<T> tClass,String... ignoreProperties)` | 按照Bean对象属性创建对应的Class对象，并忽略某些属性 |
| `cn.hutool.core.bean.BeanUtil` | `T edit(T bean,Editor<Field> editor)` | 编辑Bean的字段，static字段不会处理 例如需要对指定的字段做判空操作、null转""操作等等。 |
| `cn.hutool.core.bean.BeanUtil` | `T fillBean(T bean,ValueProvider<String> valueProvider,CopyOptions copyOptions)` | 填充Bean的核心方法 |
| `cn.hutool.core.bean.BeanUtil` | `T fillBeanWithMap(Map<?, ?> map,T bean,CopyOptions copyOptions)` | 使用Map填充Bean对象 |
| `cn.hutool.core.bean.BeanUtil` | `T fillBeanWithMap(Map<?, ?> map,T bean,boolean isIgnoreError)` | 使用Map填充Bean对象 |
| `cn.hutool.core.bean.BeanUtil` | `T fillBeanWithMap(Map<?, ?> map,T bean,boolean isToCamelCase,CopyOptions copyOptions)` | 使用Map填充Bean对象 |
| `cn.hutool.core.bean.BeanUtil` | `T fillBeanWithMap(Map<?, ?> map,T bean,boolean isToCamelCase,boolean isIgnoreError)` | 使用Map填充Bean对象，可配置将下划线转换为驼峰 |
| `cn.hutool.core.bean.BeanUtil` | `T fillBeanWithMapIgnoreCase(Map<?, ?> map,T bean,boolean isIgnoreError)` | 使用Map填充Bean对象，忽略大小写 |
| `cn.hutool.core.bean.BeanUtil` | `T getProperty(Object bean,String expression)` | 解析Bean中的属性值 |
| `cn.hutool.core.bean.BeanUtil` | `T mapToBean(Map<?, ?> map,Class<T> beanClass,CopyOptions copyOptions)` | Map转换为Bean对象 |
| `cn.hutool.core.bean.BeanUtil` | `T mapToBean(Map<?, ?> map,Class<T> beanClass,boolean isIgnoreError)` | Map转换为Bean对象 |
| `cn.hutool.core.bean.BeanUtil` | `T mapToBean(Map<?, ?> map,Class<T> beanClass,boolean isToCamelCase,CopyOptions copyOptions)` | Map转换为Bean对象 |
| `cn.hutool.core.bean.BeanUtil` | `T mapToBeanIgnoreCase(Map<?, ?> map,Class<T> beanClass,boolean isIgnoreError)` | Map转换为Bean对象 忽略大小写 |
| `cn.hutool.core.bean.BeanUtil` | `T toBean(Class<T> beanClass,ValueProvider<String> valueProvider,CopyOptions copyOptions)` | ServletRequest 参数转Bean |
| `cn.hutool.core.bean.BeanUtil` | `T toBean(Object source,Class<T> clazz)` | 对象或Map转Bean |
| `cn.hutool.core.bean.BeanUtil` | `T toBean(Object source,Class<T> clazz,CopyOptions options)` | 对象或Map转Bean |
| `cn.hutool.core.bean.BeanUtil` | `T toBean(Object source,Supplier<T> targetSupplier,CopyOptions options)` | 对象或Map转Bean |
| `cn.hutool.core.bean.BeanUtil` | `T toBeanIgnoreCase(Object source,Class<T> clazz,boolean ignoreError)` | 对象或Map转Bean，忽略字段转换时发生的异常 |
| `cn.hutool.core.bean.BeanUtil` | `T toBeanIgnoreError(Object source,Class<T> clazz)` | 对象或Map转Bean，忽略字段转换时发生的异常 |
| `cn.hutool.core.bean.BeanUtil` | `T trimStrFields(T bean,String... ignoreFields)` | 把Bean里面的String属性做trim操作。此方法直接对传入的Bean做修改。 通常bean直接用来绑定页面的input，用户的输入可能首尾存在空格，通常保存数据库前需要把首尾空格去掉 |
| `cn.hutool.core.bean.BeanUtil` | `boolean hasGetter(Class<?> clazz)` | 判断是否为Bean对象 判定方法是否存在只有无参数的getXXX方法或者isXXX方法 |
| `cn.hutool.core.bean.BeanUtil` | `boolean hasNullField(Object bean,String... ignoreFieldNames)` | 判断Bean是否包含值为null的属性 对象本身为null也返回true |
| `cn.hutool.core.bean.BeanUtil` | `boolean hasPublicField(Class<?> clazz)` | 指定类中是否有public类型字段(static字段除外) |
| `cn.hutool.core.bean.BeanUtil` | `boolean hasSetter(Class<?> clazz)` | 判断是否有Setter方法 判定方法是否存在只有一个参数的setXXX方法 |
| `cn.hutool.core.bean.BeanUtil` | `boolean isBean(Class<?> clazz)` | 判断是否为Bean对象，判定方法是： |
| `cn.hutool.core.bean.BeanUtil` | `boolean isCommonFieldsEqual(Object source,Object target,String... ignoreProperties)` | 判断source与target的所有公共字段的值是否相同 |
| `cn.hutool.core.bean.BeanUtil` | `boolean isEmpty(Object bean,String... ignoreFieldNames)` | 判断Bean是否为空对象，空对象表示本身为null或者所有属性都为null 此方法不判断static属性 |
| `cn.hutool.core.bean.BeanUtil` | `boolean isMatchName(Object bean,String beanClassName,boolean isSimple)` | 给定的Bean的类名是否匹配指定类名字符串 如果isSimple为true，则只匹配类名而忽略包名，例如：cn.hutool.TestEntity只匹配TestEntity 如果isSimple为false，则匹配包括包名的全类名，例如：cn.hutool.TestEntity匹配cn.hutool.TestEntity |
| `cn.hutool.core.bean.BeanUtil` | `boolean isNotEmpty(Object bean,String... ignoreFieldNames)` | 判断Bean是否为非空对象，非空对象表示本身不为null或者含有非null属性的对象 |
| `cn.hutool.core.bean.BeanUtil` | `boolean isReadableBean(Class<?> clazz)` | 判断是否为可读的Bean对象，判定方法是： |
| `cn.hutool.core.bean.BeanUtil` | `void copyProperties(Object source,Object target,CopyOptions copyOptions)` | 复制Bean对象属性 限制类用于限制拷贝的属性，例如一个类我只想复制其父类的一些属性，就可以将editable设置为父类 |
| `cn.hutool.core.bean.BeanUtil` | `void copyProperties(Object source,Object target,String... ignoreProperties)` | 复制Bean对象属性 限制类用于限制拷贝的属性，例如一个类我只想复制其父类的一些属性，就可以将editable设置为父类 |
| `cn.hutool.core.bean.BeanUtil` | `void copyProperties(Object source,Object target,boolean ignoreCase)` | 复制Bean对象属性 |
| `cn.hutool.core.bean.BeanUtil` | `void descForEach(Class<?> clazz,Consumer<? super PropDesc> action)` | 遍历Bean的属性 |
| `cn.hutool.core.bean.BeanUtil` | `void setProperty(Object bean,String expression,Object value)` | 解析Bean中的属性值 |
| `cn.hutool.core.bean.DynaBean` | `Class<T> getBeanClass()` | 获得Bean的类型 |
| `cn.hutool.core.bean.DynaBean` | `DynaBean create(Class<?> beanClass)` | 创建一个DynaBean |
| `cn.hutool.core.bean.DynaBean` | `DynaBean create(Class<?> beanClass,Object... params)` | 创建一个DynaBean |
| `cn.hutool.core.bean.DynaBean` | `DynaBean create(Object bean)` | 创建一个DynaBean |
| `cn.hutool.core.bean.DynaBean` | `Object invoke(String methodName,Object... params)` | 执行原始Bean中的方法 |
| `cn.hutool.core.bean.DynaBean` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.bean.DynaBean` | `T get(String fieldName)` | 获得字段对应值 |
| `cn.hutool.core.bean.DynaBean` | `T getBean()` | 获得原始Bean |
| `cn.hutool.core.bean.DynaBean` | `T safeGet(String fieldName)` | 获得字段对应值，获取异常返回null |
| `cn.hutool.core.bean.DynaBean` | `boolean containsProp(String fieldName)` | 检查是否有指定名称的bean属性 |
| `cn.hutool.core.bean.DynaBean` | `boolean equals(Object obj)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.bean.DynaBean` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.bean.DynaBean` | `void set(String fieldName,Object value)` | 设置字段值 |
| `cn.hutool.core.bean.NullWrapperBean` | `Class<T> getWrappedClass()` | 获取null值对应的类型 |
| `cn.hutool.core.bean.PropDesc` | `Class<?> getFieldClass()` | 获得字段类型 先获取字段的类型，如果字段不存在，则获取Getter方法的返回类型，否则获取Setter的第一个参数类型 |
| `cn.hutool.core.bean.PropDesc` | `Field getField()` | 获取字段 |
| `cn.hutool.core.bean.PropDesc` | `Method getGetter()` | 获取Getter方法，可能为null |
| `cn.hutool.core.bean.PropDesc` | `Method getSetter()` | 获取Setter方法，可能为null |
| `cn.hutool.core.bean.PropDesc` | `Object getValue(Object bean)` | 获取属性值 首先调用字段对应的Getter方法获取值，如果Getter方法不存在，则判断字段如果为public，则直接获取字段值 此方法不检查任何注解，使用前需调用 #isReadable(boolean) 检查是否可读 |
| `cn.hutool.core.bean.PropDesc` | `Object getValue(Object bean,Type targetType,boolean ignoreError)` | 获取属性值，自动转换属性值类型 首先调用字段对应的Getter方法获取值，如果Getter方法不存在，则判断字段如果为public，则直接获取字段值 |
| `cn.hutool.core.bean.PropDesc` | `PropDesc setValue(Object bean,Object value)` | 设置Bean的字段值 首先调用字段对应的Setter方法，如果Setter方法不存在，则判断字段如果为public，则直接赋值字段值 此方法不检查任何注解，使用前需调用 #isWritable(boolean) 检查是否可写 |
| `cn.hutool.core.bean.PropDesc` | `PropDesc setValue(Object bean,Object value,boolean ignoreNull,boolean ignoreError)` | 设置属性值，可以自动转换字段类型为目标类型 |
| `cn.hutool.core.bean.PropDesc` | `PropDesc setValue(Object bean,Object value,boolean ignoreNull,boolean ignoreError,boolean override)` | 设置属性值，可以自动转换字段类型为目标类型 |
| `cn.hutool.core.bean.PropDesc` | `String getFieldName()` | 获取字段名，如果存在Alias注解，读取注解的值作为名称 |
| `cn.hutool.core.bean.PropDesc` | `String getRawFieldName()` | 获取字段名称 |
| `cn.hutool.core.bean.PropDesc` | `Type getFieldType()` | 获得字段类型 先获取字段的类型，如果字段不存在，则获取Getter方法的返回类型，否则获取Setter的第一个参数类型 |
| `cn.hutool.core.bean.PropDesc` | `boolean isReadable(boolean checkTransient)` | 检查属性是否可读（即是否可以通过#getValue(Object)获取到值） |
| `cn.hutool.core.bean.PropDesc` | `boolean isWritable(boolean checkTransient)` | 检查属性是否可读（即是否可以通过#getValue(Object)获取到值） |
| `cn.hutool.core.bean.PropDesc` | `void initialize()` | 在对象的所有属性设置完成后，执行初始化逻辑。 预先计算transient关键字和@Transient注解、PropIgnore注解信息 见：https://gitee.com/chinabugotech/hutool/pulls/1335 |
| `cn.hutool.core.bean.RecordUtil` | `Map.Entry<String, Type>[] getRecordComponents(final Class<?> recordClass)` | 获取Record类中所有字段名称，getter方法名与字段同名 |
| `cn.hutool.core.bean.RecordUtil` | `Object newInstance(final Class<?> recordClass,final ValueProvider<String> valueProvider)` | 实例化Record类 |
| `cn.hutool.core.bean.RecordUtil` | `boolean isRecord(final Class<?> clazz)` | 判断给定类是否为Record类 |
