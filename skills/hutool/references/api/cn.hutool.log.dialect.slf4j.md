# cn.hutool.log.dialect.slf4j

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.log.dialect.slf4j.Slf4jLog`

```java
public class cn.hutool.log.dialect.slf4j.Slf4jLog extends cn.hutool.log.AbstractLog {
  public cn.hutool.log.dialect.slf4j.Slf4jLog(org.slf4j.Logger);
  public cn.hutool.log.dialect.slf4j.Slf4jLog(java.lang.Class<?>);
  public cn.hutool.log.dialect.slf4j.Slf4jLog(java.lang.String);
  public java.lang.String getName();
  public boolean isTraceEnabled();
  public void trace(java.lang.String, java.lang.Throwable, java.lang.String, java.lang.Object...);
  public boolean isDebugEnabled();
  public void debug(java.lang.String, java.lang.Throwable, java.lang.String, java.lang.Object...);
  public boolean isInfoEnabled();
  public void info(java.lang.String, java.lang.Throwable, java.lang.String, java.lang.Object...);
  public boolean isWarnEnabled();
  public void warn(java.lang.String, java.lang.Throwable, java.lang.String, java.lang.Object...);
  public boolean isErrorEnabled();
  public void error(java.lang.String, java.lang.Throwable, java.lang.String, java.lang.Object...);
  public void log(java.lang.String, cn.hutool.log.level.Level, java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.log.dialect.slf4j.Slf4jLogFactory`

```java
public class cn.hutool.log.dialect.slf4j.Slf4jLogFactory extends cn.hutool.log.LogFactory {
  public cn.hutool.log.dialect.slf4j.Slf4jLogFactory();
  public cn.hutool.log.dialect.slf4j.Slf4jLogFactory(boolean);
  public cn.hutool.log.Log createLog(java.lang.String);
  public cn.hutool.log.Log createLog(java.lang.Class<?>);
}
```
