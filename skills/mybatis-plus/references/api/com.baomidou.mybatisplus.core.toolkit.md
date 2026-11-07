# com.baomidou.mybatisplus.core.toolkit

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.core.toolkit.AES`

```java
public class com.baomidou.mybatisplus.core.toolkit.AES {
  public com.baomidou.mybatisplus.core.toolkit.AES();
  public static byte[] encrypt(byte[], byte[]);
  public static byte[] decrypt(byte[], byte[]);
  public static java.lang.String encrypt(java.lang.String, java.lang.String);
  public static java.lang.String decrypt(java.lang.String, java.lang.String);
  public static java.lang.String generateRandomKey();
}
```

## `com.baomidou.mybatisplus.core.toolkit.AnnotationUtils`

```java
public final class com.baomidou.mybatisplus.core.toolkit.AnnotationUtils {
  public static <T extends java.lang.annotation.Annotation> T findFirstAnnotation(java.lang.Class<T>, java.lang.reflect.Field);
  public static <T extends java.lang.annotation.Annotation> T findFirstAnnotation(java.lang.Class<T>, java.lang.Class<?>);
  public static <T extends java.lang.annotation.Annotation> T findFirstAnnotation(java.lang.Class<T>, java.lang.reflect.Method);
}
```

## `com.baomidou.mybatisplus.core.toolkit.AopUtils`

```java
public class com.baomidou.mybatisplus.core.toolkit.AopUtils {
  public com.baomidou.mybatisplus.core.toolkit.AopUtils();
  public static boolean isLoadSpringAop();
  public static <T> T getTargetObject(T);
}
```

## `com.baomidou.mybatisplus.core.toolkit.ArrayUtils`

```java
public final class com.baomidou.mybatisplus.core.toolkit.ArrayUtils {
  public static boolean isEmpty(java.lang.Object[]);
  public static boolean isNotEmpty(java.lang.Object[]);
  public static boolean isArray(java.lang.Object);
}
```

## `com.baomidou.mybatisplus.core.toolkit.Assert`

```java
public final class com.baomidou.mybatisplus.core.toolkit.Assert {
  public com.baomidou.mybatisplus.core.toolkit.Assert();
  public static void isTrue(boolean, java.lang.String, java.lang.Object...);
  public static void isFalse(boolean, java.lang.String, java.lang.Object...);
  public static void isNull(java.lang.Object, java.lang.String, java.lang.Object...);
  public static void notNull(java.lang.Object, java.lang.String, java.lang.Object...);
  public static void notEmpty(java.lang.String, java.lang.String, java.lang.Object...);
  public static void notEmpty(java.util.Collection<?>, java.lang.String, java.lang.Object...);
  public static void notEmpty(java.util.Map<?, ?>, java.lang.String, java.lang.Object...);
  public static void isEmpty(java.util.Map<?, ?>, java.lang.String, java.lang.Object...);
  public static void notEmpty(java.lang.Object[], java.lang.String, java.lang.Object...);
}
```

## `com.baomidou.mybatisplus.core.toolkit.BeanUtils`

```java
public final class com.baomidou.mybatisplus.core.toolkit.BeanUtils {
  public static java.util.Map<java.lang.String, java.lang.Object> beanToMap(java.lang.Object);
  public static <T> T mapToBean(java.util.Map<java.lang.String, ?>, java.lang.Class<T>);
  public static <T> java.util.List<java.util.Map<java.lang.String, java.lang.Object>> beansToMaps(java.util.List<T>);
  public static <T> java.util.List<T> mapsToBeans(java.util.List<? extends java.util.Map<java.lang.String, ?>>, java.lang.Class<T>);
}
```

## `com.baomidou.mybatisplus.core.toolkit.ClassUtils`

```java
public final class com.baomidou.mybatisplus.core.toolkit.ClassUtils {
  public static boolean isBoolean(java.lang.Class<?>);
  public static boolean isProxy(java.lang.Class<?>);
  public static java.lang.Class<?> getUserClass(java.lang.Class<?>);
  public static java.lang.Class<?> getUserClass(java.lang.Object);
  public static <T> T newInstance(java.lang.Class<T>);
  public static <T> T newInstance(java.lang.String);
  public static java.lang.Class<?> toClassConfident(java.lang.String);
  public static java.lang.Class<?> toClassConfident(java.lang.String, java.lang.ClassLoader);
  public static java.lang.String getPackageName(java.lang.Class<?>);
  public static java.lang.String getPackageName(java.lang.String);
  public static java.lang.ClassLoader getDefaultClassLoader();
}
```

## `com.baomidou.mybatisplus.core.toolkit.CollectionUtils`

```java
public class com.baomidou.mybatisplus.core.toolkit.CollectionUtils {
  public com.baomidou.mybatisplus.core.toolkit.CollectionUtils();
  public static boolean isEmpty(java.util.Collection<?>);
  public static boolean isNotEmpty(java.util.Collection<?>);
  public static boolean isEmpty(java.util.Map<?, ?>);
  public static boolean isNotEmpty(java.util.Map<?, ?>);
  public static <K, V> java.util.HashMap<K, V> newHashMap();
  public static <K, V> java.util.HashMap<K, V> newHashMapWithExpectedSize(int);
  public static <K, V> V computeIfAbsent(java.util.Map<K, V>, K, java.util.function.Function<? super K, ? extends V>);
  public static <K, V> java.util.List<V> getCollection(java.util.Map<K, V>, java.lang.Iterable<K>);
  public static <K, V> java.util.List<V> getCollection(java.util.Map<K, V>, java.lang.Iterable<K>, java.util.Comparator<V>);
  public static <T> java.util.List<T> toList(T...);
  public static <T> java.util.List<java.util.List<T>> split(java.util.Collection<T>, int);
}
```

## `com.baomidou.mybatisplus.core.toolkit.EncryptUtils`

```java
public class com.baomidou.mybatisplus.core.toolkit.EncryptUtils {
  public com.baomidou.mybatisplus.core.toolkit.EncryptUtils();
  public static java.lang.String md5Base64(java.lang.String);
}
```

## `com.baomidou.mybatisplus.core.toolkit.ExceptionUtils`

```java
public final class com.baomidou.mybatisplus.core.toolkit.ExceptionUtils {
  public static com.baomidou.mybatisplus.core.exceptions.MybatisPlusException mpe(java.lang.String, java.lang.Throwable, java.lang.Object...);
  public static com.baomidou.mybatisplus.core.exceptions.MybatisPlusException mpe(java.lang.String, java.lang.Object...);
  public static com.baomidou.mybatisplus.core.exceptions.MybatisPlusException mpe(java.lang.Throwable);
  public static void throwMpe(boolean, java.lang.String, java.lang.Object...);
}
```

## `com.baomidou.mybatisplus.core.toolkit.GlobalConfigUtils`

```java
public class com.baomidou.mybatisplus.core.toolkit.GlobalConfigUtils {
  public com.baomidou.mybatisplus.core.toolkit.GlobalConfigUtils();
  public static org.apache.ibatis.session.SqlSessionFactory currentSessionFactory(java.lang.Class<?>);
  public static com.baomidou.mybatisplus.core.config.GlobalConfig defaults();
  public static void setGlobalConfig(org.apache.ibatis.session.Configuration, com.baomidou.mybatisplus.core.config.GlobalConfig);
  public static com.baomidou.mybatisplus.core.config.GlobalConfig getGlobalConfig(org.apache.ibatis.session.Configuration);
  public static java.util.List<com.baomidou.mybatisplus.core.incrementer.IKeyGenerator> getKeyGenerators(org.apache.ibatis.session.Configuration);
  public static com.baomidou.mybatisplus.annotation.IdType getIdType(org.apache.ibatis.session.Configuration);
  public static com.baomidou.mybatisplus.core.config.GlobalConfig$DbConfig getDbConfig(org.apache.ibatis.session.Configuration);
  public static com.baomidou.mybatisplus.core.injector.ISqlInjector getSqlInjector(org.apache.ibatis.session.Configuration);
  public static java.util.Optional<com.baomidou.mybatisplus.core.handlers.MetaObjectHandler> getMetaObjectHandler(org.apache.ibatis.session.Configuration);
  public static java.util.Optional<com.baomidou.mybatisplus.core.handlers.AnnotationHandler> getAnnotationHandler(org.apache.ibatis.session.Configuration);
  public static java.lang.Class<?> getSuperMapperClass(org.apache.ibatis.session.Configuration);
  public static boolean isSupperMapperChildren(org.apache.ibatis.session.Configuration, java.lang.Class<?>);
  public static java.util.Set<java.lang.String> getMapperRegistryCache(org.apache.ibatis.session.Configuration);
}
```

## `com.baomidou.mybatisplus.core.toolkit.IdWorker`

```java
public class com.baomidou.mybatisplus.core.toolkit.IdWorker {
  public com.baomidou.mybatisplus.core.toolkit.IdWorker();
  public static long getId();
  public static long getId(java.lang.Object);
  public static java.lang.String getIdStr();
  public static java.lang.String getIdStr(java.lang.Object);
  public static java.lang.String getMillisecond();
  public static java.lang.String getTimeId();
  public static void initSequence(long, long);
  public static void setIdentifierGenerator(com.baomidou.mybatisplus.core.incrementer.IdentifierGenerator);
  public static java.lang.String get32UUID();
}
```

## `com.baomidou.mybatisplus.core.toolkit.LambdaUtils`

```java
public final class com.baomidou.mybatisplus.core.toolkit.LambdaUtils {
  public com.baomidou.mybatisplus.core.toolkit.LambdaUtils();
  public static <T> com.baomidou.mybatisplus.core.toolkit.support.LambdaMeta extract(com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>);
  public static java.lang.String formatKey(java.lang.String);
  public static void installCache(com.baomidou.mybatisplus.core.metadata.TableInfo);
  public static java.util.Map<java.lang.String, com.baomidou.mybatisplus.core.toolkit.support.ColumnCache> getColumnMap(java.lang.Class<?>);
}
```

## `com.baomidou.mybatisplus.core.toolkit.MybatisBatchUtils`

```java
public class com.baomidou.mybatisplus.core.toolkit.MybatisBatchUtils {
  public com.baomidou.mybatisplus.core.toolkit.MybatisBatchUtils();
  public static <T> java.util.List<org.apache.ibatis.executor.BatchResult> execute(org.apache.ibatis.session.SqlSessionFactory, java.util.Collection<T>, java.lang.String);
  public static <T> java.util.List<org.apache.ibatis.executor.BatchResult> execute(org.apache.ibatis.session.SqlSessionFactory, java.util.Collection<T>, java.lang.String, int);
  public static <T> java.util.List<org.apache.ibatis.executor.BatchResult> execute(org.apache.ibatis.session.SqlSessionFactory, java.util.Collection<T>, java.lang.String, com.baomidou.mybatisplus.core.batch.ParameterConvert<T>);
  public static <T> java.util.List<org.apache.ibatis.executor.BatchResult> execute(org.apache.ibatis.session.SqlSessionFactory, java.util.Collection<T>, java.lang.String, com.baomidou.mybatisplus.core.batch.ParameterConvert<T>, int);
  public static <T> java.util.List<org.apache.ibatis.executor.BatchResult> execute(org.apache.ibatis.session.SqlSessionFactory, java.util.Collection<T>, boolean, java.lang.String);
  public static <T> java.util.List<org.apache.ibatis.executor.BatchResult> execute(org.apache.ibatis.session.SqlSessionFactory, java.util.Collection<T>, boolean, java.lang.String, int);
  public static <T> java.util.List<org.apache.ibatis.executor.BatchResult> execute(org.apache.ibatis.session.SqlSessionFactory, java.util.Collection<T>, boolean, java.lang.String, com.baomidou.mybatisplus.core.batch.ParameterConvert<T>);
  public static <T> java.util.List<org.apache.ibatis.executor.BatchResult> execute(org.apache.ibatis.session.SqlSessionFactory, java.util.Collection<T>, boolean, java.lang.String, com.baomidou.mybatisplus.core.batch.ParameterConvert<T>, int);
  public static <T> java.util.List<org.apache.ibatis.executor.BatchResult> execute(org.apache.ibatis.session.SqlSessionFactory, java.util.Collection<T>, com.baomidou.mybatisplus.core.batch.BatchMethod<T>);
  public static <T> java.util.List<org.apache.ibatis.executor.BatchResult> execute(org.apache.ibatis.session.SqlSessionFactory, java.util.Collection<T>, com.baomidou.mybatisplus.core.batch.BatchMethod<T>, int);
  public static <T> java.util.List<org.apache.ibatis.executor.BatchResult> execute(org.apache.ibatis.session.SqlSessionFactory, java.util.Collection<T>, boolean, com.baomidou.mybatisplus.core.batch.BatchMethod<T>);
  public static <T> java.util.List<org.apache.ibatis.executor.BatchResult> execute(org.apache.ibatis.session.SqlSessionFactory, java.util.Collection<T>, boolean, com.baomidou.mybatisplus.core.batch.BatchMethod<T>, int);
  public static <T> java.util.List<org.apache.ibatis.executor.BatchResult> saveOrUpdate(org.apache.ibatis.session.SqlSessionFactory, java.util.Collection<T>, com.baomidou.mybatisplus.core.batch.BatchMethod<T>, java.util.function.BiPredicate<com.baomidou.mybatisplus.core.batch.BatchSqlSession, T>, com.baomidou.mybatisplus.core.batch.BatchMethod<T>);
  public static <T> java.util.List<org.apache.ibatis.executor.BatchResult> saveOrUpdate(org.apache.ibatis.session.SqlSessionFactory, java.util.Collection<T>, com.baomidou.mybatisplus.core.batch.BatchMethod<T>, java.util.function.BiPredicate<com.baomidou.mybatisplus.core.batch.BatchSqlSession, T>, com.baomidou.mybatisplus.core.batch.BatchMethod<T>, int);
  public static <T> java.util.List<org.apache.ibatis.executor.BatchResult> saveOrUpdate(org.apache.ibatis.session.SqlSessionFactory, java.util.Collection<T>, boolean, com.baomidou.mybatisplus.core.batch.BatchMethod<T>, java.util.function.BiPredicate<com.baomidou.mybatisplus.core.batch.BatchSqlSession, T>, com.baomidou.mybatisplus.core.batch.BatchMethod<T>);
  public static <T> java.util.List<org.apache.ibatis.executor.BatchResult> saveOrUpdate(org.apache.ibatis.session.SqlSessionFactory, java.util.Collection<T>, boolean, com.baomidou.mybatisplus.core.batch.BatchMethod<T>, java.util.function.BiPredicate<com.baomidou.mybatisplus.core.batch.BatchSqlSession, T>, com.baomidou.mybatisplus.core.batch.BatchMethod<T>, int);
}
```

## `com.baomidou.mybatisplus.core.toolkit.MybatisUtils`

```java
public final class com.baomidou.mybatisplus.core.toolkit.MybatisUtils {
  public static org.apache.ibatis.type.TypeHandler<?> newJsonTypeHandler(java.lang.Class<? extends org.apache.ibatis.type.TypeHandler<?>>, java.lang.Class<?>, java.lang.reflect.Field);
  public static org.apache.ibatis.session.SqlSessionFactory getSqlSessionFactory(com.baomidou.mybatisplus.core.override.MybatisMapperProxy<?>);
  public static org.apache.ibatis.session.SqlSessionFactory getSqlSessionFactory(org.apache.ibatis.session.SqlSession);
  public static com.baomidou.mybatisplus.core.override.MybatisMapperProxy<?> getMybatisMapperProxy(java.lang.Object);
  public static java.lang.Object extractMapperProxy(java.lang.Object);
  public static com.baomidou.mybatisplus.core.metadata.MapperProxyMetadata getMapperProxy(java.lang.Object);
}
```

## `com.baomidou.mybatisplus.core.toolkit.NetUtils`

```java
public class com.baomidou.mybatisplus.core.toolkit.NetUtils {
  public com.baomidou.mybatisplus.core.toolkit.NetUtils(com.baomidou.mybatisplus.core.toolkit.NetUtils$NetProperties);
  public java.net.InetAddress findFirstNonLoopbackAddress();
}
```

## `com.baomidou.mybatisplus.core.toolkit.NetUtils$NetProperties`

```java
public class com.baomidou.mybatisplus.core.toolkit.NetUtils$NetProperties {
  public java.util.List<java.lang.String> getPreferredNetworks();
  public java.util.List<java.lang.String> getIgnoredInterfaces();
  public void setPreferredNetworks(java.util.List<java.lang.String>);
  public void setIgnoredInterfaces(java.util.List<java.lang.String>);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
  public com.baomidou.mybatisplus.core.toolkit.NetUtils$NetProperties();
  public com.baomidou.mybatisplus.core.toolkit.NetUtils$NetProperties(java.util.List<java.lang.String>, java.util.List<java.lang.String>);
}
```

## `com.baomidou.mybatisplus.core.toolkit.ObjectUtils`

```java
public class com.baomidou.mybatisplus.core.toolkit.ObjectUtils {
  public com.baomidou.mybatisplus.core.toolkit.ObjectUtils();
  public static boolean isNull(java.lang.Object...);
  public static boolean isNotNull(java.lang.Object...);
  public static boolean isNotEmpty(java.lang.Object);
  public static boolean isEmpty(java.lang.Object);
}
```

## `com.baomidou.mybatisplus.core.toolkit.ParameterUtils`

```java
public class com.baomidou.mybatisplus.core.toolkit.ParameterUtils {
  public static java.util.Optional<com.baomidou.mybatisplus.core.metadata.IPage> findPage(java.lang.Object);
}
```

## `com.baomidou.mybatisplus.core.toolkit.PluginUtils`

```java
public abstract class com.baomidou.mybatisplus.core.toolkit.PluginUtils {
  public com.baomidou.mybatisplus.core.toolkit.PluginUtils();
  public static <T> T realTarget(java.lang.Object);
  public static org.apache.ibatis.reflection.MetaObject getMetaObject(java.lang.Object);
  public static void setAdditionalParameter(org.apache.ibatis.mapping.BoundSql, java.util.Map<java.lang.String, java.lang.Object>);
  public static com.baomidou.mybatisplus.core.toolkit.PluginUtils$MPBoundSql mpBoundSql(org.apache.ibatis.mapping.BoundSql);
  public static com.baomidou.mybatisplus.core.toolkit.PluginUtils$MPStatementHandler mpStatementHandler(org.apache.ibatis.executor.statement.StatementHandler);
}
```

## `com.baomidou.mybatisplus.core.toolkit.PluginUtils$MPBoundSql`

```java
public class com.baomidou.mybatisplus.core.toolkit.PluginUtils$MPBoundSql {
  public java.lang.String sql();
  public void sql(java.lang.String);
  public java.util.List<org.apache.ibatis.mapping.ParameterMapping> parameterMappings();
  public void parameterMappings(java.util.List<org.apache.ibatis.mapping.ParameterMapping>);
  public java.lang.Object parameterObject();
  public java.util.Map<java.lang.String, java.lang.Object> additionalParameters();
}
```

## `com.baomidou.mybatisplus.core.toolkit.PluginUtils$MPStatementHandler`

```java
public class com.baomidou.mybatisplus.core.toolkit.PluginUtils$MPStatementHandler {
  public org.apache.ibatis.executor.parameter.ParameterHandler parameterHandler();
  public org.apache.ibatis.mapping.MappedStatement mappedStatement();
  public org.apache.ibatis.executor.Executor executor();
  public com.baomidou.mybatisplus.core.toolkit.PluginUtils$MPBoundSql mPBoundSql();
  public org.apache.ibatis.mapping.BoundSql boundSql();
  public org.apache.ibatis.session.Configuration configuration();
}
```

## `com.baomidou.mybatisplus.core.toolkit.ReflectionKit`

```java
public final class com.baomidou.mybatisplus.core.toolkit.ReflectionKit {
  public com.baomidou.mybatisplus.core.toolkit.ReflectionKit();
  public static java.lang.Object getFieldValue(java.lang.Object, java.lang.String);
  public static java.lang.Class<?> getSuperClassGenericType(java.lang.Class<?>, java.lang.Class<?>, int);
  public static java.util.Map<java.lang.String, java.lang.reflect.Field> getFieldMap(java.lang.Class<?>);
  public static java.util.List<java.lang.reflect.Field> getFieldList(java.lang.Class<?>);
  public static java.util.Map<java.lang.String, java.lang.reflect.Field> excludeOverrideSuperField(java.lang.reflect.Field[], java.util.List<java.lang.reflect.Field>);
  public static boolean isPrimitiveOrWrapper(java.lang.Class<?>);
  public static java.lang.Class<?> resolvePrimitiveIfNecessary(java.lang.Class<?>);
  public static <T extends java.lang.reflect.AccessibleObject> T setAccessible(T);
}
```

## `com.baomidou.mybatisplus.core.toolkit.Sequence`

```java
public class com.baomidou.mybatisplus.core.toolkit.Sequence {
  public com.baomidou.mybatisplus.core.toolkit.Sequence(java.net.InetAddress);
  public com.baomidou.mybatisplus.core.toolkit.Sequence(long, long);
  public static long parseIdTimestamp(long);
  public synchronized long nextId();
}
```

## `com.baomidou.mybatisplus.core.toolkit.SerializationUtils`

```java
public class com.baomidou.mybatisplus.core.toolkit.SerializationUtils {
  public com.baomidou.mybatisplus.core.toolkit.SerializationUtils();
  public static <T extends java.io.Serializable> T clone(T);
  public static byte[] serialize(java.lang.Object);
  public static java.lang.Object deserialize(byte[]);
}
```

## `com.baomidou.mybatisplus.core.toolkit.SetAccessibleAction`

```java
public class com.baomidou.mybatisplus.core.toolkit.SetAccessibleAction<T extends java.lang.reflect.AccessibleObject> implements java.security.PrivilegedAction<T> {
  public com.baomidou.mybatisplus.core.toolkit.SetAccessibleAction(T);
  public T run();
  public java.lang.Object run();
}
```

## `com.baomidou.mybatisplus.core.toolkit.StringUtils`

```java
public final class com.baomidou.mybatisplus.core.toolkit.StringUtils {
  public com.baomidou.mybatisplus.core.toolkit.StringUtils();
  public static boolean isBlank(java.lang.CharSequence);
  public static java.lang.String toStringTrim(java.lang.Object);
  public static boolean isNotBlank(java.lang.CharSequence);
  public static boolean isEmpty(java.lang.CharSequence);
  public static boolean isNotEmpty(java.lang.CharSequence);
  public static boolean isCamel(java.lang.String);
  public static boolean isNotColumnName(java.lang.String);
  public static java.lang.String getTargetColumn(java.lang.String);
  public static java.lang.String camelToUnderline(java.lang.String);
  public static java.lang.String underlineToCamel(java.lang.String);
  public static java.lang.String firstToLowerCase(java.lang.String);
  public static boolean matches(java.lang.String, java.lang.String);
  public static java.lang.String sqlArgsFill(java.lang.String, java.lang.Object...);
  public static java.lang.StringBuilder replace(java.lang.CharSequence, java.util.regex.Pattern, com.baomidou.mybatisplus.core.toolkit.support.BiIntFunction<java.util.regex.Matcher, java.lang.CharSequence>);
  public static java.lang.String sqlParam(java.lang.Object);
  public static java.lang.String quotaMark(java.lang.Object);
  public static java.lang.String quotaMarkList(java.util.Collection<?>);
  public static java.lang.String concatCapitalize(java.lang.String, java.lang.String);
  public static boolean checkValNotNull(java.lang.Object);
  public static boolean checkValNull(java.lang.Object);
  public static boolean containsUpperCase(java.lang.String);
  public static boolean isCapitalMode(java.lang.String);
  public static boolean isMixedMode(java.lang.String);
  public static boolean endsWith(java.lang.String, java.lang.String);
  public static boolean isCharSequence(java.lang.Class<?>);
  public static java.lang.String prefixToLower(java.lang.String, int);
  public static java.lang.String removePrefixAfterPrefixToLower(java.lang.String, int);
  public static java.lang.String camelToHyphen(java.lang.String);
  public static boolean equals(java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String sqlInjectionReplaceBlank(java.lang.String);
  public static java.lang.String replaceAllBlank(java.lang.String);
}
```

## `com.baomidou.mybatisplus.core.toolkit.SystemClock`

```java
public class com.baomidou.mybatisplus.core.toolkit.SystemClock {
  public static long now();
  public static java.lang.String nowDate();
}
```

## `com.baomidou.mybatisplus.core.toolkit.TableNameParser`

```java
public final class com.baomidou.mybatisplus.core.toolkit.TableNameParser {
  public com.baomidou.mybatisplus.core.toolkit.TableNameParser(java.lang.String);
  public void accept(com.baomidou.mybatisplus.core.toolkit.TableNameParser$TableNameVisitor);
  public java.util.Collection<java.lang.String> tables();
}
```

## `com.baomidou.mybatisplus.core.toolkit.TableNameParser$SqlToken`

```java
public class com.baomidou.mybatisplus.core.toolkit.TableNameParser$SqlToken implements java.lang.Comparable<com.baomidou.mybatisplus.core.toolkit.TableNameParser$SqlToken> {
  public int getStart();
  public int getEnd();
  public java.lang.String getValue();
  public int compareTo(com.baomidou.mybatisplus.core.toolkit.TableNameParser$SqlToken);
  public java.lang.String toString();
  public int compareTo(java.lang.Object);
}
```

## `com.baomidou.mybatisplus.core.toolkit.TableNameParser$TableNameVisitor`

```java
public interface com.baomidou.mybatisplus.core.toolkit.TableNameParser$TableNameVisitor {
  public abstract void visit(com.baomidou.mybatisplus.core.toolkit.TableNameParser$SqlToken);
}
```

## `com.baomidou.mybatisplus.core.toolkit.Wrappers`

```java
public final class com.baomidou.mybatisplus.core.toolkit.Wrappers {
  public static <T> com.baomidou.mybatisplus.core.conditions.query.QueryWrapper<T> query();
  public static <T> com.baomidou.mybatisplus.core.conditions.query.QueryWrapper<T> query(T);
  public static <T> com.baomidou.mybatisplus.core.conditions.query.QueryWrapper<T> query(java.lang.Class<T>);
  public static <T> com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper<T> lambdaQuery();
  public static <T> com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper<T> lambdaQuery(T);
  public static <T> com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper<T> lambdaQuery(java.lang.Class<T>);
  public static <T> com.baomidou.mybatisplus.core.conditions.update.UpdateWrapper<T> update();
  public static <T> com.baomidou.mybatisplus.core.conditions.update.UpdateWrapper<T> update(T);
  public static <T> com.baomidou.mybatisplus.core.conditions.update.LambdaUpdateWrapper<T> lambdaUpdate();
  public static <T> com.baomidou.mybatisplus.core.conditions.update.LambdaUpdateWrapper<T> lambdaUpdate(T);
  public static <T> com.baomidou.mybatisplus.core.conditions.update.LambdaUpdateWrapper<T> lambdaUpdate(java.lang.Class<T>);
  public static <T> com.baomidou.mybatisplus.core.conditions.query.QueryWrapper<T> emptyWrapper();
}
```
