# com.feilong.taglib.display

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.taglib.display.CacheContentBuilder`

```java
public interface com.feilong.taglib.display.CacheContentBuilder<T extends com.feilong.taglib.display.CacheParam, V> {
  public abstract V build(T);
}
```

## `com.feilong.taglib.display.LocaleSupportUtil`

```java
public final class com.feilong.taglib.display.LocaleSupportUtil {
  public static java.util.Locale toLocal(java.lang.Object, javax.servlet.http.HttpServletRequest);
  public static <T extends com.feilong.taglib.display.loadbundle.LoadBundleParam> java.util.Map<java.lang.String, java.lang.String> build(T);
}
```

## `com.feilong.taglib.display.SimpleTagParamCacheManager`

```java
public final class com.feilong.taglib.display.SimpleTagParamCacheManager {
  public static <T extends com.feilong.taglib.display.CacheParam, V> V getContent(T, com.feilong.taglib.display.CacheContentBuilder<T, V>);
}
```
