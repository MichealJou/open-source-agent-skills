# cn.hutool.log.level

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.log.level.DebugLog`

```java
public interface cn.hutool.log.level.DebugLog {
  public abstract boolean isDebugEnabled();
  public abstract void debug(java.lang.Throwable);
  public abstract void debug(java.lang.String, java.lang.Object...);
  public abstract void debug(java.lang.Throwable, java.lang.String, java.lang.Object...);
  public abstract void debug(java.lang.String, java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.log.level.ErrorLog`

```java
public interface cn.hutool.log.level.ErrorLog {
  public abstract boolean isErrorEnabled();
  public abstract void error(java.lang.Throwable);
  public abstract void error(java.lang.String, java.lang.Object...);
  public abstract void error(java.lang.Throwable, java.lang.String, java.lang.Object...);
  public abstract void error(java.lang.String, java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.log.level.InfoLog`

```java
public interface cn.hutool.log.level.InfoLog {
  public abstract boolean isInfoEnabled();
  public abstract void info(java.lang.Throwable);
  public abstract void info(java.lang.String, java.lang.Object...);
  public abstract void info(java.lang.Throwable, java.lang.String, java.lang.Object...);
  public abstract void info(java.lang.String, java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.log.level.Level`

```java
public final class cn.hutool.log.level.Level extends java.lang.Enum<cn.hutool.log.level.Level> {
  public static cn.hutool.log.level.Level[] values();
  public static cn.hutool.log.level.Level valueOf(java.lang.String);
}
```

## `cn.hutool.log.level.TraceLog`

```java
public interface cn.hutool.log.level.TraceLog {
  public abstract boolean isTraceEnabled();
  public abstract void trace(java.lang.Throwable);
  public abstract void trace(java.lang.String, java.lang.Object...);
  public abstract void trace(java.lang.Throwable, java.lang.String, java.lang.Object...);
  public abstract void trace(java.lang.String, java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.log.level.WarnLog`

```java
public interface cn.hutool.log.level.WarnLog {
  public abstract boolean isWarnEnabled();
  public abstract void warn(java.lang.Throwable);
  public abstract void warn(java.lang.String, java.lang.Object...);
  public abstract void warn(java.lang.Throwable, java.lang.String, java.lang.Object...);
  public abstract void warn(java.lang.String, java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```
