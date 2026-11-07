# cn.hutool.core.convert

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.convert.AbstractConverter`

```java
public abstract class cn.hutool.core.convert.AbstractConverter<T> implements cn.hutool.core.convert.Converter<T>, java.io.Serializable {
  public cn.hutool.core.convert.AbstractConverter();
  public T convertQuietly(java.lang.Object, T);
  public T convert(java.lang.Object, T);
  public java.lang.Class<T> getTargetType();
}
```

## `cn.hutool.core.convert.BasicType`

```java
public final class cn.hutool.core.convert.BasicType extends java.lang.Enum<cn.hutool.core.convert.BasicType> {
  public static cn.hutool.core.convert.BasicType[] values();
  public static cn.hutool.core.convert.BasicType valueOf(java.lang.String);
  public static java.lang.Class<?> wrap(java.lang.Class<?>);
  public static java.lang.Class<?> unWrap(java.lang.Class<?>);
}
```

## `cn.hutool.core.convert.CastUtil`

```java
public class cn.hutool.core.convert.CastUtil {
  public cn.hutool.core.convert.CastUtil();
  public static <T> java.util.Collection<T> castUp(java.util.Collection<? extends T>);
  public static <T> java.util.Collection<T> castDown(java.util.Collection<? super T>);
  public static <T> java.util.Set<T> castUp(java.util.Set<? extends T>);
  public static <T> java.util.Set<T> castDown(java.util.Set<? super T>);
  public static <T> java.util.List<T> castUp(java.util.List<? extends T>);
  public static <T> java.util.List<T> castDown(java.util.List<? super T>);
  public static <K, V> java.util.Map<K, V> castUp(java.util.Map<? extends K, ? extends V>);
  public static <K, V> java.util.Map<K, V> castDown(java.util.Map<? super K, ? super V>);
}
```

## `cn.hutool.core.convert.Convert`

```java
public class cn.hutool.core.convert.Convert {
  public cn.hutool.core.convert.Convert();
  public static java.lang.String toStr(java.lang.Object, java.lang.String);
  public static java.lang.String toStr(java.lang.Object);
  public static java.lang.String[] toStrArray(java.lang.Object);
  public static java.lang.Character toChar(java.lang.Object, java.lang.Character);
  public static java.lang.Character toChar(java.lang.Object);
  public static java.lang.Character[] toCharArray(java.lang.Object);
  public static java.lang.Byte toByte(java.lang.Object, java.lang.Byte);
  public static java.lang.Byte toByte(java.lang.Object);
  public static java.lang.Byte[] toByteArray(java.lang.Object);
  public static byte[] toPrimitiveByteArray(java.lang.Object);
  public static java.lang.Short toShort(java.lang.Object, java.lang.Short);
  public static java.lang.Short toShort(java.lang.Object);
  public static java.lang.Short[] toShortArray(java.lang.Object);
  public static java.lang.Number toNumber(java.lang.Object, java.lang.Number);
  public static java.lang.Number toNumber(java.lang.Object);
  public static java.lang.Number[] toNumberArray(java.lang.Object);
  public static java.lang.Integer toInt(java.lang.Object, java.lang.Integer);
  public static java.lang.Integer toInt(java.lang.Object);
  public static java.lang.Integer[] toIntArray(java.lang.Object);
  public static java.lang.Long toLong(java.lang.Object, java.lang.Long);
  public static java.lang.Long toLong(java.lang.Object);
  public static java.lang.Long[] toLongArray(java.lang.Object);
  public static java.lang.Double toDouble(java.lang.Object, java.lang.Double);
  public static java.lang.Double toDouble(java.lang.Object);
  public static java.lang.Double[] toDoubleArray(java.lang.Object);
  public static java.lang.Float toFloat(java.lang.Object, java.lang.Float);
  public static java.lang.Float toFloat(java.lang.Object);
  public static java.lang.Float[] toFloatArray(java.lang.Object);
  public static java.lang.Boolean toBool(java.lang.Object, java.lang.Boolean);
  public static java.lang.Boolean toBool(java.lang.Object);
  public static java.lang.Boolean[] toBooleanArray(java.lang.Object);
  public static java.math.BigInteger toBigInteger(java.lang.Object, java.math.BigInteger);
  public static java.math.BigInteger toBigInteger(java.lang.Object);
  public static java.math.BigDecimal toBigDecimal(java.lang.Object, java.math.BigDecimal);
  public static java.math.BigDecimal toBigDecimal(java.lang.Object);
  public static java.util.Date toDate(java.lang.Object, java.util.Date);
  public static java.time.LocalDateTime toLocalDateTime(java.lang.Object, java.time.LocalDateTime);
  public static java.time.LocalDateTime toLocalDateTime(java.lang.Object);
  public static java.util.Date toInstant(java.lang.Object, java.util.Date);
  public static java.util.Date toDate(java.lang.Object);
  public static <E extends java.lang.Enum<E>> E toEnum(java.lang.Class<E>, java.lang.Object, E);
  public static <E extends java.lang.Enum<E>> E toEnum(java.lang.Class<E>, java.lang.Object);
  public static java.util.Collection<?> toCollection(java.lang.Class<?>, java.lang.Class<?>, java.lang.Object);
  public static java.util.List<?> toList(java.lang.Object);
  public static <T> java.util.List<T> toList(java.lang.Class<T>, java.lang.Object);
  public static <T> java.util.Set<T> toSet(java.lang.Class<T>, java.lang.Object);
  public static <K, V> java.util.Map<K, V> toMap(java.lang.Class<K>, java.lang.Class<V>, java.lang.Object);
  public static <K, V> java.util.Map<K, V> toMap(java.lang.Class<? extends java.util.Map>, java.lang.Class<K>, java.lang.Class<V>, java.lang.Object);
  public static <T> T convertByClassName(java.lang.String, java.lang.Object) throws cn.hutool.core.convert.ConvertException;
  public static <T> T convert(java.lang.Class<T>, java.lang.Object) throws cn.hutool.core.convert.ConvertException;
  public static <T> T convert(cn.hutool.core.lang.TypeReference<T>, java.lang.Object) throws cn.hutool.core.convert.ConvertException;
  public static <T> T convert(java.lang.reflect.Type, java.lang.Object) throws cn.hutool.core.convert.ConvertException;
  public static <T> T convert(java.lang.Class<T>, java.lang.Object, T) throws cn.hutool.core.convert.ConvertException;
  public static <T> T convert(java.lang.reflect.Type, java.lang.Object, T) throws cn.hutool.core.convert.ConvertException;
  public static <T> T convertQuietly(java.lang.reflect.Type, java.lang.Object);
  public static <T> T convertQuietly(java.lang.reflect.Type, java.lang.Object, T);
  public static <T> T convertWithCheck(java.lang.reflect.Type, java.lang.Object, T, boolean);
  public static java.lang.String toSBC(java.lang.String);
  public static java.lang.String toSBC(java.lang.String, java.util.Set<java.lang.Character>);
  public static java.lang.String toDBC(java.lang.String);
  public static java.lang.String toDBC(java.lang.String, java.util.Set<java.lang.Character>);
  public static java.lang.String toHex(java.lang.String, java.nio.charset.Charset);
  public static java.lang.String toHex(byte[]);
  public static byte[] hexToBytes(java.lang.String);
  public static java.lang.String hexToStr(java.lang.String, java.nio.charset.Charset);
  public static java.lang.String strToUnicode(java.lang.String);
  public static java.lang.String unicodeToStr(java.lang.String);
  public static java.lang.String convertCharset(java.lang.String, java.lang.String, java.lang.String);
  public static long convertTime(long, java.util.concurrent.TimeUnit, java.util.concurrent.TimeUnit);
  public static java.lang.Class<?> wrap(java.lang.Class<?>);
  public static java.lang.Class<?> unWrap(java.lang.Class<?>);
  public static java.lang.String numberToWord(java.lang.Number);
  public static java.lang.String numberToSimple(java.lang.Number);
  public static java.lang.String numberToChinese(double, boolean);
  public static int chineseToNumber(java.lang.String);
  public static java.lang.String digitToChinese(java.lang.Number);
  public static java.math.BigDecimal chineseMoneyToNumber(java.lang.String);
  public static byte intToByte(int);
  public static int byteToUnsignedInt(byte);
  public static short bytesToShort(byte[]);
  public static byte[] shortToBytes(short);
  public static int bytesToInt(byte[]);
  public static byte[] intToBytes(int);
  public static byte[] longToBytes(long);
  public static long bytesToLong(byte[]);
}
```

## `cn.hutool.core.convert.ConvertException`

```java
public class cn.hutool.core.convert.ConvertException extends java.lang.RuntimeException {
  public cn.hutool.core.convert.ConvertException(java.lang.Throwable);
  public cn.hutool.core.convert.ConvertException(java.lang.String);
  public cn.hutool.core.convert.ConvertException(java.lang.String, java.lang.Object...);
  public cn.hutool.core.convert.ConvertException(java.lang.String, java.lang.Throwable);
  public cn.hutool.core.convert.ConvertException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.core.convert.Converter`

```java
public interface cn.hutool.core.convert.Converter<T> {
  public abstract T convert(java.lang.Object, T) throws java.lang.IllegalArgumentException;
  public default T convertWithCheck(java.lang.Object, T, boolean);
}
```

## `cn.hutool.core.convert.ConverterRegistry`

```java
public class cn.hutool.core.convert.ConverterRegistry implements java.io.Serializable {
  public static cn.hutool.core.convert.ConverterRegistry getInstance();
  public cn.hutool.core.convert.ConverterRegistry();
  public cn.hutool.core.convert.ConverterRegistry putCustom(java.lang.reflect.Type, java.lang.Class<? extends cn.hutool.core.convert.Converter<?>>);
  public cn.hutool.core.convert.ConverterRegistry putCustom(java.lang.reflect.Type, cn.hutool.core.convert.Converter<?>);
  public <T> cn.hutool.core.convert.Converter<T> getConverter(java.lang.reflect.Type, boolean);
  public <T> cn.hutool.core.convert.Converter<T> getDefaultConverter(java.lang.reflect.Type);
  public <T> cn.hutool.core.convert.Converter<T> getCustomConverter(java.lang.reflect.Type);
  public <T> T convert(java.lang.reflect.Type, java.lang.Object, T, boolean) throws cn.hutool.core.convert.ConvertException;
  public <T> T convert(java.lang.reflect.Type, java.lang.Object, T) throws cn.hutool.core.convert.ConvertException;
  public <T> T convert(java.lang.reflect.Type, java.lang.Object) throws cn.hutool.core.convert.ConvertException;
}
```

## `cn.hutool.core.convert.NumberChineseFormatter`

```java
public class cn.hutool.core.convert.NumberChineseFormatter {
  public cn.hutool.core.convert.NumberChineseFormatter();
  public static java.lang.String format(double, boolean);
  public static java.lang.String format(double, boolean, boolean, java.lang.String, java.lang.String);
  public static java.lang.String format(double, boolean, boolean);
  public static java.lang.String format(long, boolean);
  public static java.lang.String formatSimple(long);
  public static java.lang.String formatThousand(int, boolean);
  public static java.lang.String format(java.math.BigDecimal, boolean, boolean);
  public static java.lang.String numberCharToChinese(char, boolean);
  public static java.math.BigDecimal chineseMoneyToNumber(java.lang.String);
  public static int chineseToNumber(java.lang.String);
}
```

## `cn.hutool.core.convert.NumberWithFormat`

```java
public class cn.hutool.core.convert.NumberWithFormat extends java.lang.Number implements cn.hutool.core.convert.TypeConverter, java.lang.Comparable<cn.hutool.core.convert.NumberWithFormat> {
  public cn.hutool.core.convert.NumberWithFormat(java.lang.Number, java.lang.String);
  public java.lang.Object convert(java.lang.reflect.Type, java.lang.Object);
  public java.lang.Object getNumber();
  public int intValue();
  public long longValue();
  public float floatValue();
  public double doubleValue();
  public java.lang.String toString();
  public int compareTo(cn.hutool.core.convert.NumberWithFormat);
  public int compareTo(java.lang.Object);
}
```

## `cn.hutool.core.convert.NumberWordFormatter`

```java
public class cn.hutool.core.convert.NumberWordFormatter {
  public cn.hutool.core.convert.NumberWordFormatter();
  public static java.lang.String format(java.lang.Object);
  public static java.lang.String formatSimple(long);
  public static java.lang.String formatSimple(long, boolean);
}
```

## `cn.hutool.core.convert.TypeConverter`

```java
public interface cn.hutool.core.convert.TypeConverter {
  public abstract java.lang.Object convert(java.lang.reflect.Type, java.lang.Object);
}
```
