# cn.hutool.core.lang.mutable

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.lang.mutable.Mutable`

```java
public interface cn.hutool.core.lang.mutable.Mutable<T> {
  public abstract T get();
  public abstract void set(T);
}
```

## `cn.hutool.core.lang.mutable.MutableBool`

```java
public class cn.hutool.core.lang.mutable.MutableBool implements java.lang.Comparable<cn.hutool.core.lang.mutable.MutableBool>, cn.hutool.core.lang.mutable.Mutable<java.lang.Boolean>, java.io.Serializable {
  public cn.hutool.core.lang.mutable.MutableBool();
  public cn.hutool.core.lang.mutable.MutableBool(boolean);
  public cn.hutool.core.lang.mutable.MutableBool(java.lang.String) throws java.lang.NumberFormatException;
  public java.lang.Boolean get();
  public void set(boolean);
  public void set(java.lang.Boolean);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public int compareTo(cn.hutool.core.lang.mutable.MutableBool);
  public java.lang.String toString();
  public int compareTo(java.lang.Object);
  public void set(java.lang.Object);
  public java.lang.Object get();
}
```

## `cn.hutool.core.lang.mutable.MutableByte`

```java
public class cn.hutool.core.lang.mutable.MutableByte extends java.lang.Number implements java.lang.Comparable<cn.hutool.core.lang.mutable.MutableByte>, cn.hutool.core.lang.mutable.Mutable<java.lang.Number> {
  public cn.hutool.core.lang.mutable.MutableByte();
  public cn.hutool.core.lang.mutable.MutableByte(byte);
  public cn.hutool.core.lang.mutable.MutableByte(java.lang.Number);
  public cn.hutool.core.lang.mutable.MutableByte(java.lang.String) throws java.lang.NumberFormatException;
  public java.lang.Byte get();
  public void set(byte);
  public void set(java.lang.Number);
  public cn.hutool.core.lang.mutable.MutableByte increment();
  public cn.hutool.core.lang.mutable.MutableByte decrement();
  public cn.hutool.core.lang.mutable.MutableByte add(byte);
  public cn.hutool.core.lang.mutable.MutableByte add(java.lang.Number);
  public cn.hutool.core.lang.mutable.MutableByte subtract(byte);
  public cn.hutool.core.lang.mutable.MutableByte subtract(java.lang.Number);
  public byte byteValue();
  public int intValue();
  public long longValue();
  public float floatValue();
  public double doubleValue();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public int compareTo(cn.hutool.core.lang.mutable.MutableByte);
  public java.lang.String toString();
  public int compareTo(java.lang.Object);
  public void set(java.lang.Object);
  public java.lang.Object get();
}
```

## `cn.hutool.core.lang.mutable.MutableDouble`

```java
public class cn.hutool.core.lang.mutable.MutableDouble extends java.lang.Number implements java.lang.Comparable<cn.hutool.core.lang.mutable.MutableDouble>, cn.hutool.core.lang.mutable.Mutable<java.lang.Number> {
  public cn.hutool.core.lang.mutable.MutableDouble();
  public cn.hutool.core.lang.mutable.MutableDouble(double);
  public cn.hutool.core.lang.mutable.MutableDouble(java.lang.Number);
  public cn.hutool.core.lang.mutable.MutableDouble(java.lang.String) throws java.lang.NumberFormatException;
  public java.lang.Double get();
  public void set(double);
  public void set(java.lang.Number);
  public cn.hutool.core.lang.mutable.MutableDouble increment();
  public cn.hutool.core.lang.mutable.MutableDouble decrement();
  public cn.hutool.core.lang.mutable.MutableDouble add(double);
  public cn.hutool.core.lang.mutable.MutableDouble add(java.lang.Number);
  public cn.hutool.core.lang.mutable.MutableDouble subtract(double);
  public cn.hutool.core.lang.mutable.MutableDouble subtract(java.lang.Number);
  public int intValue();
  public long longValue();
  public float floatValue();
  public double doubleValue();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public int compareTo(cn.hutool.core.lang.mutable.MutableDouble);
  public java.lang.String toString();
  public int compareTo(java.lang.Object);
  public void set(java.lang.Object);
  public java.lang.Object get();
}
```

## `cn.hutool.core.lang.mutable.MutableFloat`

```java
public class cn.hutool.core.lang.mutable.MutableFloat extends java.lang.Number implements java.lang.Comparable<cn.hutool.core.lang.mutable.MutableFloat>, cn.hutool.core.lang.mutable.Mutable<java.lang.Number> {
  public cn.hutool.core.lang.mutable.MutableFloat();
  public cn.hutool.core.lang.mutable.MutableFloat(float);
  public cn.hutool.core.lang.mutable.MutableFloat(java.lang.Number);
  public cn.hutool.core.lang.mutable.MutableFloat(java.lang.String) throws java.lang.NumberFormatException;
  public java.lang.Float get();
  public void set(float);
  public void set(java.lang.Number);
  public cn.hutool.core.lang.mutable.MutableFloat increment();
  public cn.hutool.core.lang.mutable.MutableFloat decrement();
  public cn.hutool.core.lang.mutable.MutableFloat add(float);
  public cn.hutool.core.lang.mutable.MutableFloat add(java.lang.Number);
  public cn.hutool.core.lang.mutable.MutableFloat subtract(float);
  public cn.hutool.core.lang.mutable.MutableFloat subtract(java.lang.Number);
  public int intValue();
  public long longValue();
  public float floatValue();
  public double doubleValue();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public int compareTo(cn.hutool.core.lang.mutable.MutableFloat);
  public java.lang.String toString();
  public int compareTo(java.lang.Object);
  public void set(java.lang.Object);
  public java.lang.Object get();
}
```

## `cn.hutool.core.lang.mutable.MutableInt`

```java
public class cn.hutool.core.lang.mutable.MutableInt extends java.lang.Number implements java.lang.Comparable<cn.hutool.core.lang.mutable.MutableInt>, cn.hutool.core.lang.mutable.Mutable<java.lang.Number> {
  public cn.hutool.core.lang.mutable.MutableInt();
  public cn.hutool.core.lang.mutable.MutableInt(int);
  public cn.hutool.core.lang.mutable.MutableInt(java.lang.Number);
  public cn.hutool.core.lang.mutable.MutableInt(java.lang.String) throws java.lang.NumberFormatException;
  public java.lang.Integer get();
  public void set(int);
  public void set(java.lang.Number);
  public cn.hutool.core.lang.mutable.MutableInt increment();
  public cn.hutool.core.lang.mutable.MutableInt decrement();
  public cn.hutool.core.lang.mutable.MutableInt add(int);
  public cn.hutool.core.lang.mutable.MutableInt add(java.lang.Number);
  public cn.hutool.core.lang.mutable.MutableInt subtract(int);
  public cn.hutool.core.lang.mutable.MutableInt subtract(java.lang.Number);
  public int intValue();
  public long longValue();
  public float floatValue();
  public double doubleValue();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public int compareTo(cn.hutool.core.lang.mutable.MutableInt);
  public java.lang.String toString();
  public int compareTo(java.lang.Object);
  public void set(java.lang.Object);
  public java.lang.Object get();
}
```

## `cn.hutool.core.lang.mutable.MutableLong`

```java
public class cn.hutool.core.lang.mutable.MutableLong extends java.lang.Number implements java.lang.Comparable<cn.hutool.core.lang.mutable.MutableLong>, cn.hutool.core.lang.mutable.Mutable<java.lang.Number> {
  public cn.hutool.core.lang.mutable.MutableLong();
  public cn.hutool.core.lang.mutable.MutableLong(long);
  public cn.hutool.core.lang.mutable.MutableLong(java.lang.Number);
  public cn.hutool.core.lang.mutable.MutableLong(java.lang.String) throws java.lang.NumberFormatException;
  public java.lang.Long get();
  public void set(long);
  public void set(java.lang.Number);
  public cn.hutool.core.lang.mutable.MutableLong increment();
  public cn.hutool.core.lang.mutable.MutableLong decrement();
  public cn.hutool.core.lang.mutable.MutableLong add(long);
  public cn.hutool.core.lang.mutable.MutableLong add(java.lang.Number);
  public cn.hutool.core.lang.mutable.MutableLong subtract(long);
  public cn.hutool.core.lang.mutable.MutableLong subtract(java.lang.Number);
  public int intValue();
  public long longValue();
  public float floatValue();
  public double doubleValue();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public int compareTo(cn.hutool.core.lang.mutable.MutableLong);
  public java.lang.String toString();
  public int compareTo(java.lang.Object);
  public void set(java.lang.Object);
  public java.lang.Object get();
}
```

## `cn.hutool.core.lang.mutable.MutableObj`

```java
public class cn.hutool.core.lang.mutable.MutableObj<T> implements cn.hutool.core.lang.mutable.Mutable<T>, java.io.Serializable {
  public static <T> cn.hutool.core.lang.mutable.MutableObj<T> of(T);
  public cn.hutool.core.lang.mutable.MutableObj();
  public cn.hutool.core.lang.mutable.MutableObj(T);
  public T get();
  public void set(T);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `cn.hutool.core.lang.mutable.MutablePair`

```java
public class cn.hutool.core.lang.mutable.MutablePair<K, V> extends cn.hutool.core.lang.Pair<K, V> implements cn.hutool.core.lang.mutable.Mutable<cn.hutool.core.lang.Pair<K, V>> {
  public cn.hutool.core.lang.mutable.MutablePair(K, V);
  public cn.hutool.core.lang.mutable.MutablePair<K, V> setKey(K);
  public cn.hutool.core.lang.mutable.MutablePair<K, V> setValue(V);
  public cn.hutool.core.lang.Pair<K, V> get();
  public void set(cn.hutool.core.lang.Pair<K, V>);
  public void set(java.lang.Object);
  public java.lang.Object get();
}
```

## `cn.hutool.core.lang.mutable.MutableShort`

```java
public class cn.hutool.core.lang.mutable.MutableShort extends java.lang.Number implements java.lang.Comparable<cn.hutool.core.lang.mutable.MutableShort>, cn.hutool.core.lang.mutable.Mutable<java.lang.Number> {
  public cn.hutool.core.lang.mutable.MutableShort();
  public cn.hutool.core.lang.mutable.MutableShort(short);
  public cn.hutool.core.lang.mutable.MutableShort(java.lang.Number);
  public cn.hutool.core.lang.mutable.MutableShort(java.lang.String) throws java.lang.NumberFormatException;
  public java.lang.Short get();
  public void set(short);
  public void set(java.lang.Number);
  public cn.hutool.core.lang.mutable.MutableShort increment();
  public cn.hutool.core.lang.mutable.MutableShort decrement();
  public cn.hutool.core.lang.mutable.MutableShort add(short);
  public cn.hutool.core.lang.mutable.MutableShort add(java.lang.Number);
  public cn.hutool.core.lang.mutable.MutableShort subtract(short);
  public cn.hutool.core.lang.mutable.MutableShort subtract(java.lang.Number);
  public short shortValue();
  public int intValue();
  public long longValue();
  public float floatValue();
  public double doubleValue();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public int compareTo(cn.hutool.core.lang.mutable.MutableShort);
  public java.lang.String toString();
  public int compareTo(java.lang.Object);
  public void set(java.lang.Object);
  public java.lang.Object get();
}
```
