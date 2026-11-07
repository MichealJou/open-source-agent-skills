# com.feilong.core.lang.reflect

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.core.lang.reflect.ConstructorUtil` | `T newInstance(Class<T> klass,Object... parameterValues)` | 新建实例,返回指定类型 klass 的实例,使用正确的构造函数使用参数类型 parameterValues . |
| `com.feilong.core.lang.reflect.ConstructorUtil` | `T newInstance(Class<T> klass,Object[] parameterValues,Class<?>[] parameterTypes)` | 返回指定类型 klass ,指定参数 parameterValues 和指定参数类型 parameterTypes 的构造函数示例. |
| `com.feilong.core.lang.reflect.FieldUtil` | `List<Field> getAllFieldList(final Class<?> klass,String... excludeFieldNames)` | 获得 klass 排除某些 excludeFieldNames 之后的字段list. |
| `com.feilong.core.lang.reflect.FieldUtil` | `Map<String, Object> getAllFieldNameAndValueMap(Object obj,String... excludeFieldNames)` | 获得对象 obj 所有字段的值( 不是属性 ),key是 fieldName,value 是值. |
| `com.feilong.core.lang.reflect.MethodUtil` | `T invokeMethod(Object obj,String methodName,Object... params)` | 执行指定对象 object 的指定方法 methodName . |
| `com.feilong.core.lang.reflect.MethodUtil` | `T invokeMethod(final Object object,final String methodName,Object[] args,Class<?>[] parameterTypes)` | 执行指定对象 object 的指定方法 methodName . |
| `com.feilong.core.lang.reflect.MethodUtil` | `T invokeStaticMethod(Class<?> klass,String staticMethodName,Object... params)` | 执行指定类型 klass 的指定静态方法 staticMethodName (同时支持 私有静态方法). |
| `com.feilong.core.lang.reflect.MethodUtil` | `T invokeStaticMethod(final Class<?> klass,final String staticMethodName,Object[] args,Class<?>[] parameterTypes)` | 执行指定类型 klass 的指定静态方法 staticMethodName (同时支持 私有静态方法). |
| `com.feilong.core.lang.reflect.TypeUtil` | `Class<?>[] getGenericInterfacesParameterizedRawTypes(Class<?> klass,Class<?> extractInterfaceClass)` | 获得类的 接口 上的泛型参数的类型. |
| `com.feilong.core.lang.reflect.TypeUtil` | `Class<?>[] getGenericSuperclassParameterizedRawTypes(Class<?> klass)` | 获得类的 父类 上的泛型参数的类型. |
