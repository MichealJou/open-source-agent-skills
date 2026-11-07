# com.feilong.lib.ezmorph

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.ezmorph.IntegerValueUtil`

```java
public class com.feilong.lib.ezmorph.IntegerValueUtil {
  public com.feilong.lib.ezmorph.IntegerValueUtil();
  public static java.lang.String getIntegerValue(java.lang.Object);
}
```

## `com.feilong.lib.ezmorph.MorphException`

```java
public class com.feilong.lib.ezmorph.MorphException extends com.feilong.core.DefaultRuntimeException {
  public com.feilong.lib.ezmorph.MorphException(java.lang.String);
  public com.feilong.lib.ezmorph.MorphException(java.lang.String, java.lang.Throwable);
  public com.feilong.lib.ezmorph.MorphException(java.lang.Throwable);
}
```

## `com.feilong.lib.ezmorph.MorphUtils`

```java
public class com.feilong.lib.ezmorph.MorphUtils {
  public static void registerStandardMorphers(com.feilong.lib.ezmorph.MorpherRegistry);
}
```

## `com.feilong.lib.ezmorph.Morpher`

```java
public interface com.feilong.lib.ezmorph.Morpher {
  public abstract java.lang.Class<?> morphsTo();
  public abstract boolean supports(java.lang.Class<?>);
}
```

## `com.feilong.lib.ezmorph.MorpherRegistry`

```java
public class com.feilong.lib.ezmorph.MorpherRegistry implements java.io.Serializable {
  public com.feilong.lib.ezmorph.MorpherRegistry();
  public synchronized void clear();
  public synchronized com.feilong.lib.ezmorph.Morpher getMorpherFor(java.lang.Class<?>);
  public java.lang.Object morph(java.lang.Class<?>, java.lang.Object);
  public void registerMorpher(com.feilong.lib.ezmorph.Morpher);
}
```

## `com.feilong.lib.ezmorph.ObjectMorpher`

```java
public interface com.feilong.lib.ezmorph.ObjectMorpher extends com.feilong.lib.ezmorph.Morpher {
  public abstract java.lang.Object morph(java.lang.Object);
}
```
