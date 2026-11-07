# com.feilong.lib.excel.convertor

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.excel.convertor.AbstractChoiceConvertor`

```java
public abstract class com.feilong.lib.excel.convertor.AbstractChoiceConvertor<T> extends com.feilong.lib.excel.convertor.AbstractDataConvertor<T> {
  public com.feilong.lib.excel.convertor.AbstractChoiceConvertor();
}
```

## `com.feilong.lib.excel.convertor.AbstractDataConvertor`

```java
public abstract class com.feilong.lib.excel.convertor.AbstractDataConvertor<T> implements com.feilong.lib.excel.convertor.DataConvertor<T> {
  public com.feilong.lib.excel.convertor.AbstractDataConvertor();
  public T convert(java.lang.Object, int, java.lang.String, com.feilong.excel.definition.ExcelCell);
}
```

## `com.feilong.lib.excel.convertor.BigDecimalConvertor`

```java
public class com.feilong.lib.excel.convertor.BigDecimalConvertor extends com.feilong.lib.excel.convertor.AbstractDataConvertor<java.math.BigDecimal> {
  public com.feilong.lib.excel.convertor.BigDecimalConvertor();
  public java.lang.String getDataTypeAbbr();
  public java.lang.Class<java.math.BigDecimal> supportClass();
}
```

## `com.feilong.lib.excel.convertor.BooleanConvertor`

```java
public class com.feilong.lib.excel.convertor.BooleanConvertor extends com.feilong.lib.excel.convertor.AbstractDataConvertor<java.lang.Boolean> {
  public com.feilong.lib.excel.convertor.BooleanConvertor();
  public java.lang.String getDataTypeAbbr();
  public java.lang.Class<java.lang.Boolean> supportClass();
}
```

## `com.feilong.lib.excel.convertor.DataConvertor`

```java
public interface com.feilong.lib.excel.convertor.DataConvertor<T> {
  public abstract java.lang.Class<T> supportClass();
  public abstract java.lang.String getDataTypeAbbr();
  public abstract T convert(java.lang.Object, int, java.lang.String, com.feilong.excel.definition.ExcelCell);
}
```

## `com.feilong.lib.excel.convertor.DateConvertor`

```java
public class com.feilong.lib.excel.convertor.DateConvertor extends com.feilong.lib.excel.convertor.AbstractDataConvertor<java.util.Date> {
  public com.feilong.lib.excel.convertor.DateConvertor();
  public java.lang.String getDatePattern();
  public void setDatePattern(java.lang.String);
  public java.lang.String getDataTypeAbbr();
  public java.lang.Class<java.util.Date> supportClass();
}
```

## `com.feilong.lib.excel.convertor.DoubleConvertor`

```java
public class com.feilong.lib.excel.convertor.DoubleConvertor extends com.feilong.lib.excel.convertor.AbstractDataConvertor<java.lang.Double> {
  public com.feilong.lib.excel.convertor.DoubleConvertor();
  public java.lang.String getDataTypeAbbr();
  public java.lang.Class<java.lang.Double> supportClass();
}
```

## `com.feilong.lib.excel.convertor.IntegerConvertor`

```java
public class com.feilong.lib.excel.convertor.IntegerConvertor extends com.feilong.lib.excel.convertor.AbstractChoiceConvertor<java.lang.Integer> {
  public com.feilong.lib.excel.convertor.IntegerConvertor();
  public java.lang.String getDataTypeAbbr();
  public java.lang.Class<java.lang.Integer> supportClass();
}
```

## `com.feilong.lib.excel.convertor.LongConvertor`

```java
public class com.feilong.lib.excel.convertor.LongConvertor extends com.feilong.lib.excel.convertor.AbstractChoiceConvertor<java.lang.Long> {
  public com.feilong.lib.excel.convertor.LongConvertor();
  public java.lang.String getDataTypeAbbr();
  public java.lang.Class<java.lang.Long> supportClass();
}
```

## `com.feilong.lib.excel.convertor.StringConvertor`

```java
public class com.feilong.lib.excel.convertor.StringConvertor extends com.feilong.lib.excel.convertor.AbstractChoiceConvertor<java.lang.String> {
  public com.feilong.lib.excel.convertor.StringConvertor();
  public java.lang.String getDataTypeAbbr();
  public java.lang.Class<java.lang.String> supportClass();
}
```
