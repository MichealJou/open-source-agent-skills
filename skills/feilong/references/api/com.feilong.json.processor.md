# com.feilong.json.processor

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.json.processor.BigDecimalJsonValueProcessor`

```java
public class com.feilong.json.processor.BigDecimalJsonValueProcessor extends com.feilong.json.processor.AbstractJsonValueProcessor {
  public com.feilong.json.processor.BigDecimalJsonValueProcessor();
  public com.feilong.json.processor.BigDecimalJsonValueProcessor(java.lang.String);
  public java.lang.Object processObjectValue(java.lang.String, java.lang.Object, com.feilong.lib.json.JsonConfig);
  public java.lang.Object processArrayValue(java.lang.Object, com.feilong.lib.json.JsonConfig);
}
```

## `com.feilong.json.processor.CalendarJsonValueProcessor`

```java
public class com.feilong.json.processor.CalendarJsonValueProcessor extends com.feilong.json.processor.AbstractJsonValueProcessor {
  public com.feilong.json.processor.CalendarJsonValueProcessor(java.lang.String);
  public java.lang.Object processObjectValue(java.lang.String, java.lang.Object, com.feilong.lib.json.JsonConfig);
  public java.lang.Object processArrayValue(java.lang.Object, com.feilong.lib.json.JsonConfig);
}
```

## `com.feilong.json.processor.CapitalizePropertyNameProcessor`

```java
public class com.feilong.json.processor.CapitalizePropertyNameProcessor implements com.feilong.lib.json.processors.PropertyNameProcessor {
  public java.lang.String processPropertyName(java.lang.Class, java.lang.String);
}
```

## `com.feilong.json.processor.DateJsonValueProcessor`

```java
public class com.feilong.json.processor.DateJsonValueProcessor extends com.feilong.json.processor.AbstractJsonValueProcessor {
  public com.feilong.json.processor.DateJsonValueProcessor(java.lang.String);
  public java.lang.Object processObjectValue(java.lang.String, java.lang.Object, com.feilong.lib.json.JsonConfig);
  public java.lang.Object processArrayValue(java.lang.Object, com.feilong.lib.json.JsonConfig);
}
```

## `com.feilong.json.processor.SensitiveWordsJsonValueProcessor`

```java
public class com.feilong.json.processor.SensitiveWordsJsonValueProcessor extends com.feilong.json.processor.AbstractJsonValueProcessor {
  public com.feilong.json.processor.SensitiveWordsJsonValueProcessor();
  public java.lang.Object processObjectValue(java.lang.String, java.lang.Object, com.feilong.lib.json.JsonConfig);
  public java.lang.Object processArrayValue(java.lang.Object, com.feilong.lib.json.JsonConfig);
}
```

## `com.feilong.json.processor.SimpleMapPropertyNameProcessor`

```java
public class com.feilong.json.processor.SimpleMapPropertyNameProcessor implements com.feilong.lib.json.processors.PropertyNameProcessor {
  public com.feilong.json.processor.SimpleMapPropertyNameProcessor();
  public com.feilong.json.processor.SimpleMapPropertyNameProcessor(java.util.Map<java.lang.String, java.lang.String>);
  public java.lang.String processPropertyName(java.lang.Class, java.lang.String);
}
```

## `com.feilong.json.processor.StringOverLengthJsonValueProcessor`

```java
public class com.feilong.json.processor.StringOverLengthJsonValueProcessor extends com.feilong.json.processor.AbstractJsonValueProcessor {
  public com.feilong.json.processor.StringOverLengthJsonValueProcessor();
  public com.feilong.json.processor.StringOverLengthJsonValueProcessor(int);
  public com.feilong.json.processor.StringOverLengthJsonValueProcessor(int, java.lang.String);
  public static java.lang.Object format(java.lang.Object, int);
  public static java.lang.Object format(java.lang.Object, int, java.lang.String);
  public int getMaxLength();
  public void setMaxLength(int);
  public java.lang.String getOverLengthMaskString();
  public void setOverLengthMaskString(java.lang.String);
  public java.lang.Object processObjectValue(java.lang.String, java.lang.Object, com.feilong.lib.json.JsonConfig);
  public java.lang.Object processArrayValue(java.lang.Object, com.feilong.lib.json.JsonConfig);
}
```

## `com.feilong.json.processor.ToStringJsonValueProcessor`

```java
public class com.feilong.json.processor.ToStringJsonValueProcessor extends com.feilong.json.processor.AbstractJsonValueProcessor {
  public com.feilong.json.processor.ToStringJsonValueProcessor();
  public java.lang.Object processObjectValue(java.lang.String, java.lang.Object, com.feilong.lib.json.JsonConfig);
  public java.lang.Object processArrayValue(java.lang.Object, com.feilong.lib.json.JsonConfig);
}
```
