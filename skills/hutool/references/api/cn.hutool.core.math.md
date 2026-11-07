# cn.hutool.core.math

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.math.Arrangement`

```java
public class cn.hutool.core.math.Arrangement implements java.io.Serializable {
  public cn.hutool.core.math.Arrangement(java.lang.String[]);
  public static long count(int);
  public static long count(int, int);
  public static long countAll(int);
  public java.util.List<java.lang.String[]> select();
  public java.util.List<java.lang.String[]> select(int);
  public java.util.List<java.lang.String[]> selectAll();
  public java.lang.Iterable<java.lang.String[]> iterate(int);
}
```

## `cn.hutool.core.math.BitStatusUtil`

```java
public class cn.hutool.core.math.BitStatusUtil {
  public cn.hutool.core.math.BitStatusUtil();
  public static int add(int, int);
  public static boolean has(int, int);
  public static int remove(int, int);
  public static int clear();
}
```

## `cn.hutool.core.math.Calculator`

```java
public class cn.hutool.core.math.Calculator {
  public cn.hutool.core.math.Calculator();
  public static double conversion(java.lang.String);
  public double calculate(java.lang.String);
}
```

## `cn.hutool.core.math.Combination`

```java
public class cn.hutool.core.math.Combination implements java.io.Serializable {
  public cn.hutool.core.math.Combination(java.lang.String[]);
  public static long count(int, int);
  public static java.math.BigInteger countBig(int, int);
  public static long countSafe(int, int);
  public static long countAll(int);
  public java.util.List<java.lang.String[]> select(int);
  public java.util.List<java.lang.String[]> selectAll();
}
```

## `cn.hutool.core.math.MathUtil`

```java
public class cn.hutool.core.math.MathUtil {
  public cn.hutool.core.math.MathUtil();
  public static long arrangementCount(int, int);
  public static long arrangementCount(int);
  public static java.util.List<java.lang.String[]> arrangementSelect(java.lang.String[], int);
  public static java.util.List<java.lang.String[]> arrangementSelect(java.lang.String[]);
  public static long combinationCount(int, int);
  public static java.util.List<java.lang.String[]> combinationSelect(java.lang.String[], int);
  public static long yuanToCent(double);
  public static double centToYuan(long);
}
```

## `cn.hutool.core.math.Money`

```java
public class cn.hutool.core.math.Money implements java.io.Serializable, java.lang.Comparable<cn.hutool.core.math.Money> {
  public cn.hutool.core.math.Money();
  public cn.hutool.core.math.Money(long, int);
  public cn.hutool.core.math.Money(long, int, java.util.Currency);
  public cn.hutool.core.math.Money(java.lang.String);
  public cn.hutool.core.math.Money(java.lang.String, java.util.Currency);
  public cn.hutool.core.math.Money(java.lang.String, java.util.Currency, java.math.RoundingMode);
  public cn.hutool.core.math.Money(double);
  public cn.hutool.core.math.Money(double, java.util.Currency);
  public cn.hutool.core.math.Money(java.math.BigDecimal);
  public cn.hutool.core.math.Money(java.math.BigDecimal, java.math.RoundingMode);
  public cn.hutool.core.math.Money(java.math.BigDecimal, java.util.Currency);
  public cn.hutool.core.math.Money(java.math.BigDecimal, java.util.Currency, java.math.RoundingMode);
  public java.math.BigDecimal getAmount();
  public void setAmount(java.math.BigDecimal);
  public long getCent();
  public java.util.Currency getCurrency();
  public int getCentFactor();
  public boolean equals(java.lang.Object);
  public boolean equals(cn.hutool.core.math.Money);
  public int hashCode();
  public int compareTo(cn.hutool.core.math.Money);
  public boolean greaterThan(cn.hutool.core.math.Money);
  public cn.hutool.core.math.Money add(cn.hutool.core.math.Money);
  public cn.hutool.core.math.Money addTo(cn.hutool.core.math.Money);
  public cn.hutool.core.math.Money subtract(cn.hutool.core.math.Money);
  public cn.hutool.core.math.Money subtractFrom(cn.hutool.core.math.Money);
  public cn.hutool.core.math.Money multiply(long);
  public cn.hutool.core.math.Money multiplyBy(long);
  public cn.hutool.core.math.Money multiply(double);
  public cn.hutool.core.math.Money multiplyBy(double);
  public cn.hutool.core.math.Money multiply(java.math.BigDecimal);
  public cn.hutool.core.math.Money multiplyBy(java.math.BigDecimal);
  public cn.hutool.core.math.Money multiply(java.math.BigDecimal, java.math.RoundingMode);
  public cn.hutool.core.math.Money multiplyBy(java.math.BigDecimal, java.math.RoundingMode);
  public cn.hutool.core.math.Money divide(double);
  public cn.hutool.core.math.Money divideBy(double);
  public cn.hutool.core.math.Money divide(java.math.BigDecimal);
  public cn.hutool.core.math.Money divide(java.math.BigDecimal, java.math.RoundingMode);
  public cn.hutool.core.math.Money divideBy(java.math.BigDecimal);
  public cn.hutool.core.math.Money divideBy(java.math.BigDecimal, java.math.RoundingMode);
  public cn.hutool.core.math.Money[] allocate(int);
  public cn.hutool.core.math.Money[] allocate(long[]);
  public java.lang.String toString();
  public java.lang.String dump();
  public void setCent(long);
  public int compareTo(java.lang.Object);
}
```
