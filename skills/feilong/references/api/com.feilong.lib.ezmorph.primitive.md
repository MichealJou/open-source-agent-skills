# com.feilong.lib.ezmorph.primitive

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.ezmorph.primitive.AbstractPrimitiveMorpher`

```java
public abstract class com.feilong.lib.ezmorph.primitive.AbstractPrimitiveMorpher<T> implements com.feilong.lib.ezmorph.Morpher {
  public com.feilong.lib.ezmorph.primitive.AbstractPrimitiveMorpher();
  public com.feilong.lib.ezmorph.primitive.AbstractPrimitiveMorpher(boolean);
  public boolean isUseDefault();
  public T getDefaultValue();
  public boolean supports(java.lang.Class<?>);
}
```

## `com.feilong.lib.ezmorph.primitive.BooleanMorpher`

```java
public final class com.feilong.lib.ezmorph.primitive.BooleanMorpher extends com.feilong.lib.ezmorph.primitive.AbstractPrimitiveMorpher<java.lang.Boolean> {
  public com.feilong.lib.ezmorph.primitive.BooleanMorpher();
  public com.feilong.lib.ezmorph.primitive.BooleanMorpher(boolean);
  public boolean morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
}
```

## `com.feilong.lib.ezmorph.primitive.ByteMorpher`

```java
public final class com.feilong.lib.ezmorph.primitive.ByteMorpher extends com.feilong.lib.ezmorph.primitive.AbstractPrimitiveMorpher<java.lang.Byte> {
  public com.feilong.lib.ezmorph.primitive.ByteMorpher();
  public com.feilong.lib.ezmorph.primitive.ByteMorpher(byte);
  public byte morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
}
```

## `com.feilong.lib.ezmorph.primitive.CharMorpher`

```java
public final class com.feilong.lib.ezmorph.primitive.CharMorpher extends com.feilong.lib.ezmorph.primitive.AbstractPrimitiveMorpher<java.lang.Character> {
  public com.feilong.lib.ezmorph.primitive.CharMorpher();
  public com.feilong.lib.ezmorph.primitive.CharMorpher(char);
  public char morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
}
```

## `com.feilong.lib.ezmorph.primitive.DoubleMorpher`

```java
public final class com.feilong.lib.ezmorph.primitive.DoubleMorpher extends com.feilong.lib.ezmorph.primitive.AbstractPrimitiveMorpher<java.lang.Double> {
  public com.feilong.lib.ezmorph.primitive.DoubleMorpher();
  public com.feilong.lib.ezmorph.primitive.DoubleMorpher(double);
  public double morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
}
```

## `com.feilong.lib.ezmorph.primitive.FloatMorpher`

```java
public final class com.feilong.lib.ezmorph.primitive.FloatMorpher extends com.feilong.lib.ezmorph.primitive.AbstractPrimitiveMorpher<java.lang.Float> {
  public com.feilong.lib.ezmorph.primitive.FloatMorpher();
  public com.feilong.lib.ezmorph.primitive.FloatMorpher(float);
  public float morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
}
```

## `com.feilong.lib.ezmorph.primitive.IntMorpher`

```java
public final class com.feilong.lib.ezmorph.primitive.IntMorpher extends com.feilong.lib.ezmorph.primitive.AbstractPrimitiveMorpher<java.lang.Integer> {
  public com.feilong.lib.ezmorph.primitive.IntMorpher();
  public com.feilong.lib.ezmorph.primitive.IntMorpher(int);
  public int morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
}
```

## `com.feilong.lib.ezmorph.primitive.LongMorpher`

```java
public final class com.feilong.lib.ezmorph.primitive.LongMorpher extends com.feilong.lib.ezmorph.primitive.AbstractPrimitiveMorpher<java.lang.Long> {
  public com.feilong.lib.ezmorph.primitive.LongMorpher();
  public com.feilong.lib.ezmorph.primitive.LongMorpher(long);
  public long morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
}
```

## `com.feilong.lib.ezmorph.primitive.ShortMorpher`

```java
public final class com.feilong.lib.ezmorph.primitive.ShortMorpher extends com.feilong.lib.ezmorph.primitive.AbstractPrimitiveMorpher<java.lang.Short> {
  public com.feilong.lib.ezmorph.primitive.ShortMorpher();
  public com.feilong.lib.ezmorph.primitive.ShortMorpher(short);
  public short morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
}
```
