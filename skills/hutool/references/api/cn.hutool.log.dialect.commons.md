# cn.hutool.log.dialect.commons

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.log.dialect.commons.ApacheCommonsLog`

```java
public class cn.hutool.log.dialect.commons.ApacheCommonsLog extends cn.hutool.log.AbstractLog {
  public cn.hutool.log.dialect.commons.ApacheCommonsLog(org.apache.commons.logging.Log, java.lang.String);
  public cn.hutool.log.dialect.commons.ApacheCommonsLog(java.lang.Class<?>);
  public cn.hutool.log.dialect.commons.ApacheCommonsLog(java.lang.String);
  public java.lang.String getName();
  public boolean isTraceEnabled();
  public void trace(java.lang.String, java.lang.Throwable, java.lang.String, java.lang.Object...);
  public boolean isDebugEnabled();
  public void debug(java.lang.String, java.lang.Throwable, java.lang.String, java.lang.Object...);
  public boolean isInfoEnabled();
  public void info(java.lang.String, java.lang.Throwable, java.lang.String, java.lang.Object...);
  public boolean isWarnEnabled();
  public void warn(java.lang.String, java.lang.Object...);
  public void warn(java.lang.Throwable, java.lang.String, java.lang.Object...);
  public void warn(java.lang.String, java.lang.Throwable, java.lang.String, java.lang.Object...);
  public boolean isErrorEnabled();
  public void error(java.lang.String, java.lang.Throwable, java.lang.String, java.lang.Object...);
  public void log(java.lang.String, cn.hutool.log.level.Level, java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.log.dialect.commons.ApacheCommonsLog4JLog`

```java
public class cn.hutool.log.dialect.commons.ApacheCommonsLog4JLog extends cn.hutool.log.dialect.log4j.Log4jLog {
  public cn.hutool.log.dialect.commons.ApacheCommonsLog4JLog(org.apache.commons.logging.Log);
  public cn.hutool.log.dialect.commons.ApacheCommonsLog4JLog(java.lang.Class<?>);
  public cn.hutool.log.dialect.commons.ApacheCommonsLog4JLog(java.lang.String);
}
```

## `cn.hutool.log.dialect.commons.ApacheCommonsLogFactory`

```java
public class cn.hutool.log.dialect.commons.ApacheCommonsLogFactory extends cn.hutool.log.LogFactory {
  public cn.hutool.log.dialect.commons.ApacheCommonsLogFactory();
  public cn.hutool.log.Log createLog(java.lang.String);
  public cn.hutool.log.Log createLog(java.lang.Class<?>);
}
```
