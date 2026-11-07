# com.feilong.tools.slf4j

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.tools.slf4j.Slf4jUtil` | `String format(String messagePattern,Object... args)` | 格式化字符串,此方法是抽取slf4j的核心方法. 在java中,常会拼接字符串生成新的字符串值,在字符串拼接过程中容易写错或者位置写错 slf4j的log支持格式化输出log,比如: log.debug("{}","feilong"); log.info("{},{}","feilong","hello"); 这些写法非常简洁且有效,不易出错 因此,你可以在代码中出现这样的写法: |
| `com.feilong.tools.slf4j.Slf4jUtil` | `boolean isEnabledDebug(String logLevel)` | 判断指定的logvel 是否小于等于debug级别. 使用场景: 可以使用配置中心来控制类的日志级别, 而不需要每次修改log4j xml 或者logback xml 配置文件再重新发布 |
| `com.feilong.tools.slf4j.Slf4jUtil` | `boolean isEnabledInfo(String logLevel)` | 判断指定的logvel 是否小于等于info级别. 使用场景: 可以使用配置中心来控制类的日志级别, 而不需要每次修改log4j xml 或者logback xml 配置文件再重新发布 |
