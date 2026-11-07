# cn.hutool.core.lang.caller

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.lang.caller.Caller` | `Class<?> getCaller()` | 获得调用者 |
| `cn.hutool.core.lang.caller.Caller` | `Class<?> getCaller(int depth)` | 获得调用者，指定第几级调用者 调用者层级关系： |
| `cn.hutool.core.lang.caller.Caller` | `Class<?> getCallerCaller()` | 获得调用者的调用者 |
| `cn.hutool.core.lang.caller.Caller` | `boolean isCalledBy(Class<?> clazz)` | 是否被指定类调用 |
| `cn.hutool.core.lang.caller.CallerUtil` | `Class<?> getCaller()` | 获得调用者 |
| `cn.hutool.core.lang.caller.CallerUtil` | `Class<?> getCaller(int depth)` | 获得调用者，指定第几级调用者 调用者层级关系： |
| `cn.hutool.core.lang.caller.CallerUtil` | `Class<?> getCallerCaller()` | 获得调用者的调用者 |
| `cn.hutool.core.lang.caller.CallerUtil` | `String getCallerMethodName(boolean isFullName)` | 获取调用此方法的方法名 |
| `cn.hutool.core.lang.caller.CallerUtil` | `boolean isCalledBy(Class<?> clazz)` | 是否被指定类调用 |
| `cn.hutool.core.lang.caller.SecurityManagerCaller` | `Class<?> getCaller()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.caller.SecurityManagerCaller` | `Class<?> getCaller(int depth)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.caller.SecurityManagerCaller` | `Class<?> getCallerCaller()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.caller.SecurityManagerCaller` | `boolean isCalledBy(Class<?> clazz)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.caller.StackTraceCaller` | `Class<?> getCaller()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.caller.StackTraceCaller` | `Class<?> getCaller(int depth)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.caller.StackTraceCaller` | `Class<?> getCallerCaller()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.caller.StackTraceCaller` | `boolean isCalledBy(Class<?> clazz)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
