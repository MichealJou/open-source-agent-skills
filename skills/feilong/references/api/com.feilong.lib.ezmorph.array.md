# com.feilong.lib.ezmorph.array

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.ezmorph.array.AbstractArrayMorpher`

```java
public abstract class com.feilong.lib.ezmorph.array.AbstractArrayMorpher implements com.feilong.lib.ezmorph.ObjectMorpher {
  public com.feilong.lib.ezmorph.array.AbstractArrayMorpher();
  public com.feilong.lib.ezmorph.array.AbstractArrayMorpher(boolean);
  public boolean isUseDefault();
  public void setUseDefault(boolean);
  public boolean supports(java.lang.Class<?>);
}
```

## `com.feilong.lib.ezmorph.array.BooleanArrayMorpher`

```java
public final class com.feilong.lib.ezmorph.array.BooleanArrayMorpher extends com.feilong.lib.ezmorph.array.AbstractArrayMorpher {
  public com.feilong.lib.ezmorph.array.BooleanArrayMorpher();
  public com.feilong.lib.ezmorph.array.BooleanArrayMorpher(boolean);
  public boolean getDefaultValue();
  public java.lang.Object morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
}
```

## `com.feilong.lib.ezmorph.array.BooleanObjectArrayMorpher`

```java
public final class com.feilong.lib.ezmorph.array.BooleanObjectArrayMorpher extends com.feilong.lib.ezmorph.array.AbstractArrayMorpher {
  public com.feilong.lib.ezmorph.array.BooleanObjectArrayMorpher();
  public com.feilong.lib.ezmorph.array.BooleanObjectArrayMorpher(java.lang.Boolean);
  public java.lang.Boolean getDefaultValue();
  public java.lang.Object morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
}
```

## `com.feilong.lib.ezmorph.array.ByteArrayMorpher`

```java
public final class com.feilong.lib.ezmorph.array.ByteArrayMorpher extends com.feilong.lib.ezmorph.array.AbstractArrayMorpher {
  public com.feilong.lib.ezmorph.array.ByteArrayMorpher();
  public com.feilong.lib.ezmorph.array.ByteArrayMorpher(byte);
  public byte getDefaultValue();
  public java.lang.Object morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
}
```

## `com.feilong.lib.ezmorph.array.CharArrayMorpher`

```java
public final class com.feilong.lib.ezmorph.array.CharArrayMorpher extends com.feilong.lib.ezmorph.array.AbstractArrayMorpher {
  public com.feilong.lib.ezmorph.array.CharArrayMorpher();
  public com.feilong.lib.ezmorph.array.CharArrayMorpher(char);
  public char getDefaultValue();
  public java.lang.Object morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
}
```

## `com.feilong.lib.ezmorph.array.CharacterObjectArrayMorpher`

```java
public final class com.feilong.lib.ezmorph.array.CharacterObjectArrayMorpher extends com.feilong.lib.ezmorph.array.AbstractArrayMorpher {
  public com.feilong.lib.ezmorph.array.CharacterObjectArrayMorpher();
  public com.feilong.lib.ezmorph.array.CharacterObjectArrayMorpher(java.lang.Character);
  public java.lang.Character getDefaultValue();
  public java.lang.Object morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
}
```

## `com.feilong.lib.ezmorph.array.DoubleArrayMorpher`

```java
public final class com.feilong.lib.ezmorph.array.DoubleArrayMorpher extends com.feilong.lib.ezmorph.array.AbstractArrayMorpher {
  public com.feilong.lib.ezmorph.array.DoubleArrayMorpher();
  public com.feilong.lib.ezmorph.array.DoubleArrayMorpher(double);
  public double getDefaultValue();
  public java.lang.Object morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
}
```

## `com.feilong.lib.ezmorph.array.FloatArrayMorpher`

```java
public final class com.feilong.lib.ezmorph.array.FloatArrayMorpher extends com.feilong.lib.ezmorph.array.AbstractArrayMorpher {
  public com.feilong.lib.ezmorph.array.FloatArrayMorpher();
  public com.feilong.lib.ezmorph.array.FloatArrayMorpher(float);
  public float getDefaultValue();
  public java.lang.Object morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
}
```

## `com.feilong.lib.ezmorph.array.IntArrayMorpher`

```java
public final class com.feilong.lib.ezmorph.array.IntArrayMorpher extends com.feilong.lib.ezmorph.array.AbstractArrayMorpher {
  public com.feilong.lib.ezmorph.array.IntArrayMorpher();
  public com.feilong.lib.ezmorph.array.IntArrayMorpher(int);
  public int getDefaultValue();
  public java.lang.Object morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
}
```

## `com.feilong.lib.ezmorph.array.LongArrayMorpher`

```java
public final class com.feilong.lib.ezmorph.array.LongArrayMorpher extends com.feilong.lib.ezmorph.array.AbstractArrayMorpher {
  public com.feilong.lib.ezmorph.array.LongArrayMorpher();
  public com.feilong.lib.ezmorph.array.LongArrayMorpher(long);
  public long getDefaultValue();
  public java.lang.Object morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
}
```

## `com.feilong.lib.ezmorph.array.ObjectArrayMorpher`

```java
public final class com.feilong.lib.ezmorph.array.ObjectArrayMorpher extends com.feilong.lib.ezmorph.array.AbstractArrayMorpher {
  public com.feilong.lib.ezmorph.array.ObjectArrayMorpher(com.feilong.lib.ezmorph.Morpher);
  public java.lang.Object morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
  public boolean supports(java.lang.Class<?>);
}
```

## `com.feilong.lib.ezmorph.array.ShortArrayMorpher`

```java
public final class com.feilong.lib.ezmorph.array.ShortArrayMorpher extends com.feilong.lib.ezmorph.array.AbstractArrayMorpher {
  public com.feilong.lib.ezmorph.array.ShortArrayMorpher();
  public com.feilong.lib.ezmorph.array.ShortArrayMorpher(short);
  public short getDefaultValue();
  public java.lang.Object morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
}
```
