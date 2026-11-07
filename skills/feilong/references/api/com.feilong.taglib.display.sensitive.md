# com.feilong.taglib.display.sensitive

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.taglib.display.sensitive.SensitiveConfig`

```java
public class com.feilong.taglib.display.sensitive.SensitiveConfig {
  public com.feilong.taglib.display.sensitive.SensitiveConfig(java.lang.String);
  public com.feilong.taglib.display.sensitive.SensitiveConfig(java.lang.String, char);
  public com.feilong.taglib.display.sensitive.SensitiveConfig(com.feilong.taglib.display.sensitive.SensitiveType);
  public com.feilong.taglib.display.sensitive.SensitiveConfig(com.feilong.taglib.display.sensitive.SensitiveType, char);
  public char getMaskChar();
  public void setMaskChar(char);
  public java.lang.String getType();
  public void setType(java.lang.String);
}
```

## `com.feilong.taglib.display.sensitive.SensitivePropertiesConfig`

```java
public final class com.feilong.taglib.display.sensitive.SensitivePropertiesConfig {
  public static java.lang.Integer[] load(java.lang.String);
}
```

## `com.feilong.taglib.display.sensitive.SensitiveTag`

```java
public class com.feilong.taglib.display.sensitive.SensitiveTag extends com.feilong.taglib.AbstractStartWriteContentTag {
  public com.feilong.taglib.display.sensitive.SensitiveTag();
  public void setValue(java.lang.String);
  public void setType(java.lang.String);
  public void setMaskChar(char);
}
```

## `com.feilong.taglib.display.sensitive.SensitiveType`

```java
public abstract class com.feilong.taglib.display.sensitive.SensitiveType extends java.lang.Enum<com.feilong.taglib.display.sensitive.SensitiveType> {
  public static com.feilong.taglib.display.sensitive.SensitiveType[] values();
  public static com.feilong.taglib.display.sensitive.SensitiveType valueOf(java.lang.String);
  public static com.feilong.taglib.display.sensitive.SensitiveType toSensitiveType(java.lang.String);
  public java.lang.String getType();
}
```

## `com.feilong.taglib.display.sensitive.SensitiveUtil`

```java
public final class com.feilong.taglib.display.sensitive.SensitiveUtil {
  public static java.lang.String parse(java.lang.String, com.feilong.taglib.display.sensitive.SensitiveConfig);
  public static java.lang.String parse(java.lang.String, char, int, int);
}
```
