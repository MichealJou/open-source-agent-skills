# cn.hutool.core.getter

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.getter.ArrayTypeGetter`

```java
public interface cn.hutool.core.getter.ArrayTypeGetter {
  public abstract java.lang.String[] getObjs(java.lang.String);
  public abstract java.lang.String[] getStrs(java.lang.String);
  public abstract java.lang.Integer[] getInts(java.lang.String);
  public abstract java.lang.Short[] getShorts(java.lang.String);
  public abstract java.lang.Boolean[] getBools(java.lang.String);
  public abstract java.lang.Long[] getLongs(java.lang.String);
  public abstract java.lang.Character[] getChars(java.lang.String);
  public abstract java.lang.Double[] getDoubles(java.lang.String);
  public abstract java.lang.Byte[] getBytes(java.lang.String);
  public abstract java.math.BigInteger[] getBigIntegers(java.lang.String);
  public abstract java.math.BigDecimal[] getBigDecimals(java.lang.String);
}
```

## `cn.hutool.core.getter.BasicTypeGetter`

```java
public interface cn.hutool.core.getter.BasicTypeGetter<K> {
  public abstract java.lang.Object getObj(K);
  public abstract java.lang.String getStr(K);
  public abstract java.lang.Integer getInt(K);
  public abstract java.lang.Short getShort(K);
  public abstract java.lang.Boolean getBool(K);
  public abstract java.lang.Long getLong(K);
  public abstract java.lang.Character getChar(K);
  public abstract java.lang.Float getFloat(K);
  public abstract java.lang.Double getDouble(K);
  public abstract java.lang.Byte getByte(K);
  public abstract java.math.BigDecimal getBigDecimal(K);
  public abstract java.math.BigInteger getBigInteger(K);
  public abstract <E extends java.lang.Enum<E>> E getEnum(java.lang.Class<E>, K);
  public abstract java.util.Date getDate(K);
}
```

## `cn.hutool.core.getter.GroupedTypeGetter`

```java
public interface cn.hutool.core.getter.GroupedTypeGetter {
  public abstract java.lang.String getStrByGroup(java.lang.String, java.lang.String);
  public abstract java.lang.Integer getIntByGroup(java.lang.String, java.lang.String);
  public abstract java.lang.Short getShortByGroup(java.lang.String, java.lang.String);
  public abstract java.lang.Boolean getBoolByGroup(java.lang.String, java.lang.String);
  public abstract java.lang.Long getLongByGroup(java.lang.String, java.lang.String);
  public abstract java.lang.Character getCharByGroup(java.lang.String, java.lang.String);
  public abstract java.lang.Double getDoubleByGroup(java.lang.String, java.lang.String);
  public abstract java.lang.Byte getByteByGroup(java.lang.String, java.lang.String);
  public abstract java.math.BigDecimal getBigDecimalByGroup(java.lang.String, java.lang.String);
  public abstract java.math.BigInteger getBigIntegerByGroup(java.lang.String, java.lang.String);
}
```

## `cn.hutool.core.getter.ListTypeGetter`

```java
public interface cn.hutool.core.getter.ListTypeGetter {
  public abstract java.util.List<java.lang.Object> getObjList(java.lang.String);
  public abstract java.util.List<java.lang.String> getStrList(java.lang.String);
  public abstract java.util.List<java.lang.Integer> getIntList(java.lang.String);
  public abstract java.util.List<java.lang.Short> getShortList(java.lang.String);
  public abstract java.util.List<java.lang.Boolean> getBoolList(java.lang.String);
  public abstract java.util.List<java.lang.Long> getLongList(java.lang.String);
  public abstract java.util.List<java.lang.Character> getCharList(java.lang.String);
  public abstract java.util.List<java.lang.Double> getDoubleList(java.lang.String);
  public abstract java.util.List<java.lang.Byte> getByteList(java.lang.String);
  public abstract java.util.List<java.math.BigDecimal> getBigDecimalList(java.lang.String);
  public abstract java.util.List<java.math.BigInteger> getBigIntegerList(java.lang.String);
}
```

## `cn.hutool.core.getter.OptArrayTypeGetter`

```java
public interface cn.hutool.core.getter.OptArrayTypeGetter {
  public abstract java.lang.Object[] getObjs(java.lang.String, java.lang.Object[]);
  public abstract java.lang.String[] getStrs(java.lang.String, java.lang.String[]);
  public abstract java.lang.Integer[] getInts(java.lang.String, java.lang.Integer[]);
  public abstract java.lang.Short[] getShorts(java.lang.String, java.lang.Short[]);
  public abstract java.lang.Boolean[] getBools(java.lang.String, java.lang.Boolean[]);
  public abstract java.lang.Long[] getLongs(java.lang.String, java.lang.Long[]);
  public abstract java.lang.Character[] getChars(java.lang.String, java.lang.Character[]);
  public abstract java.lang.Double[] getDoubles(java.lang.String, java.lang.Double[]);
  public abstract java.lang.Byte[] getBytes(java.lang.String, java.lang.Byte[]);
  public abstract java.math.BigInteger[] getBigIntegers(java.lang.String, java.math.BigInteger[]);
  public abstract java.math.BigDecimal[] getBigDecimals(java.lang.String, java.math.BigDecimal[]);
}
```

## `cn.hutool.core.getter.OptBasicTypeGetter`

```java
public interface cn.hutool.core.getter.OptBasicTypeGetter<K> {
  public abstract java.lang.Object getObj(K, java.lang.Object);
  public abstract java.lang.String getStr(K, java.lang.String);
  public abstract java.lang.Integer getInt(K, java.lang.Integer);
  public abstract java.lang.Short getShort(K, java.lang.Short);
  public abstract java.lang.Boolean getBool(K, java.lang.Boolean);
  public abstract java.lang.Long getLong(K, java.lang.Long);
  public abstract java.lang.Character getChar(K, java.lang.Character);
  public abstract java.lang.Float getFloat(K, java.lang.Float);
  public abstract java.lang.Double getDouble(K, java.lang.Double);
  public abstract java.lang.Byte getByte(K, java.lang.Byte);
  public abstract java.math.BigDecimal getBigDecimal(K, java.math.BigDecimal);
  public abstract java.math.BigInteger getBigInteger(K, java.math.BigInteger);
  public abstract <E extends java.lang.Enum<E>> E getEnum(java.lang.Class<E>, K, E);
  public abstract java.util.Date getDate(K, java.util.Date);
}
```

## `cn.hutool.core.getter.OptNullBasicTypeFromObjectGetter`

```java
public interface cn.hutool.core.getter.OptNullBasicTypeFromObjectGetter<K> extends cn.hutool.core.getter.OptNullBasicTypeGetter<K> {
  public default java.lang.String getStr(K, java.lang.String);
  public default java.lang.Integer getInt(K, java.lang.Integer);
  public default java.lang.Short getShort(K, java.lang.Short);
  public default java.lang.Boolean getBool(K, java.lang.Boolean);
  public default java.lang.Long getLong(K, java.lang.Long);
  public default java.lang.Character getChar(K, java.lang.Character);
  public default java.lang.Float getFloat(K, java.lang.Float);
  public default java.lang.Double getDouble(K, java.lang.Double);
  public default java.lang.Byte getByte(K, java.lang.Byte);
  public default java.math.BigDecimal getBigDecimal(K, java.math.BigDecimal);
  public default java.math.BigInteger getBigInteger(K, java.math.BigInteger);
  public default <E extends java.lang.Enum<E>> E getEnum(java.lang.Class<E>, K, E);
  public default java.util.Date getDate(K, java.util.Date);
}
```

## `cn.hutool.core.getter.OptNullBasicTypeFromStringGetter`

```java
public interface cn.hutool.core.getter.OptNullBasicTypeFromStringGetter<K> extends cn.hutool.core.getter.OptNullBasicTypeGetter<K> {
  public default java.lang.Object getObj(K, java.lang.Object);
  public default java.lang.Integer getInt(K, java.lang.Integer);
  public default java.lang.Short getShort(K, java.lang.Short);
  public default java.lang.Boolean getBool(K, java.lang.Boolean);
  public default java.lang.Long getLong(K, java.lang.Long);
  public default java.lang.Character getChar(K, java.lang.Character);
  public default java.lang.Float getFloat(K, java.lang.Float);
  public default java.lang.Double getDouble(K, java.lang.Double);
  public default java.lang.Byte getByte(K, java.lang.Byte);
  public default java.math.BigDecimal getBigDecimal(K, java.math.BigDecimal);
  public default java.math.BigInteger getBigInteger(K, java.math.BigInteger);
  public default <E extends java.lang.Enum<E>> E getEnum(java.lang.Class<E>, K, E);
  public default java.util.Date getDate(K, java.util.Date);
}
```

## `cn.hutool.core.getter.OptNullBasicTypeGetter`

```java
public interface cn.hutool.core.getter.OptNullBasicTypeGetter<K> extends cn.hutool.core.getter.BasicTypeGetter<K>, cn.hutool.core.getter.OptBasicTypeGetter<K> {
  public default java.lang.Object getObj(K);
  public default java.lang.String getStr(K);
  public default java.lang.Integer getInt(K);
  public default java.lang.Short getShort(K);
  public default java.lang.Boolean getBool(K);
  public default java.lang.Long getLong(K);
  public default java.lang.Character getChar(K);
  public default java.lang.Float getFloat(K);
  public default java.lang.Double getDouble(K);
  public default java.lang.Byte getByte(K);
  public default java.math.BigDecimal getBigDecimal(K);
  public default java.math.BigInteger getBigInteger(K);
  public default <E extends java.lang.Enum<E>> E getEnum(java.lang.Class<E>, K);
  public default java.util.Date getDate(K);
}
```
