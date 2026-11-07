# cn.hutool.core.lang.func

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.lang.func.Consumer3` | `void accept(P1 p1,P2 p2,P3 p3)` | 接收参数方法 |
| `cn.hutool.core.lang.func.Func` | `R call(P... parameters)` | 执行函数 |
| `cn.hutool.core.lang.func.Func` | `R callWithRuntimeException(P... parameters)` | 执行函数，异常包装为RuntimeException |
| `cn.hutool.core.lang.func.Func0` | `R call()` | 执行函数 |
| `cn.hutool.core.lang.func.Func0` | `R callWithRuntimeException()` | 执行函数，异常包装为RuntimeException |
| `cn.hutool.core.lang.func.Func1` | `R call(P parameter)` | 执行函数 |
| `cn.hutool.core.lang.func.Func1` | `R callWithRuntimeException(P parameter)` | 执行函数，异常包装为RuntimeException |
| `cn.hutool.core.lang.func.LambdaUtil` | `Class<P> getRealClass(Func1<P, R> func)` | 通过对象的方法或类的静态方法引用，然后根据SerializedLambda#getInstantiatedMethodType()获取lambda实现类 传入lambda有参数且含有返回值的情况能够匹配到此方法： 引用特定类型的任意对象的实例方法： |
| `cn.hutool.core.lang.func.LambdaUtil` | `Class<R> getRealClass(Func0<?> func)` | 通过对象的方法或类的静态方法引用，获取lambda实现类 传入lambda无参数但含有返回值的情况能够匹配到此方法： 引用特定对象的实例方法： |
| `cn.hutool.core.lang.func.LambdaUtil` | `SerializedLambda resolve(Func0<R> func)` | 解析lambda表达式,加了缓存。 该缓存可能会在任意不定的时间被清除 |
| `cn.hutool.core.lang.func.LambdaUtil` | `SerializedLambda resolve(Func1<T, ?> func)` | 解析lambda表达式,加了缓存。 该缓存可能会在任意不定的时间被清除 |
| `cn.hutool.core.lang.func.LambdaUtil` | `String getFieldName(Func0<T> func)` | 获取lambda表达式Getter或Setter函数（方法）对应的字段名称，规则如下： getXxxx获取为xxxx，如getName得到name。 setXxxx获取为xxxx，如setName得到name。 isXxxx获取为xxxx，如isName得到name。 其它不满足规则的方法名抛出IllegalArgumentException |
| `cn.hutool.core.lang.func.LambdaUtil` | `String getFieldName(Func1<T, ?> func)` | 获取lambda表达式Getter或Setter函数（方法）对应的字段名称，规则如下： getXxxx获取为xxxx，如getName得到name。 setXxxx获取为xxxx，如setName得到name。 isXxxx获取为xxxx，如isName得到name。 其它不满足规则的方法名抛出IllegalArgumentException |
| `cn.hutool.core.lang.func.LambdaUtil` | `String getMethodName(Func0<R> func)` | 获取lambda表达式函数（方法）名称 |
| `cn.hutool.core.lang.func.LambdaUtil` | `String getMethodName(Func1<P, ?> func)` | 获取lambda表达式函数（方法）名称 |
| `cn.hutool.core.lang.func.Supplier1` | `Supplier<T> toSupplier(P1 p1)` | 将带有参数的Supplier转换为无参Supplier |
| `cn.hutool.core.lang.func.Supplier1` | `T get(P1 p1)` | 生成实例的方法 |
| `cn.hutool.core.lang.func.Supplier2` | `Supplier<T> toSupplier(P1 p1,P2 p2)` | 将带有参数的Supplier转换为无参Supplier |
| `cn.hutool.core.lang.func.Supplier2` | `T get(P1 p1,P2 p2)` | 生成实例的方法 |
| `cn.hutool.core.lang.func.Supplier3` | `Supplier<T> toSupplier(P1 p1,P2 p2,P3 p3)` | 将带有参数的Supplier转换为无参Supplier |
| `cn.hutool.core.lang.func.Supplier3` | `T get(P1 p1,P2 p2,P3 p3)` | 生成实例的方法 |
| `cn.hutool.core.lang.func.Supplier4` | `Supplier<T> toSupplier(P1 p1,P2 p2,P3 p3,P4 p4)` | 将带有参数的Supplier转换为无参Supplier |
| `cn.hutool.core.lang.func.Supplier4` | `T get(P1 p1,P2 p2,P3 p3,P4 p4)` | 生成实例的方法 |
| `cn.hutool.core.lang.func.Supplier5` | `Supplier<T> toSupplier(P1 p1,P2 p2,P3 p3,P4 p4,P5 p5)` | 将带有参数的Supplier转换为无参Supplier |
| `cn.hutool.core.lang.func.Supplier5` | `T get(P1 p1,P2 p2,P3 p3,P4 p4,P5 p5)` | 生成实例的方法 |
| `cn.hutool.core.lang.func.VoidFunc` | `void call(P... parameters)` | 执行函数 |
| `cn.hutool.core.lang.func.VoidFunc` | `void callWithRuntimeException(P... parameters)` | 执行函数，异常包装为RuntimeException |
| `cn.hutool.core.lang.func.VoidFunc0` | `void call()` | 执行函数 |
| `cn.hutool.core.lang.func.VoidFunc0` | `void callWithRuntimeException()` | 执行函数，异常包装为RuntimeException |
| `cn.hutool.core.lang.func.VoidFunc1` | `void call(P parameter)` | 执行函数 |
| `cn.hutool.core.lang.func.VoidFunc1` | `void callWithRuntimeException(P parameter)` | 执行函数，异常包装为RuntimeException |
