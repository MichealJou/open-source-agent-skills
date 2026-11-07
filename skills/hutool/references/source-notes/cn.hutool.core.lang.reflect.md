# cn.hutool.core.lang.reflect

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.lang.reflect.ActualTypeMapperPool` | `Map<String, Type> getStrKeyMap(Type type)` | 获取泛型变量名（字符串）和泛型实际类型的对应关系Map |
| `cn.hutool.core.lang.reflect.ActualTypeMapperPool` | `Map<Type, Type> get(Type type)` | 获取泛型变量和泛型实际类型的对应关系Map |
| `cn.hutool.core.lang.reflect.ActualTypeMapperPool` | `Type getActualType(Type type,GenericArrayType genericArrayType)` | 获得泛型变量对应的泛型实际类型，如果此变量没有对应的实际类型，返回null |
| `cn.hutool.core.lang.reflect.ActualTypeMapperPool` | `Type getActualType(Type type,TypeVariable<?> typeVariable)` | 获得泛型变量对应的泛型实际类型，如果此变量没有对应的实际类型，返回null |
| `cn.hutool.core.lang.reflect.ActualTypeMapperPool` | `Type[] getActualTypes(Type type,Type... typeVariables)` | 获取指定泛型变量对应的真实类型 由于子类中泛型参数实现和父类（接口）中泛型定义位置是一一对应的，因此可以通过对应关系找到泛型实现类型 |
| `cn.hutool.core.lang.reflect.LookupFactory` | `MethodHandles.Lookup lookup(Class<?> callerClass)` | jdk8中如果直接调用MethodHandles#lookup()获取到的MethodHandles.Lookup在调用findSpecial和unreflectSpecial 时会出现权限不够问题，抛出"no private access for invokespecial"异常，因此针对JDK8及JDK9+分别封装lookup方法。 |
| `cn.hutool.core.lang.reflect.MethodHandleUtil` | `MethodHandle findConstructor(Class<?> callerClass,Class<?>... args)` | 查找指定的构造方法 |
| `cn.hutool.core.lang.reflect.MethodHandleUtil` | `MethodHandle findConstructor(Class<?> callerClass,MethodType type)` | 查找指定的构造方法 |
| `cn.hutool.core.lang.reflect.MethodHandleUtil` | `MethodHandle findMethod(Class<?> callerClass,String name,MethodType type)` | 查找指定方法的方法句柄 此方法只会查找： 当前类的方法（包括构造方法和private方法） 父类的方法（包括构造方法和private方法） 当前类的static方法 |
| `cn.hutool.core.lang.reflect.MethodHandleUtil` | `MethodHandles.Lookup lookup(Class<?> callerClass)` | jdk8中如果直接调用MethodHandles#lookup()获取到的MethodHandles.Lookup在调用findSpecial和unreflectSpecial 时会出现权限不够问题，抛出"no private access for invokespecial"异常，因此针对JDK8及JDK9+分别封装lookup方法。 |
| `cn.hutool.core.lang.reflect.MethodHandleUtil` | `T invoke(Object obj,Method method,Object... args)` | 执行接口或对象中的方法 |
| `cn.hutool.core.lang.reflect.MethodHandleUtil` | `T invoke(boolean isSpecial,Object obj,Method method,Object... args)` | 执行接口或对象中的方法 |
| `cn.hutool.core.lang.reflect.MethodHandleUtil` | `T invokeSpecial(Object obj,Method method,Object... args)` | 执行接口或对象中的特殊方法（private、static等） |
| `cn.hutool.core.lang.reflect.MethodHandleUtil` | `T invokeSpecial(Object obj,String methodName,Object... args)` | 执行接口或对象中的特殊方法（private、static等） |
