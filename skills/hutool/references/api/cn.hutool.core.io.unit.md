# cn.hutool.core.io.unit

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.io.unit.DataSize`

```java
public final class cn.hutool.core.io.unit.DataSize implements java.lang.Comparable<cn.hutool.core.io.unit.DataSize> {
  public static cn.hutool.core.io.unit.DataSize ofBytes(long);
  public static cn.hutool.core.io.unit.DataSize ofKilobytes(long);
  public static cn.hutool.core.io.unit.DataSize ofMegabytes(long);
  public static cn.hutool.core.io.unit.DataSize ofGigabytes(long);
  public static cn.hutool.core.io.unit.DataSize ofTerabytes(long);
  public static cn.hutool.core.io.unit.DataSize of(long, cn.hutool.core.io.unit.DataUnit);
  public static cn.hutool.core.io.unit.DataSize of(java.math.BigDecimal, cn.hutool.core.io.unit.DataUnit);
  public static cn.hutool.core.io.unit.DataSize parse(java.lang.CharSequence);
  public static cn.hutool.core.io.unit.DataSize parse(java.lang.CharSequence, cn.hutool.core.io.unit.DataUnit);
  public boolean isNegative();
  public long toBytes();
  public long toKilobytes();
  public long toMegabytes();
  public long toGigabytes();
  public long toTerabytes();
  public int compareTo(cn.hutool.core.io.unit.DataSize);
  public java.lang.String toString();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public int compareTo(java.lang.Object);
}
```

## `cn.hutool.core.io.unit.DataSizeUtil`

```java
public class cn.hutool.core.io.unit.DataSizeUtil {
  public cn.hutool.core.io.unit.DataSizeUtil();
  public static long parse(java.lang.String);
  public static java.lang.String format(long);
  public static java.lang.String format(java.lang.Long, cn.hutool.core.io.unit.DataUnit);
}
```

## `cn.hutool.core.io.unit.DataUnit`

```java
public final class cn.hutool.core.io.unit.DataUnit extends java.lang.Enum<cn.hutool.core.io.unit.DataUnit> {
  public static cn.hutool.core.io.unit.DataUnit[] values();
  public static cn.hutool.core.io.unit.DataUnit valueOf(java.lang.String);
  public java.lang.String getSuffix();
  public static cn.hutool.core.io.unit.DataUnit fromSuffix(java.lang.String);
}
```
