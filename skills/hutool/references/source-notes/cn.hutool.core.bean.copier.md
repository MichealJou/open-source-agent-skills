# cn.hutool.core.bean.copier

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.bean.copier.BeanCopier` | `BeanCopier<T> create(Object source,T target,CopyOptions copyOptions)` | 创建BeanCopier |
| `cn.hutool.core.bean.copier.BeanCopier` | `BeanCopier<T> create(Object source,T target,Type destType,CopyOptions copyOptions)` | 创建BeanCopier |
| `cn.hutool.core.bean.copier.BeanCopier` | `T copy()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.bean.copier.BeanToBeanCopier` | `T copy()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.bean.copier.BeanToMapCopier` | `Map copy()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.bean.copier.CopyOptions` | `CopyOptions create()` | 创建拷贝选项 |
| `cn.hutool.core.bean.copier.CopyOptions` | `CopyOptions create(Class<?> editable,boolean ignoreNullValue,String... ignoreProperties)` | 创建拷贝选项 |
| `cn.hutool.core.bean.copier.CopyOptions` | `CopyOptions ignoreCase()` | 设置忽略字段的大小写 |
| `cn.hutool.core.bean.copier.CopyOptions` | `CopyOptions ignoreError()` | 设置忽略字段的注入错误 |
| `cn.hutool.core.bean.copier.CopyOptions` | `CopyOptions ignoreNullValue()` | 设置忽略空值，当源对象的值为null时，忽略而不注入此值 |
| `cn.hutool.core.bean.copier.CopyOptions` | `CopyOptions setAutoTransCamelCase(final boolean autoTransCamelCase)` | 设置是否自动转换为驼峰方式 一般用于map转bean和bean转bean出现非驼峰格式时，在尝试转换失败的情况下，是否二次检查转为驼峰匹配 此设置用于解决Bean和Map转换中的匹配问题而设置，并不是一个强制参数。 当map转bean时，如果map中是下划线等非驼峰模式，自动匹配对应的驼峰字段，避免出现字段不拷贝问题。 当bean转bean时，由于字段命名不规范，使用了非驼峰方式，增加兼容性。 但是bean转Map和map转map时，没有使用这个参数，是因为没有匹配的必要，转map不存在无法匹配到的问题，因此此参数无效。 |
| `cn.hutool.core.bean.copier.CopyOptions` | `CopyOptions setConverter(TypeConverter converter)` | 设置自定义类型转换器，默认使用全局万能转换器转换。 |
| `cn.hutool.core.bean.copier.CopyOptions` | `CopyOptions setEditable(Class<?> editable)` | 设置限制的类或接口，必须为目标对象的实现接口或父类，用于限制拷贝的属性 |
| `cn.hutool.core.bean.copier.CopyOptions` | `CopyOptions setFieldMapping(Map<String, String> fieldMapping)` | 设置拷贝属性的字段映射，用于不同的属性之前拷贝做对应表用 需要注意的是，当使用ValueProvider作为数据提供者时，这个映射是相反的，即fieldMapping中key为目标Bean的名称，而value是提供者中的key |
| `cn.hutool.core.bean.copier.CopyOptions` | `CopyOptions setFieldNameEditor(Editor<String> fieldNameEditor)` | 设置字段属性编辑器，用于自定义属性转换规则，例如驼峰转下划线等 此转换器只针对源端的字段做转换，请确认转换后与目标端字段一致 当转换后的字段名为null时忽略这个字段 需要注意的是，当使用ValueProvider作为数据提供者时，这个映射是相反的，即fieldMapping中key为目标Bean的名称，而value是提供者中的key |
| `cn.hutool.core.bean.copier.CopyOptions` | `CopyOptions setFieldValueEditor(BiFunction<String, Object, Object> fieldValueEditor)` | 设置字段属性值编辑器，用于自定义属性值转换规则，例如null转""等 |
| `cn.hutool.core.bean.copier.CopyOptions` | `CopyOptions setFormatIfDate(String formatIfDate)` | 设置日期格式，用于日期转字符串，默认为null |
| `cn.hutool.core.bean.copier.CopyOptions` | `CopyOptions setIgnoreCase(boolean ignoreCase)` | 设置是否忽略字段的大小写 |
| `cn.hutool.core.bean.copier.CopyOptions` | `CopyOptions setIgnoreError(boolean ignoreError)` | 设置是否忽略字段的注入错误 |
| `cn.hutool.core.bean.copier.CopyOptions` | `CopyOptions setIgnoreNullValue(boolean ignoreNullVall)` | 设置是否忽略空值，当源对象的值为null时，true: 忽略而不注入此值，false: 注入null |
| `cn.hutool.core.bean.copier.CopyOptions` | `CopyOptions setIgnoreProperties(Func1<P, R>... funcs)` | 设置忽略的目标对象中属性列表，设置一个属性列表，不拷贝这些属性值，Lambda方式 |
| `cn.hutool.core.bean.copier.CopyOptions` | `CopyOptions setIgnoreProperties(String... ignoreProperties)` | 设置忽略的目标对象中属性列表，设置一个属性列表，不拷贝这些属性值 |
| `cn.hutool.core.bean.copier.CopyOptions` | `CopyOptions setOverride(boolean override)` | 设置是否覆盖目标值，如果不覆盖，会先读取目标对象的值，为null则写，否则忽略。如果覆盖，则不判断直接写 |
| `cn.hutool.core.bean.copier.CopyOptions` | `CopyOptions setPropertiesFilter(BiPredicate<Field, Object> propertiesFilter)` | 属性过滤器，断言通过的属性才会被复制 BiPredicate#test(Object, Object)返回true则属性通过，false不通过，抛弃之 |
| `cn.hutool.core.bean.copier.CopyOptions` | `CopyOptions setTransientSupport(boolean transientSupport)` | 设置是否支持transient关键字修饰和@Transient注解，如果支持，被修饰的字段或方法对应的字段将被忽略。 |
| `cn.hutool.core.bean.copier.CopyOptions` | `String getFormatIfDate()` | 获取日期格式，用于日期转字符串，默认为null |
| `cn.hutool.core.bean.copier.IJSONTypeConverter` | `T toBean(Type type)` | 转为实体类对象 |
| `cn.hutool.core.bean.copier.MapToBeanCopier` | `T copy()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.bean.copier.MapToMapCopier` | `Map copy()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.bean.copier.ValueProvider` | `Object value(T key,Type valueType)` | 获取值 返回值一般需要匹配被注入类型，如果不匹配会调用默认转换 Convert#convert(Type, Object)实现转换 |
| `cn.hutool.core.bean.copier.ValueProvider` | `boolean containsKey(T key)` | 是否包含指定KEY，如果不包含则忽略注入 此接口方法单独需要实现的意义在于：有些值提供者（比如Map）key是存在的，但是value为null，此时如果需要注入这个null，需要根据此方法判断 |
| `cn.hutool.core.bean.copier.ValueProviderToBeanCopier` | `T copy()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
