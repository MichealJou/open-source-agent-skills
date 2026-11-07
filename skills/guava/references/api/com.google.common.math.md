# com.google.common.math

版本：33.4.8-jre。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.google.common.math.BigDecimalMath`

```java
public class com.google.common.math.BigDecimalMath {
  public static double roundToDouble(java.math.BigDecimal, java.math.RoundingMode);
}
```

## `com.google.common.math.BigIntegerMath`

```java
public final class com.google.common.math.BigIntegerMath {
  public static java.math.BigInteger ceilingPowerOfTwo(java.math.BigInteger);
  public static java.math.BigInteger floorPowerOfTwo(java.math.BigInteger);
  public static boolean isPowerOfTwo(java.math.BigInteger);
  public static int log2(java.math.BigInteger, java.math.RoundingMode);
  public static int log10(java.math.BigInteger, java.math.RoundingMode);
  public static java.math.BigInteger sqrt(java.math.BigInteger, java.math.RoundingMode);
  public static double roundToDouble(java.math.BigInteger, java.math.RoundingMode);
  public static java.math.BigInteger divide(java.math.BigInteger, java.math.BigInteger, java.math.RoundingMode);
  public static java.math.BigInteger factorial(int);
  public static java.math.BigInteger binomial(int, int);
}
```

## `com.google.common.math.DoubleMath`

```java
public final class com.google.common.math.DoubleMath {
  public static int roundToInt(double, java.math.RoundingMode);
  public static long roundToLong(double, java.math.RoundingMode);
  public static java.math.BigInteger roundToBigInteger(double, java.math.RoundingMode);
  public static boolean isPowerOfTwo(double);
  public static double log2(double);
  public static int log2(double, java.math.RoundingMode);
  public static boolean isMathematicalInteger(double);
  public static double factorial(int);
  public static boolean fuzzyEquals(double, double, double);
  public static int fuzzyCompare(double, double, double);
  public static double mean(double...);
  public static double mean(int...);
  public static double mean(long...);
  public static double mean(java.lang.Iterable<? extends java.lang.Number>);
  public static double mean(java.util.Iterator<? extends java.lang.Number>);
}
```

## `com.google.common.math.IntMath`

```java
public final class com.google.common.math.IntMath {
  public static int ceilingPowerOfTwo(int);
  public static int floorPowerOfTwo(int);
  public static boolean isPowerOfTwo(int);
  public static int log2(int, java.math.RoundingMode);
  public static int log10(int, java.math.RoundingMode);
  public static int pow(int, int);
  public static int sqrt(int, java.math.RoundingMode);
  public static int divide(int, int, java.math.RoundingMode);
  public static int mod(int, int);
  public static int gcd(int, int);
  public static int checkedAdd(int, int);
  public static int checkedSubtract(int, int);
  public static int checkedMultiply(int, int);
  public static int checkedPow(int, int);
  public static int saturatedAdd(int, int);
  public static int saturatedSubtract(int, int);
  public static int saturatedMultiply(int, int);
  public static int saturatedPow(int, int);
  public static int factorial(int);
  public static int binomial(int, int);
  public static int mean(int, int);
  public static boolean isPrime(int);
}
```

## `com.google.common.math.LinearTransformation`

```java
public abstract class com.google.common.math.LinearTransformation {
  public com.google.common.math.LinearTransformation();
  public static com.google.common.math.LinearTransformation$LinearTransformationBuilder mapping(double, double);
  public static com.google.common.math.LinearTransformation vertical(double);
  public static com.google.common.math.LinearTransformation horizontal(double);
  public static com.google.common.math.LinearTransformation forNaN();
  public abstract boolean isVertical();
  public abstract boolean isHorizontal();
  public abstract double slope();
  public abstract double transform(double);
  public abstract com.google.common.math.LinearTransformation inverse();
}
```

## `com.google.common.math.LinearTransformation$LinearTransformationBuilder`

```java
public final class com.google.common.math.LinearTransformation$LinearTransformationBuilder {
  public com.google.common.math.LinearTransformation and(double, double);
  public com.google.common.math.LinearTransformation withSlope(double);
}
```

## `com.google.common.math.LongMath`

```java
public final class com.google.common.math.LongMath {
  public static long ceilingPowerOfTwo(long);
  public static long floorPowerOfTwo(long);
  public static boolean isPowerOfTwo(long);
  public static int log2(long, java.math.RoundingMode);
  public static int log10(long, java.math.RoundingMode);
  public static long pow(long, int);
  public static long sqrt(long, java.math.RoundingMode);
  public static long divide(long, long, java.math.RoundingMode);
  public static int mod(long, int);
  public static long mod(long, long);
  public static long gcd(long, long);
  public static long checkedAdd(long, long);
  public static long checkedSubtract(long, long);
  public static long checkedMultiply(long, long);
  public static long checkedPow(long, int);
  public static long saturatedAdd(long, long);
  public static long saturatedSubtract(long, long);
  public static long saturatedMultiply(long, long);
  public static long saturatedPow(long, int);
  public static long factorial(int);
  public static long binomial(int, int);
  public static long mean(long, long);
  public static boolean isPrime(long);
  public static double roundToDouble(long, java.math.RoundingMode);
}
```

## `com.google.common.math.PairedStats`

```java
public final class com.google.common.math.PairedStats implements java.io.Serializable {
  public long count();
  public com.google.common.math.Stats xStats();
  public com.google.common.math.Stats yStats();
  public double populationCovariance();
  public double sampleCovariance();
  public double pearsonsCorrelationCoefficient();
  public com.google.common.math.LinearTransformation leastSquaresFit();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
  public byte[] toByteArray();
  public static com.google.common.math.PairedStats fromByteArray(byte[]);
}
```

## `com.google.common.math.PairedStatsAccumulator`

```java
public final class com.google.common.math.PairedStatsAccumulator {
  public com.google.common.math.PairedStatsAccumulator();
  public void add(double, double);
  public void addAll(com.google.common.math.PairedStats);
  public com.google.common.math.PairedStats snapshot();
  public long count();
  public com.google.common.math.Stats xStats();
  public com.google.common.math.Stats yStats();
  public double populationCovariance();
  public final double sampleCovariance();
  public final double pearsonsCorrelationCoefficient();
  public final com.google.common.math.LinearTransformation leastSquaresFit();
}
```

## `com.google.common.math.Quantiles`

```java
public final class com.google.common.math.Quantiles {
  public com.google.common.math.Quantiles();
  public static com.google.common.math.Quantiles$ScaleAndIndex median();
  public static com.google.common.math.Quantiles$Scale quartiles();
  public static com.google.common.math.Quantiles$Scale percentiles();
  public static com.google.common.math.Quantiles$Scale scale(int);
}
```

## `com.google.common.math.Quantiles$Scale`

```java
public final class com.google.common.math.Quantiles$Scale {
  public com.google.common.math.Quantiles$ScaleAndIndex index(int);
  public com.google.common.math.Quantiles$ScaleAndIndexes indexes(int...);
  public com.google.common.math.Quantiles$ScaleAndIndexes indexes(java.util.Collection<java.lang.Integer>);
}
```

## `com.google.common.math.Quantiles$ScaleAndIndex`

```java
public final class com.google.common.math.Quantiles$ScaleAndIndex {
  public double compute(java.util.Collection<? extends java.lang.Number>);
  public double compute(double...);
  public double compute(long...);
  public double compute(int...);
  public double computeInPlace(double...);
}
```

## `com.google.common.math.Quantiles$ScaleAndIndexes`

```java
public final class com.google.common.math.Quantiles$ScaleAndIndexes {
  public java.util.Map<java.lang.Integer, java.lang.Double> compute(java.util.Collection<? extends java.lang.Number>);
  public java.util.Map<java.lang.Integer, java.lang.Double> compute(double...);
  public java.util.Map<java.lang.Integer, java.lang.Double> compute(long...);
  public java.util.Map<java.lang.Integer, java.lang.Double> compute(int...);
  public java.util.Map<java.lang.Integer, java.lang.Double> computeInPlace(double...);
}
```

## `com.google.common.math.Stats`

```java
public final class com.google.common.math.Stats implements java.io.Serializable {
  public static com.google.common.math.Stats of(java.lang.Iterable<? extends java.lang.Number>);
  public static com.google.common.math.Stats of(java.util.Iterator<? extends java.lang.Number>);
  public static com.google.common.math.Stats of(double...);
  public static com.google.common.math.Stats of(int...);
  public static com.google.common.math.Stats of(long...);
  public static com.google.common.math.Stats of(java.util.stream.DoubleStream);
  public static com.google.common.math.Stats of(java.util.stream.IntStream);
  public static com.google.common.math.Stats of(java.util.stream.LongStream);
  public static java.util.stream.Collector<java.lang.Number, com.google.common.math.StatsAccumulator, com.google.common.math.Stats> toStats();
  public long count();
  public double mean();
  public double sum();
  public double populationVariance();
  public double populationStandardDeviation();
  public double sampleVariance();
  public double sampleStandardDeviation();
  public double min();
  public double max();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
  public static double meanOf(java.lang.Iterable<? extends java.lang.Number>);
  public static double meanOf(java.util.Iterator<? extends java.lang.Number>);
  public static double meanOf(double...);
  public static double meanOf(int...);
  public static double meanOf(long...);
  public byte[] toByteArray();
  public static com.google.common.math.Stats fromByteArray(byte[]);
}
```

## `com.google.common.math.StatsAccumulator`

```java
public final class com.google.common.math.StatsAccumulator {
  public com.google.common.math.StatsAccumulator();
  public void add(double);
  public void addAll(java.lang.Iterable<? extends java.lang.Number>);
  public void addAll(java.util.Iterator<? extends java.lang.Number>);
  public void addAll(double...);
  public void addAll(int...);
  public void addAll(long...);
  public void addAll(java.util.stream.DoubleStream);
  public void addAll(java.util.stream.IntStream);
  public void addAll(java.util.stream.LongStream);
  public void addAll(com.google.common.math.Stats);
  public void addAll(com.google.common.math.StatsAccumulator);
  public com.google.common.math.Stats snapshot();
  public long count();
  public double mean();
  public final double sum();
  public final double populationVariance();
  public final double populationStandardDeviation();
  public final double sampleVariance();
  public final double sampleStandardDeviation();
  public double min();
  public double max();
}
```
