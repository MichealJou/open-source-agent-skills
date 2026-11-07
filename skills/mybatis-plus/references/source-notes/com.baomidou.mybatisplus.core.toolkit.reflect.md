# com.baomidou.mybatisplus.core.toolkit.reflect

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.core.toolkit.reflect.GenericTypeUtils` | `Class<?>[] resolveTypeArguments(final Class<?> clazz,final Class<?> genericIfc)` | 获取泛型工具助手 |
| `com.baomidou.mybatisplus.core.toolkit.reflect.GenericTypeUtils` | `boolean hasGenericTypeResolver()` | 判断是否有自定泛型提取类或能否加载SpringCore进行泛型提取 |
| `com.baomidou.mybatisplus.core.toolkit.reflect.GenericTypeUtils` | `void setGenericTypeResolver(IGenericTypeResolver genericTypeResolver)` | 设置泛型工具助手。如果不想使用Spring封装，可以使用前替换掉 |
| `com.baomidou.mybatisplus.core.toolkit.reflect.IGenericTypeResolver` | `Class<?>[] resolveTypeArguments(final Class<?> clazz,final Class<?> genericIfc)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.reflect.SpringReflectionHelper` | `Class<?>[] resolveTypeArguments(Class<?> clazz,Class<?> genericIfc)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.reflect.TypeParameterResolver` | `Map<TypeVariable<?>, Type> resolveParameterValues(Type from)` | 解析指定类型下的泛型参数实现信息 |
| `com.baomidou.mybatisplus.core.toolkit.reflect.TypeParameterResolver` | `Type calculateParameterValue(Map<TypeVariable<?>, Type> map,TypeVariable<?> parameter)` | 计算参数值 |
| `com.baomidou.mybatisplus.core.toolkit.reflect.TypeParameterResolver` | `Type resolveClassIndexedParameter(Type type,Class<?> source,int index)` | 获取类型上指定索引位置参数的实现信息 |
| `com.baomidou.mybatisplus.core.toolkit.reflect.TypeParameterResolver` | `void visitType(Type type)` | 访问类型，类型中需要关注两个：Class 和 ParameterizedType |
