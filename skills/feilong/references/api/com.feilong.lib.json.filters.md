# com.feilong.lib.json.filters

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.json.filters.AndPropertyFilter`

```java
public class com.feilong.lib.json.filters.AndPropertyFilter implements com.feilong.lib.json.util.PropertyFilter {
  public com.feilong.lib.json.filters.AndPropertyFilter(com.feilong.lib.json.util.PropertyFilter, com.feilong.lib.json.util.PropertyFilter);
  public boolean apply(java.lang.Object, java.lang.String, java.lang.Object);
}
```

## `com.feilong.lib.json.filters.NotPropertyFilter`

```java
public class com.feilong.lib.json.filters.NotPropertyFilter implements com.feilong.lib.json.util.PropertyFilter {
  public com.feilong.lib.json.filters.NotPropertyFilter(com.feilong.lib.json.util.PropertyFilter);
  public boolean apply(java.lang.Object, java.lang.String, java.lang.Object);
}
```

## `com.feilong.lib.json.filters.OrPropertyFilter`

```java
public class com.feilong.lib.json.filters.OrPropertyFilter implements com.feilong.lib.json.util.PropertyFilter {
  public com.feilong.lib.json.filters.OrPropertyFilter(com.feilong.lib.json.util.PropertyFilter...);
  public boolean apply(java.lang.Object, java.lang.String, java.lang.Object);
}
```
