# com.feilong.context.converter

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.context.converter.AbstractBeanClassStringToBeanConverter`

```java
public abstract class com.feilong.context.converter.AbstractBeanClassStringToBeanConverter<T> extends com.feilong.context.converter.AbstractStringToBeanConverter<T> {
  public com.feilong.context.converter.AbstractBeanClassStringToBeanConverter();
  public java.lang.Class<T> getBeanClass();
  public void setBeanClass(java.lang.Class<T>);
}
```

## `com.feilong.context.converter.AbstractStringToBeanConverter`

```java
public abstract class com.feilong.context.converter.AbstractStringToBeanConverter<T> implements com.feilong.context.converter.StringToBeanConverter<T> {
  public com.feilong.context.converter.AbstractStringToBeanConverter();
  public T convert(java.lang.String);
}
```

## `com.feilong.context.converter.IfStringToBeanConverter`

```java
public class com.feilong.context.converter.IfStringToBeanConverter<T> extends com.feilong.context.converter.AbstractStringToBeanConverter<T> {
  public com.feilong.context.converter.IfStringToBeanConverter();
  public com.feilong.context.converter.IfStringToBeanConverter(org.apache.commons.collections4.Predicate<java.lang.String>, com.feilong.context.converter.StringToBeanConverter<T>, com.feilong.context.converter.StringToBeanConverter<T>);
  public void setPredicate(org.apache.commons.collections4.Predicate<java.lang.String>);
  public void setTrueStringToBeanConverter(com.feilong.context.converter.StringToBeanConverter<T>);
  public void setFalseStringToBeanConverter(com.feilong.context.converter.StringToBeanConverter<T>);
}
```

## `com.feilong.context.converter.JsonStringToBeanConverter`

```java
public class com.feilong.context.converter.JsonStringToBeanConverter<T> extends com.feilong.context.converter.AbstractStringToBeanConverter<T> {
  public com.feilong.context.converter.JsonStringToBeanConverter();
  public com.feilong.context.converter.JsonStringToBeanConverter(java.lang.Class<T>);
  public com.feilong.context.converter.JsonStringToBeanConverter(com.feilong.json.JsonToJavaConfig);
  public void setJsonToJavaConfig(com.feilong.json.JsonToJavaConfig);
}
```

## `com.feilong.context.converter.JsonStringToListConverter`

```java
public class com.feilong.context.converter.JsonStringToListConverter<T> extends com.feilong.context.converter.AbstractStringToBeanConverter<java.util.List<T>> {
  public com.feilong.context.converter.JsonStringToListConverter();
  public com.feilong.context.converter.JsonStringToListConverter(java.lang.Class<T>);
  public com.feilong.context.converter.JsonStringToListConverter(com.feilong.json.JsonToJavaConfig);
  public void setJsonToJavaConfig(com.feilong.json.JsonToJavaConfig);
}
```

## `com.feilong.context.converter.MapBuilderStringToBeanConverter`

```java
public class com.feilong.context.converter.MapBuilderStringToBeanConverter<T> extends com.feilong.context.converter.AbstractBeanClassStringToBeanConverter<T> {
  public com.feilong.context.converter.MapBuilderStringToBeanConverter();
  public com.feilong.context.converter.MapBuilderStringToBeanConverter(com.feilong.context.converter.builder.NameAndValueMapBuilder, com.feilong.context.converter.builder.BeanBuilder);
  public com.feilong.context.converter.builder.NameAndValueMapBuilder getNameAndValueMapBuilder();
  public void setNameAndValueMapBuilder(com.feilong.context.converter.builder.NameAndValueMapBuilder);
  public com.feilong.context.converter.builder.BeanBuilder getBeanBuilder();
  public void setBeanBuilder(com.feilong.context.converter.builder.BeanBuilder);
}
```

## `com.feilong.context.converter.StringToBeanConverter`

```java
public interface com.feilong.context.converter.StringToBeanConverter<T> {
  public abstract T convert(java.lang.String);
}
```

## `com.feilong.context.converter.XMLMapBuilderStringToBeanConverter`

```java
public class com.feilong.context.converter.XMLMapBuilderStringToBeanConverter<T> extends com.feilong.context.converter.MapBuilderStringToBeanConverter<T> {
  public com.feilong.context.converter.XMLMapBuilderStringToBeanConverter();
  public com.feilong.context.converter.XMLMapBuilderStringToBeanConverter(java.lang.String);
  public com.feilong.context.converter.XMLMapBuilderStringToBeanConverter(java.lang.String, com.feilong.context.converter.builder.BeanBuilder);
  public com.feilong.context.converter.XMLMapBuilderStringToBeanConverter(com.feilong.context.converter.builder.NameAndValueMapBuilder, com.feilong.context.converter.builder.BeanBuilder);
}
```

## `com.feilong.context.converter.XStreamStringToBeanConverter`

```java
public class com.feilong.context.converter.XStreamStringToBeanConverter<T> extends com.feilong.context.converter.AbstractBeanClassStringToBeanConverter<T> {
  public com.feilong.context.converter.XStreamStringToBeanConverter();
}
```
