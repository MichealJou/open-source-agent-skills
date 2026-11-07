# com.feilong.lib.ezmorph.object

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.ezmorph.object.AbstractObjectMorpher`

```java
public abstract class com.feilong.lib.ezmorph.object.AbstractObjectMorpher<T> implements com.feilong.lib.ezmorph.ObjectMorpher {
  public com.feilong.lib.ezmorph.object.AbstractObjectMorpher();
  public com.feilong.lib.ezmorph.object.AbstractObjectMorpher(boolean);
  public boolean isUseDefault();
  public T getDefaultValue();
  public boolean supports(java.lang.Class<?>);
}
```

## `com.feilong.lib.ezmorph.object.BigDecimalMorpher`

```java
public final class com.feilong.lib.ezmorph.object.BigDecimalMorpher extends com.feilong.lib.ezmorph.object.AbstractObjectMorpher<java.math.BigDecimal> {
  public com.feilong.lib.ezmorph.object.BigDecimalMorpher();
  public com.feilong.lib.ezmorph.object.BigDecimalMorpher(java.math.BigDecimal);
  public java.lang.Object morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
}
```

## `com.feilong.lib.ezmorph.object.BigIntegerMorpher`

```java
public final class com.feilong.lib.ezmorph.object.BigIntegerMorpher extends com.feilong.lib.ezmorph.object.AbstractObjectMorpher {
  public com.feilong.lib.ezmorph.object.BigIntegerMorpher();
  public com.feilong.lib.ezmorph.object.BigIntegerMorpher(java.math.BigInteger);
  public java.lang.Object morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
}
```

## `com.feilong.lib.ezmorph.object.BooleanObjectMorpher`

```java
public final class com.feilong.lib.ezmorph.object.BooleanObjectMorpher extends com.feilong.lib.ezmorph.object.AbstractObjectMorpher<java.lang.Boolean> {
  public com.feilong.lib.ezmorph.object.BooleanObjectMorpher();
  public com.feilong.lib.ezmorph.object.BooleanObjectMorpher(java.lang.Boolean);
  public java.lang.Object morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
}
```

## `com.feilong.lib.ezmorph.object.CharacterObjectMorpher`

```java
public final class com.feilong.lib.ezmorph.object.CharacterObjectMorpher extends com.feilong.lib.ezmorph.object.AbstractObjectMorpher<java.lang.Character> {
  public com.feilong.lib.ezmorph.object.CharacterObjectMorpher();
  public com.feilong.lib.ezmorph.object.CharacterObjectMorpher(java.lang.Character);
  public java.lang.Object morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
}
```

## `com.feilong.lib.ezmorph.object.ClassMorpher`

```java
public final class com.feilong.lib.ezmorph.object.ClassMorpher implements com.feilong.lib.ezmorph.ObjectMorpher {
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.Object morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
  public boolean supports(java.lang.Class<?>);
}
```

## `com.feilong.lib.ezmorph.object.DateMorpher`

```java
public final class com.feilong.lib.ezmorph.object.DateMorpher extends com.feilong.lib.ezmorph.object.AbstractObjectMorpher<java.util.Date> {
  public com.feilong.lib.ezmorph.object.DateMorpher(java.lang.String...);
  public com.feilong.lib.ezmorph.object.DateMorpher(java.lang.String[], java.util.Locale, boolean);
  public java.lang.Object morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
  public boolean supports(java.lang.Class<?>);
}
```

## `com.feilong.lib.ezmorph.object.EnumMorpher`

```java
public class com.feilong.lib.ezmorph.object.EnumMorpher implements com.feilong.lib.ezmorph.ObjectMorpher {
  public com.feilong.lib.ezmorph.object.EnumMorpher(java.lang.Class<?>);
  public java.lang.Object morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
  public boolean supports(java.lang.Class<?>);
}
```

## `com.feilong.lib.ezmorph.object.IdentityObjectMorpher`

```java
public final class com.feilong.lib.ezmorph.object.IdentityObjectMorpher implements com.feilong.lib.ezmorph.ObjectMorpher {
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.Object morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
  public boolean supports(java.lang.Class<?>);
}
```

## `com.feilong.lib.ezmorph.object.NumberMorpher`

```java
public final class com.feilong.lib.ezmorph.object.NumberMorpher extends com.feilong.lib.ezmorph.object.AbstractObjectMorpher<java.lang.Number> {
  public com.feilong.lib.ezmorph.object.NumberMorpher(java.lang.Class<?>);
  public com.feilong.lib.ezmorph.object.NumberMorpher(java.lang.Class<?>, java.lang.Number);
  public java.lang.Object morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
  public void setDefaultValue(java.lang.Number);
}
```

## `com.feilong.lib.ezmorph.object.StringMorpher`

```java
public final class com.feilong.lib.ezmorph.object.StringMorpher implements com.feilong.lib.ezmorph.ObjectMorpher {
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.Object morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
  public boolean supports(java.lang.Class<?>);
}
```
