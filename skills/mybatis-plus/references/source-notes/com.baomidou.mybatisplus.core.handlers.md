# com.baomidou.mybatisplus.core.handlers

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.core.handlers.AnnotationHandler` | `T getAnnotation(Class<?> beanClass,Class<T> annotationClass)` | 从类上获取注解 |
| `com.baomidou.mybatisplus.core.handlers.AnnotationHandler` | `T getAnnotation(Field field,Class<T> annotationClass)` | 从字段上获取注解 |
| `com.baomidou.mybatisplus.core.handlers.AnnotationHandler` | `T getAnnotation(Method method,Class<T> annotationClass)` | 从方法上获取注解 |
| `com.baomidou.mybatisplus.core.handlers.AnnotationHandler` | `boolean isAnnotationPresent(Class<?> beanClass,Class<T> annotationClass)` | 判断类上是否存在注解 |
| `com.baomidou.mybatisplus.core.handlers.AnnotationHandler` | `boolean isAnnotationPresent(Field field,Class<T> annotationClass)` | 判断字段上是否存在注解 |
| `com.baomidou.mybatisplus.core.handlers.AnnotationHandler` | `boolean isAnnotationPresent(Method method,Class<T> annotationClass)` | 判断方法上是否存在注解 |
| `com.baomidou.mybatisplus.core.handlers.CompositeEnumTypeHandler` | `E getResult(CallableStatement cs,int columnIndex)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.handlers.CompositeEnumTypeHandler` | `E getResult(ResultSet rs,String columnName)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.handlers.CompositeEnumTypeHandler` | `E getResult(ResultSet rs,int columnIndex)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.handlers.CompositeEnumTypeHandler` | `TypeHandler<T> getInstance(Class<?> javaTypeClass,Class<?> typeHandlerClass)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.handlers.CompositeEnumTypeHandler` | `void setDefaultEnumTypeHandler(Class<? extends TypeHandler> defaultEnumTypeHandler)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.handlers.CompositeEnumTypeHandler` | `void setParameter(PreparedStatement ps,int i,E parameter,JdbcType jdbcType)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.handlers.IJsonTypeHandler` | `String toJson(T obj)` | 序列化json |
| `com.baomidou.mybatisplus.core.handlers.IJsonTypeHandler` | `T parse(String json)` | 反序列化json |
| `com.baomidou.mybatisplus.core.handlers.MetaObjectHandler` | `MetaObjectHandler fillStrategy(MetaObject metaObject,String fieldName,Object fieldVal)` | 填充策略,默认有值不覆盖,如果提供的值为null也不填充 |
| `com.baomidou.mybatisplus.core.handlers.MetaObjectHandler` | `MetaObjectHandler setFieldValByName(String fieldName,Object fieldVal,MetaObject metaObject)` | 通用填充 |
| `com.baomidou.mybatisplus.core.handlers.MetaObjectHandler` | `MetaObjectHandler strictFill(boolean insertFill,TableInfo tableInfo,MetaObject metaObject,List<StrictFill<?, ?>> strictFills)` | 严格填充,只针对非主键的字段,只有该表注解了fill 并且 字段名和字段属性 能匹配到才会进行填充(null 值不填充) |
| `com.baomidou.mybatisplus.core.handlers.MetaObjectHandler` | `MetaObjectHandler strictFillStrategy(MetaObject metaObject,String fieldName,Supplier<?> fieldVal)` | 严格模式填充策略,默认有值不覆盖,如果提供的值为null也不填充 |
| `com.baomidou.mybatisplus.core.handlers.MetaObjectHandler` | `MetaObjectHandler strictInsertFill(MetaObject metaObject,String fieldName,Class<T> fieldType,E fieldVal)` | 【原文待译】@param metaObject metaObject meta object parameter |
| `com.baomidou.mybatisplus.core.handlers.MetaObjectHandler` | `MetaObjectHandler strictInsertFill(MetaObject metaObject,String fieldName,Supplier<E> fieldVal,Class<T> fieldType)` | 【原文待译】@param metaObject metaObject meta object parameter |
| `com.baomidou.mybatisplus.core.handlers.MetaObjectHandler` | `MetaObjectHandler strictInsertFill(TableInfo tableInfo,MetaObject metaObject,List<StrictFill<?, ?>> strictFills)` | 【原文待译】@param metaObject metaObject meta object parameter |
| `com.baomidou.mybatisplus.core.handlers.MetaObjectHandler` | `MetaObjectHandler strictUpdateFill(MetaObject metaObject,String fieldName,Class<T> fieldType,E fieldVal)` | 【原文待译】@param metaObject metaObject meta object parameter |
| `com.baomidou.mybatisplus.core.handlers.MetaObjectHandler` | `MetaObjectHandler strictUpdateFill(MetaObject metaObject,String fieldName,Supplier<E> fieldVal,Class<T> fieldType)` | 【原文待译】@param metaObject metaObject meta object parameter |
| `com.baomidou.mybatisplus.core.handlers.MetaObjectHandler` | `MetaObjectHandler strictUpdateFill(TableInfo tableInfo,MetaObject metaObject,List<StrictFill<?, ?>> strictFills)` | 【原文待译】@param metaObject metaObject meta object parameter |
| `com.baomidou.mybatisplus.core.handlers.MetaObjectHandler` | `Object getFieldValByName(String fieldName,MetaObject metaObject)` | 【原文待译】get value from java bean by propertyName |
| `com.baomidou.mybatisplus.core.handlers.MetaObjectHandler` | `TableInfo findTableInfo(MetaObject metaObject)` | find the tableInfo cache by metaObject 获取 TableInfo 缓存 |
| `com.baomidou.mybatisplus.core.handlers.MetaObjectHandler` | `boolean openInsertFill()` | 是否开启了插入填充 |
| `com.baomidou.mybatisplus.core.handlers.MetaObjectHandler` | `boolean openInsertFill(MappedStatement mappedStatement)` | 是否开启插入填充 |
| `com.baomidou.mybatisplus.core.handlers.MetaObjectHandler` | `boolean openUpdateFill()` | 是否开启了更新填充 |
| `com.baomidou.mybatisplus.core.handlers.MetaObjectHandler` | `boolean openUpdateFill(MappedStatement mappedStatement)` | 是否开启了更新填充 |
| `com.baomidou.mybatisplus.core.handlers.MetaObjectHandler` | `void insertFill(MetaObject metaObject)` | 插入元对象字段填充（用于插入时对公共字段的填充） |
| `com.baomidou.mybatisplus.core.handlers.MetaObjectHandler` | `void updateFill(MetaObject metaObject)` | 更新元对象字段填充（用于更新时对公共字段的填充） |
| `com.baomidou.mybatisplus.core.handlers.MybatisEnumTypeHandler` | `E getNullableResult(CallableStatement cs,int columnIndex)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.handlers.MybatisEnumTypeHandler` | `E getNullableResult(ResultSet rs,String columnName)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.handlers.MybatisEnumTypeHandler` | `E getNullableResult(ResultSet rs,int columnIndex)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.handlers.MybatisEnumTypeHandler` | `Optional<String> findEnumValueFieldName(Class<?> clazz)` | 查找标记标记EnumValue字段 |
| `com.baomidou.mybatisplus.core.handlers.MybatisEnumTypeHandler` | `boolean isMpEnums(Class<?> clazz)` | 判断是否为MP枚举处理 |
| `com.baomidou.mybatisplus.core.handlers.MybatisEnumTypeHandler` | `void setNonNullParameter(PreparedStatement ps,int i,E parameter,JdbcType jdbcType)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.handlers.PostInitTableInfoHandler` | `TableInfo creteTableInfo(Configuration configuration,Class<?> entityType)` | 提供对 TableInfo 增强的能力 |
| `com.baomidou.mybatisplus.core.handlers.PostInitTableInfoHandler` | `void postFieldInfo(TableFieldInfo fieldInfo,Configuration configuration)` | 参与 TableFieldInfo 初始化 |
| `com.baomidou.mybatisplus.core.handlers.PostInitTableInfoHandler` | `void postTableInfo(TableInfo tableInfo,Configuration configuration)` | 参与 TableInfo 初始化 |
| `com.baomidou.mybatisplus.core.handlers.StrictFill` | `StrictFill<T, E> of(String fieldName,Class<T> fieldType,E fieldVal)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.handlers.StrictFill` | `StrictFill<T, E> of(String fieldName,Supplier<E> fieldVal,Class<T> fieldType)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
