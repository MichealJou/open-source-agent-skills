# com.feilong.context.format

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.context.format.AbstractStringFormatter`

```java
public abstract class com.feilong.context.format.AbstractStringFormatter implements com.feilong.context.format.StringFormatter {
  public com.feilong.context.format.AbstractStringFormatter();
  public java.lang.String format(java.lang.String);
}
```

## `com.feilong.context.format.JsonStringFormatter`

```java
public class com.feilong.context.format.JsonStringFormatter extends com.feilong.context.format.AbstractStringFormatter {
  public com.feilong.context.format.JsonStringFormatter();
}
```

## `com.feilong.context.format.StringFormatter`

```java
public interface com.feilong.context.format.StringFormatter {
  public abstract java.lang.String format(java.lang.String);
}
```

## `com.feilong.context.format.XMLStringFormatter`

```java
public class com.feilong.context.format.XMLStringFormatter extends com.feilong.context.format.AbstractStringFormatter {
  public com.feilong.context.format.XMLStringFormatter();
}
```
