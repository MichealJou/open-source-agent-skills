# cn.hutool.log.dialect.tinylog

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.log.dialect.tinylog.TinyLog`

```java
public class cn.hutool.log.dialect.tinylog.TinyLog extends cn.hutool.log.AbstractLog {
  public cn.hutool.log.dialect.tinylog.TinyLog(java.lang.Class<?>);
  public cn.hutool.log.dialect.tinylog.TinyLog(java.lang.String);
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
  public boolean isEnabled(cn.hutool.log.level.Level);
}
```

## `cn.hutool.log.dialect.tinylog.TinyLog2`

```java
public class cn.hutool.log.dialect.tinylog.TinyLog2 extends cn.hutool.log.AbstractLog {
  public cn.hutool.log.dialect.tinylog.TinyLog2(java.lang.Class<?>);
  public cn.hutool.log.dialect.tinylog.TinyLog2(java.lang.String);
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
  public boolean isEnabled(cn.hutool.log.level.Level);
}
```

## `cn.hutool.log.dialect.tinylog.TinyLog2Factory`

```java
public class cn.hutool.log.dialect.tinylog.TinyLog2Factory extends cn.hutool.log.LogFactory {
  public cn.hutool.log.dialect.tinylog.TinyLog2Factory();
  public cn.hutool.log.Log createLog(java.lang.String);
  public cn.hutool.log.Log createLog(java.lang.Class<?>);
}
```

## `cn.hutool.log.dialect.tinylog.TinyLogFactory`

```java
public class cn.hutool.log.dialect.tinylog.TinyLogFactory extends cn.hutool.log.LogFactory {
  public cn.hutool.log.dialect.tinylog.TinyLogFactory();
  public cn.hutool.log.Log createLog(java.lang.String);
  public cn.hutool.log.Log createLog(java.lang.Class<?>);
}
```
