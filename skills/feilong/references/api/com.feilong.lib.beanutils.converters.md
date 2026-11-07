# com.feilong.lib.beanutils.converters

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.beanutils.converters.AbstractConverter`

```java
public abstract class com.feilong.lib.beanutils.converters.AbstractConverter implements com.feilong.lib.beanutils.Converter {
  public com.feilong.lib.beanutils.converters.AbstractConverter();
  public com.feilong.lib.beanutils.converters.AbstractConverter(java.lang.Object);
  public boolean isUseDefault();
  public <T> T convert(java.lang.Class<T>, java.lang.Object);
  public java.lang.String toString();
}
```

## `com.feilong.lib.beanutils.converters.ArrayConverter`

```java
public class com.feilong.lib.beanutils.converters.ArrayConverter extends com.feilong.lib.beanutils.converters.AbstractConverter {
  public com.feilong.lib.beanutils.converters.ArrayConverter(java.lang.Class<?>, com.feilong.lib.beanutils.Converter);
  public com.feilong.lib.beanutils.converters.ArrayConverter(java.lang.Class<?>, com.feilong.lib.beanutils.Converter, int);
  public void setDelimiter(char);
  public void setAllowedChars(char[]);
  public void setOnlyFirstToString(boolean);
  public java.lang.String toString();
}
```

## `com.feilong.lib.beanutils.converters.BigDecimalConverter`

```java
public final class com.feilong.lib.beanutils.converters.BigDecimalConverter extends com.feilong.lib.beanutils.converters.NumberConverter {
  public com.feilong.lib.beanutils.converters.BigDecimalConverter();
  public com.feilong.lib.beanutils.converters.BigDecimalConverter(java.lang.Object);
}
```

## `com.feilong.lib.beanutils.converters.BigIntegerConverter`

```java
public final class com.feilong.lib.beanutils.converters.BigIntegerConverter extends com.feilong.lib.beanutils.converters.NumberConverter {
  public com.feilong.lib.beanutils.converters.BigIntegerConverter();
  public com.feilong.lib.beanutils.converters.BigIntegerConverter(java.lang.Object);
}
```

## `com.feilong.lib.beanutils.converters.BooleanConverter`

```java
public final class com.feilong.lib.beanutils.converters.BooleanConverter extends com.feilong.lib.beanutils.converters.AbstractConverter {
  public com.feilong.lib.beanutils.converters.BooleanConverter();
  public com.feilong.lib.beanutils.converters.BooleanConverter(java.lang.Object);
  public com.feilong.lib.beanutils.converters.BooleanConverter(java.lang.String[], java.lang.String[]);
  public com.feilong.lib.beanutils.converters.BooleanConverter(java.lang.String[], java.lang.String[], java.lang.Object);
}
```

## `com.feilong.lib.beanutils.converters.ByteConverter`

```java
public final class com.feilong.lib.beanutils.converters.ByteConverter extends com.feilong.lib.beanutils.converters.NumberConverter {
  public com.feilong.lib.beanutils.converters.ByteConverter();
  public com.feilong.lib.beanutils.converters.ByteConverter(java.lang.Object);
}
```

## `com.feilong.lib.beanutils.converters.CalendarConverter`

```java
public final class com.feilong.lib.beanutils.converters.CalendarConverter extends com.feilong.lib.beanutils.converters.DateTimeConverter {
  public com.feilong.lib.beanutils.converters.CalendarConverter();
  public com.feilong.lib.beanutils.converters.CalendarConverter(java.lang.Object);
}
```

## `com.feilong.lib.beanutils.converters.CharacterConverter`

```java
public final class com.feilong.lib.beanutils.converters.CharacterConverter extends com.feilong.lib.beanutils.converters.AbstractConverter {
  public com.feilong.lib.beanutils.converters.CharacterConverter();
  public com.feilong.lib.beanutils.converters.CharacterConverter(java.lang.Object);
}
```

## `com.feilong.lib.beanutils.converters.ClassConverter`

```java
public final class com.feilong.lib.beanutils.converters.ClassConverter extends com.feilong.lib.beanutils.converters.AbstractConverter {
  public com.feilong.lib.beanutils.converters.ClassConverter();
  public com.feilong.lib.beanutils.converters.ClassConverter(java.lang.Object);
}
```

## `com.feilong.lib.beanutils.converters.ConverterFacade`

```java
public final class com.feilong.lib.beanutils.converters.ConverterFacade implements com.feilong.lib.beanutils.Converter {
  public com.feilong.lib.beanutils.converters.ConverterFacade(com.feilong.lib.beanutils.Converter);
  public <T> T convert(java.lang.Class<T>, java.lang.Object);
  public java.lang.String toString();
}
```

## `com.feilong.lib.beanutils.converters.DateConverter`

```java
public final class com.feilong.lib.beanutils.converters.DateConverter extends com.feilong.lib.beanutils.converters.DateTimeConverter {
  public com.feilong.lib.beanutils.converters.DateConverter();
  public com.feilong.lib.beanutils.converters.DateConverter(java.lang.Object);
}
```

## `com.feilong.lib.beanutils.converters.DateTimeConverter`

```java
public abstract class com.feilong.lib.beanutils.converters.DateTimeConverter extends com.feilong.lib.beanutils.converters.AbstractConverter {
  public com.feilong.lib.beanutils.converters.DateTimeConverter();
  public com.feilong.lib.beanutils.converters.DateTimeConverter(java.lang.Object);
  public void setUseLocaleFormat(boolean);
  public java.util.TimeZone getTimeZone();
  public void setTimeZone(java.util.TimeZone);
  public java.util.Locale getLocale();
  public void setLocale(java.util.Locale);
  public void setPattern(java.lang.String);
  public java.lang.String[] getPatterns();
  public void setPatterns(java.lang.String[]);
  public java.lang.String toString();
}
```

## `com.feilong.lib.beanutils.converters.DoubleConverter`

```java
public final class com.feilong.lib.beanutils.converters.DoubleConverter extends com.feilong.lib.beanutils.converters.NumberConverter {
  public com.feilong.lib.beanutils.converters.DoubleConverter();
  public com.feilong.lib.beanutils.converters.DoubleConverter(java.lang.Object);
}
```

## `com.feilong.lib.beanutils.converters.FileConverter`

```java
public final class com.feilong.lib.beanutils.converters.FileConverter extends com.feilong.lib.beanutils.converters.AbstractConverter {
  public com.feilong.lib.beanutils.converters.FileConverter();
  public com.feilong.lib.beanutils.converters.FileConverter(java.lang.Object);
}
```

## `com.feilong.lib.beanutils.converters.FloatConverter`

```java
public final class com.feilong.lib.beanutils.converters.FloatConverter extends com.feilong.lib.beanutils.converters.NumberConverter {
  public com.feilong.lib.beanutils.converters.FloatConverter();
  public com.feilong.lib.beanutils.converters.FloatConverter(java.lang.Object);
}
```

## `com.feilong.lib.beanutils.converters.IntegerConverter`

```java
public final class com.feilong.lib.beanutils.converters.IntegerConverter extends com.feilong.lib.beanutils.converters.NumberConverter {
  public com.feilong.lib.beanutils.converters.IntegerConverter();
  public com.feilong.lib.beanutils.converters.IntegerConverter(java.lang.Object);
}
```

## `com.feilong.lib.beanutils.converters.LongConverter`

```java
public final class com.feilong.lib.beanutils.converters.LongConverter extends com.feilong.lib.beanutils.converters.NumberConverter {
  public com.feilong.lib.beanutils.converters.LongConverter();
  public com.feilong.lib.beanutils.converters.LongConverter(java.lang.Object);
}
```

## `com.feilong.lib.beanutils.converters.NumberConverter`

```java
public abstract class com.feilong.lib.beanutils.converters.NumberConverter extends com.feilong.lib.beanutils.converters.AbstractConverter {
  public com.feilong.lib.beanutils.converters.NumberConverter(boolean);
  public com.feilong.lib.beanutils.converters.NumberConverter(boolean, java.lang.Object);
  public boolean isAllowDecimals();
  public void setUseLocaleFormat(boolean);
  public java.lang.String getPattern();
  public void setPattern(java.lang.String);
  public java.util.Locale getLocale();
  public void setLocale(java.util.Locale);
  public java.lang.String toString();
}
```

## `com.feilong.lib.beanutils.converters.ShortConverter`

```java
public final class com.feilong.lib.beanutils.converters.ShortConverter extends com.feilong.lib.beanutils.converters.NumberConverter {
  public com.feilong.lib.beanutils.converters.ShortConverter();
  public com.feilong.lib.beanutils.converters.ShortConverter(java.lang.Object);
}
```

## `com.feilong.lib.beanutils.converters.SqlDateConverter`

```java
public final class com.feilong.lib.beanutils.converters.SqlDateConverter extends com.feilong.lib.beanutils.converters.DateTimeConverter {
  public com.feilong.lib.beanutils.converters.SqlDateConverter();
  public com.feilong.lib.beanutils.converters.SqlDateConverter(java.lang.Object);
}
```

## `com.feilong.lib.beanutils.converters.SqlTimeConverter`

```java
public final class com.feilong.lib.beanutils.converters.SqlTimeConverter extends com.feilong.lib.beanutils.converters.DateTimeConverter {
  public com.feilong.lib.beanutils.converters.SqlTimeConverter();
  public com.feilong.lib.beanutils.converters.SqlTimeConverter(java.lang.Object);
}
```

## `com.feilong.lib.beanutils.converters.SqlTimestampConverter`

```java
public final class com.feilong.lib.beanutils.converters.SqlTimestampConverter extends com.feilong.lib.beanutils.converters.DateTimeConverter {
  public com.feilong.lib.beanutils.converters.SqlTimestampConverter();
  public com.feilong.lib.beanutils.converters.SqlTimestampConverter(java.lang.Object);
}
```

## `com.feilong.lib.beanutils.converters.StringConverter`

```java
public final class com.feilong.lib.beanutils.converters.StringConverter extends com.feilong.lib.beanutils.converters.AbstractConverter {
  public com.feilong.lib.beanutils.converters.StringConverter();
  public com.feilong.lib.beanutils.converters.StringConverter(java.lang.Object);
}
```

## `com.feilong.lib.beanutils.converters.URLConverter`

```java
public final class com.feilong.lib.beanutils.converters.URLConverter extends com.feilong.lib.beanutils.converters.AbstractConverter {
  public com.feilong.lib.beanutils.converters.URLConverter();
  public com.feilong.lib.beanutils.converters.URLConverter(java.lang.Object);
}
```
