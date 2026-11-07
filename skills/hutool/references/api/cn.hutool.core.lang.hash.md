# cn.hutool.core.lang.hash

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.lang.hash.CityHash`

```java
public class cn.hutool.core.lang.hash.CityHash {
  public cn.hutool.core.lang.hash.CityHash();
  public static int hash32(byte[]);
  public static long hash64(byte[]);
  public static long hash64(byte[], long, long);
  public static long hash64(byte[], long);
  public static cn.hutool.core.lang.hash.Number128 hash128(byte[]);
  public static cn.hutool.core.lang.hash.Number128 hash128(byte[], cn.hutool.core.lang.hash.Number128);
}
```

## `cn.hutool.core.lang.hash.Hash`

```java
public interface cn.hutool.core.lang.hash.Hash<T> {
  public abstract java.lang.Number hash(T);
}
```

## `cn.hutool.core.lang.hash.Hash128`

```java
public interface cn.hutool.core.lang.hash.Hash128<T> extends cn.hutool.core.lang.hash.Hash<T> {
  public abstract cn.hutool.core.lang.hash.Number128 hash128(T);
  public default java.lang.Number hash(T);
}
```

## `cn.hutool.core.lang.hash.Hash32`

```java
public interface cn.hutool.core.lang.hash.Hash32<T> extends cn.hutool.core.lang.hash.Hash<T> {
  public abstract int hash32(T);
  public default java.lang.Number hash(T);
}
```

## `cn.hutool.core.lang.hash.Hash64`

```java
public interface cn.hutool.core.lang.hash.Hash64<T> extends cn.hutool.core.lang.hash.Hash<T> {
  public abstract long hash64(T);
  public default java.lang.Number hash(T);
}
```

## `cn.hutool.core.lang.hash.KetamaHash`

```java
public class cn.hutool.core.lang.hash.KetamaHash implements cn.hutool.core.lang.hash.Hash64<java.lang.String>, cn.hutool.core.lang.hash.Hash32<java.lang.String> {
  public cn.hutool.core.lang.hash.KetamaHash();
  public long hash64(java.lang.String);
  public int hash32(java.lang.String);
  public java.lang.Number hash(java.lang.String);
  public java.lang.Number hash(java.lang.Object);
  public long hash64(java.lang.Object);
  public int hash32(java.lang.Object);
}
```

## `cn.hutool.core.lang.hash.MetroHash`

```java
public class cn.hutool.core.lang.hash.MetroHash {
  public cn.hutool.core.lang.hash.MetroHash();
  public static long hash64(byte[]);
  public static cn.hutool.core.lang.hash.Number128 hash128(byte[]);
  public static long hash64(byte[], long);
  public static cn.hutool.core.lang.hash.Number128 hash128(byte[], long);
}
```

## `cn.hutool.core.lang.hash.MurmurHash`

```java
public class cn.hutool.core.lang.hash.MurmurHash implements java.io.Serializable {
  public cn.hutool.core.lang.hash.MurmurHash();
  public static int hash32(java.lang.CharSequence);
  public static int hash32(byte[]);
  public static int hash32(byte[], int, int);
  public static int hash32(byte[], int, int, int);
  public static long hash64(java.lang.CharSequence);
  public static long hash64(byte[]);
  public static long hash64(byte[], int, int);
  public static long[] hash128(java.lang.CharSequence);
  public static long[] hash128(byte[]);
  public static long[] hash128(byte[], int, int);
  public static long[] hash128(byte[], int, int, int);
}
```

## `cn.hutool.core.lang.hash.Number128`

```java
public class cn.hutool.core.lang.hash.Number128 extends java.lang.Number {
  public cn.hutool.core.lang.hash.Number128(long, long);
  public long getLowValue();
  public void setLowValue(long);
  public long getHighValue();
  public void setHighValue(long);
  public long[] getLongArray();
  public int intValue();
  public long longValue();
  public float floatValue();
  public double doubleValue();
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```
