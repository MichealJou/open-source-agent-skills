# com.feilong.formatter.entity

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.formatter.entity.BeanFormatterConfig`

```java
public class com.feilong.formatter.entity.BeanFormatterConfig {
  public com.feilong.formatter.entity.BeanFormatterConfig();
  public java.lang.String[] getExcludePropertyNames();
  public void setExcludePropertyNames(java.lang.String...);
  public java.lang.String[] getIncludePropertyNames();
  public void setIncludePropertyNames(java.lang.String...);
  public java.lang.String[] getSorts();
  public void setSorts(java.lang.String...);
  public java.util.Map<java.lang.String, org.apache.commons.collections4.Transformer<java.lang.Object, java.lang.String>> getPropertyNameAndTransformerMap();
  public void setPropertyNameAndTransformerMap(java.util.Map<java.lang.String, org.apache.commons.collections4.Transformer<java.lang.Object, java.lang.String>>);
}
```

## `com.feilong.formatter.entity.FormatterColumnEntity`

```java
public class com.feilong.formatter.entity.FormatterColumnEntity {
  public com.feilong.formatter.entity.FormatterColumnEntity(java.lang.String, java.lang.String, int);
  public java.lang.String getName();
  public void setName(java.lang.String);
  public int getOrder();
  public void setOrder(int);
  public java.lang.String getPropertyName();
  public void setPropertyName(java.lang.String);
  public java.lang.String toString();
}
```
