# com.feilong.core.util.transformer

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.core.util.transformer.BeanTransformer`

```java
public class com.feilong.core.util.transformer.BeanTransformer<I, O> implements org.apache.commons.collections4.Transformer<I, O>, java.io.Serializable {
  public com.feilong.core.util.transformer.BeanTransformer(java.lang.Class<O>, java.lang.String...);
  public O transform(I);
}
```

## `com.feilong.core.util.transformer.DateToStringTransformer`

```java
public class com.feilong.core.util.transformer.DateToStringTransformer implements org.apache.commons.collections4.Transformer<java.util.Date, java.lang.String>, java.io.Serializable {
  public com.feilong.core.util.transformer.DateToStringTransformer(java.lang.String);
  public java.lang.String transform(java.util.Date);
  public java.lang.Object transform(java.lang.Object);
}
```

## `com.feilong.core.util.transformer.NumberToStringTransformer`

```java
public class com.feilong.core.util.transformer.NumberToStringTransformer implements org.apache.commons.collections4.Transformer<java.lang.Number, java.lang.String>, java.io.Serializable {
  public com.feilong.core.util.transformer.NumberToStringTransformer(java.lang.String);
  public java.lang.String transform(java.lang.Number);
  public java.lang.Object transform(java.lang.Object);
}
```

## `com.feilong.core.util.transformer.SimpleClassTransformer`

```java
public class com.feilong.core.util.transformer.SimpleClassTransformer<T, V> implements org.apache.commons.collections4.Transformer<T, V>, java.io.Serializable {
  public com.feilong.core.util.transformer.SimpleClassTransformer(java.lang.Class<V>);
  public V transform(T);
}
```

## `com.feilong.core.util.transformer.StringToDateTransformer`

```java
public class com.feilong.core.util.transformer.StringToDateTransformer implements org.apache.commons.collections4.Transformer<java.lang.String, java.util.Date>, java.io.Serializable {
  public com.feilong.core.util.transformer.StringToDateTransformer(java.lang.String);
  public java.util.Date transform(java.lang.String);
  public java.lang.Object transform(java.lang.Object);
}
```
