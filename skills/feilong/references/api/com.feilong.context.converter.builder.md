# com.feilong.context.converter.builder

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.context.converter.builder.AliasBeanBuilder`

```java
public class com.feilong.context.converter.builder.AliasBeanBuilder implements com.feilong.context.converter.builder.BeanBuilder {
  public com.feilong.context.converter.builder.AliasBeanBuilder();
  public <T> T build(java.util.Map<java.lang.String, java.lang.String>, T);
}
```

## `com.feilong.context.converter.builder.BeanBuilder`

```java
public interface com.feilong.context.converter.builder.BeanBuilder {
  public abstract <T> T build(java.util.Map<java.lang.String, java.lang.String>, T);
}
```

## `com.feilong.context.converter.builder.CommonBeanBuilder`

```java
public class com.feilong.context.converter.builder.CommonBeanBuilder implements com.feilong.context.converter.builder.BeanBuilder {
  public com.feilong.context.converter.builder.CommonBeanBuilder();
  public <T> T build(java.util.Map<java.lang.String, java.lang.String>, T);
}
```

## `com.feilong.context.converter.builder.NameAndValueMapBuilder`

```java
public interface com.feilong.context.converter.builder.NameAndValueMapBuilder {
  public abstract java.util.Map<java.lang.String, java.lang.String> build(java.lang.String);
}
```

## `com.feilong.context.converter.builder.XmlNodeAttributeValueAndValueMapBuilder`

```java
public class com.feilong.context.converter.builder.XmlNodeAttributeValueAndValueMapBuilder implements com.feilong.context.converter.builder.NameAndValueMapBuilder {
  public com.feilong.context.converter.builder.XmlNodeAttributeValueAndValueMapBuilder();
  public com.feilong.context.converter.builder.XmlNodeAttributeValueAndValueMapBuilder(java.lang.String, java.lang.String);
  public java.util.Map<java.lang.String, java.lang.String> build(java.lang.String);
  public java.lang.String getXpathExpression();
  public void setXpathExpression(java.lang.String);
  public java.lang.String getNodeAttributeName();
  public void setNodeAttributeName(java.lang.String);
}
```

## `com.feilong.context.converter.builder.XmlNodeNameAndValueMapBuilder`

```java
public class com.feilong.context.converter.builder.XmlNodeNameAndValueMapBuilder implements com.feilong.context.converter.builder.NameAndValueMapBuilder {
  public com.feilong.context.converter.builder.XmlNodeNameAndValueMapBuilder();
  public com.feilong.context.converter.builder.XmlNodeNameAndValueMapBuilder(java.lang.String);
  public java.util.Map<java.lang.String, java.lang.String> build(java.lang.String);
  public java.lang.String getXpathExpression();
  public void setXpathExpression(java.lang.String);
}
```
