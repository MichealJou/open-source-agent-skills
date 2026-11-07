# cn.hutool.core.exceptions

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.exceptions.CheckedUtil` | `Func0Rt<R> uncheck(Func0<R> expression)` | 接收一个可以转化成 cn.hutool.core.lang.func.Func0 的Lambda表达式，当执行表达式抛出任何异常的时候，都会转化成运行时异常 如此一来，代码中就不用显示的try-catch转化成运行时异常 |
| `cn.hutool.core.exceptions.CheckedUtil` | `Func0Rt<R> uncheck(Func0<R> expression,Supplier1<RuntimeException, Exception> rteSupplier)` | 接收一个可以转化成 cn.hutool.core.lang.func.Func0的Lambda表达式，和一个可以把Exception转化成RuntimeExceptionde的表达式，当执行表达式抛出任何异常的时候，都会转化成运行时异常 如此一来，代码中就不用显示的try-catch转化成运行时异常 |
| `cn.hutool.core.exceptions.CheckedUtil` | `Func1Rt<P, R> uncheck(Func1<P, R> expression)` | 接收一个可以转化成 cn.hutool.core.lang.func.Func1 的Lambda表达式，当执行表达式抛出任何异常的时候，都会转化成运行时异常 如此一来，代码中就不用显示的try-catch转化成运行时异常 |
| `cn.hutool.core.exceptions.CheckedUtil` | `Func1Rt<P, R> uncheck(Func1<P, R> expression,Supplier1<RuntimeException, Exception> rteSupplier)` | 接收一个可以转化成 cn.hutool.core.lang.func.Func1的Lambda表达式，和一个可以把Exception转化成RuntimeExceptionde的表达式，当执行表达式抛出任何异常的时候，都会转化成运行时异常 如此一来，代码中就不用显示的try-catch转化成运行时异常 |
| `cn.hutool.core.exceptions.CheckedUtil` | `FuncRt<P, R> uncheck(Func<P, R> expression)` | 接收一个可以转化成 cn.hutool.core.lang.func.Func 的Lambda表达式，当执行表达式抛出任何异常的时候，都会转化成运行时异常 如此一来，代码中就不用显示的try-catch转化成运行时异常 |
| `cn.hutool.core.exceptions.CheckedUtil` | `FuncRt<P, R> uncheck(Func<P, R> expression,Supplier1<RuntimeException, Exception> rteSupplier)` | 接收一个可以转化成 cn.hutool.core.lang.func.Func的Lambda表达式，和一个可以把Exception转化成RuntimeExceptionde的表达式，当执行表达式抛出任何异常的时候，都会转化成运行时异常 如此一来，代码中就不用显示的try-catch转化成运行时异常 |
| `cn.hutool.core.exceptions.CheckedUtil` | `VoidFunc0Rt uncheck(VoidFunc0 expression)` | 接收一个可以转化成 cn.hutool.core.lang.func.VoidFunc0 的Lambda表达式，当执行表达式抛出任何异常的时候，都会转化成运行时异常 如此一来，代码中就不用显示的try-catch转化成运行时异常 |
| `cn.hutool.core.exceptions.CheckedUtil` | `VoidFunc0Rt uncheck(VoidFunc0 expression,RuntimeException rte)` | 接收一个可以转化成 cn.hutool.core.lang.func.VoidFunc0的Lambda表达式，和一个RuntimeException，当执行表达式抛出任何异常的时候，都会转化成运行时异常 如此一来，代码中就不用显示的try-catch转化成运行时异常 |
| `cn.hutool.core.exceptions.CheckedUtil` | `VoidFunc0Rt uncheck(VoidFunc0 expression,Supplier1<RuntimeException, Exception> rteSupplier)` | 接收一个可以转化成 cn.hutool.core.lang.func.VoidFunc0的Lambda表达式，和一个可以把Exception转化成RuntimeExceptionde的表达式，当执行表达式抛出任何异常的时候，都会转化成运行时异常 如此一来，代码中就不用显示的try-catch转化成运行时异常 |
| `cn.hutool.core.exceptions.CheckedUtil` | `VoidFunc1Rt<P> uncheck(VoidFunc1<P> expression)` | 接收一个可以转化成 cn.hutool.core.lang.func.VoidFunc1 的Lambda表达式，当执行表达式抛出任何异常的时候，都会转化成运行时异常 如此一来，代码中就不用显示的try-catch转化成运行时异常 |
| `cn.hutool.core.exceptions.CheckedUtil` | `VoidFunc1Rt<P> uncheck(VoidFunc1<P> expression,Supplier1<RuntimeException, Exception> rteSupplier)` | 接收一个可以转化成 cn.hutool.core.lang.func.VoidFunc1的Lambda表达式，和一个RuntimeException，当执行表达式抛出任何异常的时候，都会转化成运行时异常 如此一来，代码中就不用显示的try-catch转化成运行时异常 |
| `cn.hutool.core.exceptions.CheckedUtil` | `VoidFuncRt<P> uncheck(VoidFunc<P> expression)` | 接收一个可以转化成 cn.hutool.core.lang.func.VoidFunc 的Lambda表达式，当执行表达式抛出任何异常的时候，都会转化成运行时异常 如此一来，代码中就不用显示的try-catch转化成运行时异常 |
| `cn.hutool.core.exceptions.CheckedUtil` | `VoidFuncRt<P> uncheck(VoidFunc<P> expression,Supplier1<RuntimeException, Exception> rteSupplier)` | 接收一个可以转化成 cn.hutool.core.lang.func.VoidFunc的Lambda表达式，和一个可以把Exception转化成RuntimeExceptionde的表达式，当执行表达式抛出任何异常的时候，都会转化成运行时异常 如此一来，代码中就不用显示的try-catch转化成运行时异常 |
| `cn.hutool.core.exceptions.CheckedUtil$Func0Rt` | `R call()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.exceptions.CheckedUtil$Func1Rt` | `R call(P parameter)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.exceptions.CheckedUtil$FuncRt` | `R call(P... parameters)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.exceptions.CheckedUtil$VoidFunc0Rt` | `void call()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.exceptions.CheckedUtil$VoidFunc1Rt` | `void call(P parameter)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.exceptions.CheckedUtil$VoidFuncRt` | `void call(P... parameters)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.exceptions.ExceptionUtil` | `List<Throwable> getThrowableList(Throwable throwable)` | 获取异常链上所有异常的集合，如果Throwable 对象没有cause，返回只有一个节点的List 如果传入null，返回空集合 此方法来自Apache-Commons-Lang3 |
| `cn.hutool.core.exceptions.ExceptionUtil` | `RuntimeException wrapRuntime(String message)` | 将指定的消息包装为运行时异常 |
| `cn.hutool.core.exceptions.ExceptionUtil` | `RuntimeException wrapRuntime(Throwable throwable)` | 使用运行时异常包装编译异常 如果传入参数已经是运行时异常，则直接返回，不再额外包装 |
| `cn.hutool.core.exceptions.ExceptionUtil` | `StackTraceElement getRootStackElement()` | 获取入口堆栈信息 |
| `cn.hutool.core.exceptions.ExceptionUtil` | `StackTraceElement getStackElement(String fqcn,int i)` | 获取指定层的堆栈信息 |
| `cn.hutool.core.exceptions.ExceptionUtil` | `StackTraceElement getStackElement(int i)` | 获取指定层的堆栈信息 |
| `cn.hutool.core.exceptions.ExceptionUtil` | `StackTraceElement[] getStackElements()` | 获取当前栈信息 |
| `cn.hutool.core.exceptions.ExceptionUtil` | `String getMessage(Throwable e)` | 获得完整消息，包括异常名，消息格式为：{SimpleClassName}: {ThrowableMessage} |
| `cn.hutool.core.exceptions.ExceptionUtil` | `String getRootCauseMessage(final Throwable th)` | 获取异常链中最尾端的异常的消息，消息格式为：{SimpleClassName}: {ThrowableMessage} |
| `cn.hutool.core.exceptions.ExceptionUtil` | `String getSimpleMessage(Throwable e)` | 获得消息，调用异常类的getMessage方法 |
| `cn.hutool.core.exceptions.ExceptionUtil` | `String stacktraceToOneLineString(Throwable throwable)` | 堆栈转为单行完整字符串 |
| `cn.hutool.core.exceptions.ExceptionUtil` | `String stacktraceToOneLineString(Throwable throwable,int limit)` | 堆栈转为单行完整字符串 |
| `cn.hutool.core.exceptions.ExceptionUtil` | `String stacktraceToString(Throwable throwable)` | 堆栈转为完整字符串 |
| `cn.hutool.core.exceptions.ExceptionUtil` | `String stacktraceToString(Throwable throwable,int limit)` | 堆栈转为完整字符串 |
| `cn.hutool.core.exceptions.ExceptionUtil` | `String stacktraceToString(Throwable throwable,int limit,Map<Character, String> replaceCharToStrMap)` | 堆栈转为完整字符串 |
| `cn.hutool.core.exceptions.ExceptionUtil` | `T convertFromOrSuppressedThrowable(Throwable throwable,Class<T> exceptionClass)` | 转化指定异常为来自或者包含指定异常 |
| `cn.hutool.core.exceptions.ExceptionUtil` | `T convertFromOrSuppressedThrowable(Throwable throwable,Class<T> exceptionClass,boolean checkCause)` | 转化指定异常为来自或者包含指定异常 |
| `cn.hutool.core.exceptions.ExceptionUtil` | `T wrap(Throwable throwable,Class<T> wrapThrowable)` | 包装一个异常 |
| `cn.hutool.core.exceptions.ExceptionUtil` | `Throwable getCausedBy(Throwable throwable,Class<? extends Exception>... causeClasses)` | 获取由指定异常类引起的异常 |
| `cn.hutool.core.exceptions.ExceptionUtil` | `Throwable getRootCause(final Throwable throwable)` | 获取异常链中最尾端的异常，即异常最早发生的异常对象。 此方法通过调用Throwable#getCause() 直到没有cause为止，如果异常本身没有cause，返回异常本身 传入null返回也为null 此方法来自Apache-Commons-Lang3 |
| `cn.hutool.core.exceptions.ExceptionUtil` | `Throwable unwrap(Throwable wrapped)` | 剥离反射引发的InvocationTargetException、UndeclaredThrowableException中间异常，返回业务本身的异常 |
| `cn.hutool.core.exceptions.ExceptionUtil` | `boolean isCausedBy(Throwable throwable,Class<? extends Exception>... causeClasses)` | 判断是否由指定异常类引起 |
| `cn.hutool.core.exceptions.ExceptionUtil` | `boolean isFromOrSuppressedThrowable(Throwable throwable,Class<? extends Throwable> exceptionClass)` | 判断指定异常是否来自或者包含指定异常 |
| `cn.hutool.core.exceptions.ExceptionUtil` | `boolean isFromOrSuppressedThrowable(Throwable throwable,Class<? extends Throwable> exceptionClass,boolean checkCause)` | 判断指定异常是否来自或者包含指定异常 |
| `cn.hutool.core.exceptions.ExceptionUtil` | `void wrapAndThrow(Throwable throwable)` | 包装异常并重新抛出此异常 RuntimeException 和Error 直接抛出，其它检查异常包装为UndeclaredThrowableException 后抛出 |
| `cn.hutool.core.exceptions.ExceptionUtil` | `void wrapRuntimeAndThrow(String message)` | 将消息包装为运行时异常并抛出 |
| `cn.hutool.core.exceptions.StatefulException` | `int getStatus()` | @return 获得异常状态码 |
