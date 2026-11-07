# cn.hutool.log

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.log.AbstractLog` | `boolean isEnabled(Level level)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.log.AbstractLog` | `void debug(String format,Object... arguments)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.log.AbstractLog` | `void debug(Throwable t)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.log.AbstractLog` | `void debug(Throwable t,String format,Object... arguments)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.log.AbstractLog` | `void error(String format,Object... arguments)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.log.AbstractLog` | `void error(Throwable t)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.log.AbstractLog` | `void error(Throwable t,String format,Object... arguments)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.log.AbstractLog` | `void info(String format,Object... arguments)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.log.AbstractLog` | `void info(Throwable t)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.log.AbstractLog` | `void info(Throwable t,String format,Object... arguments)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.log.AbstractLog` | `void log(Level level,String format,Object... arguments)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.log.AbstractLog` | `void log(Level level,Throwable t,String format,Object... arguments)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.log.AbstractLog` | `void trace(String format,Object... arguments)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.log.AbstractLog` | `void trace(Throwable t)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.log.AbstractLog` | `void trace(Throwable t,String format,Object... arguments)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.log.AbstractLog` | `void warn(String format,Object... arguments)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.log.AbstractLog` | `void warn(Throwable t)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.log.AbstractLog` | `void warn(Throwable t,String format,Object... arguments)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.log.GlobalLogFactory` | `LogFactory get()` | 获取单例日志工厂类，如果不存在创建之 |
| `cn.hutool.log.GlobalLogFactory` | `LogFactory set(Class<? extends LogFactory> logFactoryClass)` | 自定义日志实现 |
| `cn.hutool.log.GlobalLogFactory` | `LogFactory set(LogFactory logFactory)` | 自定义日志实现 |
| `cn.hutool.log.Log` | `Log get()` | @return 获得日志，自动判定日志发出者 |
| `cn.hutool.log.Log` | `Log get(Class<?> clazz)` | 获得Log |
| `cn.hutool.log.Log` | `Log get(String name)` | 获得Log |
| `cn.hutool.log.Log` | `String getName()` | @return 日志对象的Name |
| `cn.hutool.log.Log` | `boolean isEnabled(Level level)` | 是否开启指定日志 |
| `cn.hutool.log.Log` | `void log(Level level,String format,Object... arguments)` | 打印指定级别的日志 |
| `cn.hutool.log.Log` | `void log(Level level,Throwable t,String format,Object... arguments)` | 打印 指定级别的日志 |
| `cn.hutool.log.Log` | `void log(String fqcn,Level level,Throwable t,String format,Object... arguments)` | 打印 ERROR 等级的日志 |
| `cn.hutool.log.LogFactory` | `Log createLog(Class<?> clazz)` | 创建日志对象 |
| `cn.hutool.log.LogFactory` | `Log createLog(String name)` | 创建日志对象 |
| `cn.hutool.log.LogFactory` | `Log get()` | @return 获得调用者的日志 |
| `cn.hutool.log.LogFactory` | `Log get(Class<?> clazz)` | 获得日志对象 |
| `cn.hutool.log.LogFactory` | `Log get(String name)` | 获得日志对象 |
| `cn.hutool.log.LogFactory` | `Log getLog(Class<?> clazz)` | 获得日志对象 |
| `cn.hutool.log.LogFactory` | `Log getLog(String name)` | 获得日志对象 |
| `cn.hutool.log.LogFactory` | `LogFactory create()` | 决定日志实现 依次按照顺序检查日志库的jar是否被引入，如果未引入任何日志库，则检查ClassPath下的logging.properties，存在则使用JdkLogFactory，否则使用ConsoleLogFactory |
| `cn.hutool.log.LogFactory` | `LogFactory getCurrentLogFactory()` | @return 当前使用的日志工厂 |
| `cn.hutool.log.LogFactory` | `LogFactory setCurrentLogFactory(Class<? extends LogFactory> logFactoryClass)` | 自定义日志实现 |
| `cn.hutool.log.LogFactory` | `LogFactory setCurrentLogFactory(LogFactory logFactory)` | 自定义日志实现 |
| `cn.hutool.log.LogFactory` | `String getName()` | 获取日志框架名，用于打印当前所用日志框架 |
| `cn.hutool.log.StaticLog` | `Log get()` | @return 获得日志，自动判定日志发出者 |
| `cn.hutool.log.StaticLog` | `Log get(Class<?> clazz)` | 获得Log |
| `cn.hutool.log.StaticLog` | `Log get(String name)` | 获得Log |
| `cn.hutool.log.StaticLog` | `void debug(Log log,String format,Object... arguments)` | Debug等级日志，小于Info |
| `cn.hutool.log.StaticLog` | `void debug(String format,Object... arguments)` | Debug等级日志，小于Info 由于动态获取Log，效率较低，建议在非频繁调用的情况下使用！！ |
| `cn.hutool.log.StaticLog` | `void error(Log log,String format,Object... arguments)` | Error等级日志 |
| `cn.hutool.log.StaticLog` | `void error(Log log,Throwable e)` | Error等级日志 |
| `cn.hutool.log.StaticLog` | `void error(Log log,Throwable e,String format,Object... arguments)` | Error等级日志 |
| `cn.hutool.log.StaticLog` | `void error(String format,Object... arguments)` | Error等级日志 由于动态获取Log，效率较低，建议在非频繁调用的情况下使用！！ |
| `cn.hutool.log.StaticLog` | `void error(Throwable e)` | Error等级日志 由于动态获取Log，效率较低，建议在非频繁调用的情况下使用！！ |
| `cn.hutool.log.StaticLog` | `void error(Throwable e,String format,Object... arguments)` | Error等级日志 由于动态获取Log，效率较低，建议在非频繁调用的情况下使用！！ |
| `cn.hutool.log.StaticLog` | `void info(Log log,String format,Object... arguments)` | Info等级日志，小于Warn |
| `cn.hutool.log.StaticLog` | `void info(String format,Object... arguments)` | Info等级日志，小于Warn 由于动态获取Log，效率较低，建议在非频繁调用的情况下使用！！ |
| `cn.hutool.log.StaticLog` | `void log(Level level,Throwable t,String format,Object... arguments)` | 打印日志 |
| `cn.hutool.log.StaticLog` | `void trace(Log log,String format,Object... arguments)` | Trace等级日志，小于Debug |
| `cn.hutool.log.StaticLog` | `void trace(String format,Object... arguments)` | Trace等级日志，小于debug 由于动态获取Log，效率较低，建议在非频繁调用的情况下使用！！ |
| `cn.hutool.log.StaticLog` | `void warn(Log log,String format,Object... arguments)` | Warn等级日志，小于Error |
| `cn.hutool.log.StaticLog` | `void warn(Log log,Throwable e,String format,Object... arguments)` | Warn等级日志，小于Error |
| `cn.hutool.log.StaticLog` | `void warn(String format,Object... arguments)` | Warn等级日志，小于Error 由于动态获取Log，效率较低，建议在非频繁调用的情况下使用！！ |
| `cn.hutool.log.StaticLog` | `void warn(Throwable e,String format,Object... arguments)` | Warn等级日志，小于Error 由于动态获取Log，效率较低，建议在非频繁调用的情况下使用！！ |
