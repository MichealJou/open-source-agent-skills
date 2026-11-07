# cn.hutool.log

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.log.AbstractLog`

```java
public abstract class cn.hutool.log.AbstractLog implements cn.hutool.log.Log,java.io.Serializable {
  public cn.hutool.log.AbstractLog();
  public boolean isEnabled(cn.hutool.log.level.Level);
  public void trace(java.lang.Throwable);
  public void trace(java.lang.String, java.lang.Object...);
  public void trace(java.lang.Throwable, java.lang.String, java.lang.Object...);
  public void debug(java.lang.Throwable);
  public void debug(java.lang.String, java.lang.Object...);
  public void debug(java.lang.Throwable, java.lang.String, java.lang.Object...);
  public void info(java.lang.Throwable);
  public void info(java.lang.String, java.lang.Object...);
  public void info(java.lang.Throwable, java.lang.String, java.lang.Object...);
  public void warn(java.lang.Throwable);
  public void warn(java.lang.String, java.lang.Object...);
  public void warn(java.lang.Throwable, java.lang.String, java.lang.Object...);
  public void error(java.lang.Throwable);
  public void error(java.lang.String, java.lang.Object...);
  public void error(java.lang.Throwable, java.lang.String, java.lang.Object...);
  public void log(cn.hutool.log.level.Level, java.lang.String, java.lang.Object...);
  public void log(cn.hutool.log.level.Level, java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.log.GlobalLogFactory`

```java
public class cn.hutool.log.GlobalLogFactory {
  public cn.hutool.log.GlobalLogFactory();
  public static cn.hutool.log.LogFactory get();
  public static cn.hutool.log.LogFactory set(java.lang.Class<? extends cn.hutool.log.LogFactory>);
  public static cn.hutool.log.LogFactory set(cn.hutool.log.LogFactory);
}
```

## `cn.hutool.log.Log`

```java
public interface cn.hutool.log.Log extends cn.hutool.log.level.TraceLog,cn.hutool.log.level.DebugLog,cn.hutool.log.level.InfoLog,cn.hutool.log.level.WarnLog,cn.hutool.log.level.ErrorLog {
  public static cn.hutool.log.Log get(java.lang.Class<?>);
  public static cn.hutool.log.Log get(java.lang.String);
  public static cn.hutool.log.Log get();
  public abstract java.lang.String getName();
  public abstract boolean isEnabled(cn.hutool.log.level.Level);
  public abstract void log(cn.hutool.log.level.Level, java.lang.String, java.lang.Object...);
  public abstract void log(cn.hutool.log.level.Level, java.lang.Throwable, java.lang.String, java.lang.Object...);
  public abstract void log(java.lang.String, cn.hutool.log.level.Level, java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.log.LogFactory`

```java
public abstract class cn.hutool.log.LogFactory {
  public cn.hutool.log.LogFactory(java.lang.String);
  public java.lang.String getName();
  public cn.hutool.log.Log getLog(java.lang.String);
  public cn.hutool.log.Log getLog(java.lang.Class<?>);
  public abstract cn.hutool.log.Log createLog(java.lang.String);
  public abstract cn.hutool.log.Log createLog(java.lang.Class<?>);
  public static cn.hutool.log.LogFactory getCurrentLogFactory();
  public static cn.hutool.log.LogFactory setCurrentLogFactory(java.lang.Class<? extends cn.hutool.log.LogFactory>);
  public static cn.hutool.log.LogFactory setCurrentLogFactory(cn.hutool.log.LogFactory);
  public static cn.hutool.log.Log get(java.lang.String);
  public static cn.hutool.log.Log get(java.lang.Class<?>);
  public static cn.hutool.log.Log get();
  public static cn.hutool.log.LogFactory create();
}
```

## `cn.hutool.log.StaticLog`

```java
public final class cn.hutool.log.StaticLog {
  public static void trace(java.lang.String, java.lang.Object...);
  public static void trace(cn.hutool.log.Log, java.lang.String, java.lang.Object...);
  public static void debug(java.lang.String, java.lang.Object...);
  public static void debug(cn.hutool.log.Log, java.lang.String, java.lang.Object...);
  public static void info(java.lang.String, java.lang.Object...);
  public static void info(cn.hutool.log.Log, java.lang.String, java.lang.Object...);
  public static void warn(java.lang.String, java.lang.Object...);
  public static void warn(java.lang.Throwable, java.lang.String, java.lang.Object...);
  public static void warn(cn.hutool.log.Log, java.lang.String, java.lang.Object...);
  public static void warn(cn.hutool.log.Log, java.lang.Throwable, java.lang.String, java.lang.Object...);
  public static void error(java.lang.Throwable);
  public static void error(java.lang.String, java.lang.Object...);
  public static void error(java.lang.Throwable, java.lang.String, java.lang.Object...);
  public static void error(cn.hutool.log.Log, java.lang.Throwable);
  public static void error(cn.hutool.log.Log, java.lang.String, java.lang.Object...);
  public static void error(cn.hutool.log.Log, java.lang.Throwable, java.lang.String, java.lang.Object...);
  public static void log(cn.hutool.log.level.Level, java.lang.Throwable, java.lang.String, java.lang.Object...);
  public static cn.hutool.log.Log get(java.lang.Class<?>);
  public static cn.hutool.log.Log get(java.lang.String);
  public static cn.hutool.log.Log get();
}
```
