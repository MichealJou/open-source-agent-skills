# cn.hutool.core.lang.caller

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.lang.caller.Caller`

```java
public interface cn.hutool.core.lang.caller.Caller {
  public abstract java.lang.Class<?> getCaller();
  public abstract java.lang.Class<?> getCallerCaller();
  public abstract java.lang.Class<?> getCaller(int);
  public abstract boolean isCalledBy(java.lang.Class<?>);
}
```

## `cn.hutool.core.lang.caller.CallerUtil`

```java
public class cn.hutool.core.lang.caller.CallerUtil {
  public cn.hutool.core.lang.caller.CallerUtil();
  public static java.lang.Class<?> getCaller();
  public static java.lang.Class<?> getCallerCaller();
  public static java.lang.Class<?> getCaller(int);
  public static boolean isCalledBy(java.lang.Class<?>);
  public static java.lang.String getCallerMethodName(boolean);
}
```

## `cn.hutool.core.lang.caller.SecurityManagerCaller`

```java
public class cn.hutool.core.lang.caller.SecurityManagerCaller extends java.lang.SecurityManager implements cn.hutool.core.lang.caller.Caller,java.io.Serializable {
  public cn.hutool.core.lang.caller.SecurityManagerCaller();
  public java.lang.Class<?> getCaller();
  public java.lang.Class<?> getCallerCaller();
  public java.lang.Class<?> getCaller(int);
  public boolean isCalledBy(java.lang.Class<?>);
}
```

## `cn.hutool.core.lang.caller.StackTraceCaller`

```java
public class cn.hutool.core.lang.caller.StackTraceCaller implements cn.hutool.core.lang.caller.Caller,java.io.Serializable {
  public cn.hutool.core.lang.caller.StackTraceCaller();
  public java.lang.Class<?> getCaller();
  public java.lang.Class<?> getCallerCaller();
  public java.lang.Class<?> getCaller(int);
  public boolean isCalledBy(java.lang.Class<?>);
}
```
