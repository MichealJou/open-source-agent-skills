# com.google.common.primitives

版本：33.4.8-jre。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.google.common.primitives.Booleans`

```java
public final class com.google.common.primitives.Booleans {
  public static java.util.Comparator<java.lang.Boolean> trueFirst();
  public static java.util.Comparator<java.lang.Boolean> falseFirst();
  public static int hashCode(boolean);
  public static int compare(boolean, boolean);
  public static boolean contains(boolean[], boolean);
  public static int indexOf(boolean[], boolean);
  public static int indexOf(boolean[], boolean[]);
  public static int lastIndexOf(boolean[], boolean);
  public static boolean[] concat(boolean[]...);
  public static boolean[] ensureCapacity(boolean[], int, int);
  public static java.lang.String join(java.lang.String, boolean...);
  public static java.util.Comparator<boolean[]> lexicographicalComparator();
  public static boolean[] toArray(java.util.Collection<java.lang.Boolean>);
  public static java.util.List<java.lang.Boolean> asList(boolean...);
  public static int countTrue(boolean...);
  public static void reverse(boolean[]);
  public static void reverse(boolean[], int, int);
  public static void rotate(boolean[], int);
  public static void rotate(boolean[], int, int, int);
}
```

## `com.google.common.primitives.Bytes`

```java
public final class com.google.common.primitives.Bytes {
  public static int hashCode(byte);
  public static boolean contains(byte[], byte);
  public static int indexOf(byte[], byte);
  public static int indexOf(byte[], byte[]);
  public static int lastIndexOf(byte[], byte);
  public static byte[] concat(byte[]...);
  public static byte[] ensureCapacity(byte[], int, int);
  public static byte[] toArray(java.util.Collection<? extends java.lang.Number>);
  public static java.util.List<java.lang.Byte> asList(byte...);
  public static void reverse(byte[]);
  public static void reverse(byte[], int, int);
  public static void rotate(byte[], int);
  public static void rotate(byte[], int, int, int);
}
```

## `com.google.common.primitives.Chars`

```java
public final class com.google.common.primitives.Chars {
  public static int hashCode(char);
  public static char checkedCast(long);
  public static char saturatedCast(long);
  public static int compare(char, char);
  public static boolean contains(char[], char);
  public static int indexOf(char[], char);
  public static int indexOf(char[], char[]);
  public static int lastIndexOf(char[], char);
  public static char min(char...);
  public static char max(char...);
  public static char constrainToRange(char, char, char);
  public static char[] concat(char[]...);
  public static byte[] toByteArray(char);
  public static char fromByteArray(byte[]);
  public static char fromBytes(byte, byte);
  public static char[] ensureCapacity(char[], int, int);
  public static java.lang.String join(java.lang.String, char...);
  public static java.util.Comparator<char[]> lexicographicalComparator();
  public static char[] toArray(java.util.Collection<java.lang.Character>);
  public static void sortDescending(char[]);
  public static void sortDescending(char[], int, int);
  public static void reverse(char[]);
  public static void reverse(char[], int, int);
  public static void rotate(char[], int);
  public static void rotate(char[], int, int, int);
  public static java.util.List<java.lang.Character> asList(char...);
}
```

## `com.google.common.primitives.Doubles`

```java
public final class com.google.common.primitives.Doubles extends com.google.common.primitives.DoublesMethodsForWeb {
  public static int hashCode(double);
  public static int compare(double, double);
  public static boolean isFinite(double);
  public static boolean contains(double[], double);
  public static int indexOf(double[], double);
  public static int indexOf(double[], double[]);
  public static int lastIndexOf(double[], double);
  public static double min(double...);
  public static double max(double...);
  public static double constrainToRange(double, double, double);
  public static double[] concat(double[]...);
  public static com.google.common.base.Converter<java.lang.String, java.lang.Double> stringConverter();
  public static double[] ensureCapacity(double[], int, int);
  public static java.lang.String join(java.lang.String, double...);
  public static java.util.Comparator<double[]> lexicographicalComparator();
  public static void sortDescending(double[]);
  public static void sortDescending(double[], int, int);
  public static void reverse(double[]);
  public static void reverse(double[], int, int);
  public static void rotate(double[], int);
  public static void rotate(double[], int, int, int);
  public static double[] toArray(java.util.Collection<? extends java.lang.Number>);
  public static java.util.List<java.lang.Double> asList(double...);
  public static java.lang.Double tryParse(java.lang.String);
}
```

## `com.google.common.primitives.Floats`

```java
public final class com.google.common.primitives.Floats extends com.google.common.primitives.FloatsMethodsForWeb {
  public static int hashCode(float);
  public static int compare(float, float);
  public static boolean isFinite(float);
  public static boolean contains(float[], float);
  public static int indexOf(float[], float);
  public static int indexOf(float[], float[]);
  public static int lastIndexOf(float[], float);
  public static float min(float...);
  public static float max(float...);
  public static float constrainToRange(float, float, float);
  public static float[] concat(float[]...);
  public static com.google.common.base.Converter<java.lang.String, java.lang.Float> stringConverter();
  public static float[] ensureCapacity(float[], int, int);
  public static java.lang.String join(java.lang.String, float...);
  public static java.util.Comparator<float[]> lexicographicalComparator();
  public static void sortDescending(float[]);
  public static void sortDescending(float[], int, int);
  public static void reverse(float[]);
  public static void reverse(float[], int, int);
  public static void rotate(float[], int);
  public static void rotate(float[], int, int, int);
  public static float[] toArray(java.util.Collection<? extends java.lang.Number>);
  public static java.util.List<java.lang.Float> asList(float...);
  public static java.lang.Float tryParse(java.lang.String);
}
```

## `com.google.common.primitives.ImmutableDoubleArray`

```java
public final class com.google.common.primitives.ImmutableDoubleArray implements java.io.Serializable {
  public static com.google.common.primitives.ImmutableDoubleArray of();
  public static com.google.common.primitives.ImmutableDoubleArray of(double);
  public static com.google.common.primitives.ImmutableDoubleArray of(double, double);
  public static com.google.common.primitives.ImmutableDoubleArray of(double, double, double);
  public static com.google.common.primitives.ImmutableDoubleArray of(double, double, double, double);
  public static com.google.common.primitives.ImmutableDoubleArray of(double, double, double, double, double);
  public static com.google.common.primitives.ImmutableDoubleArray of(double, double, double, double, double, double);
  public static com.google.common.primitives.ImmutableDoubleArray of(double, double...);
  public static com.google.common.primitives.ImmutableDoubleArray copyOf(double[]);
  public static com.google.common.primitives.ImmutableDoubleArray copyOf(java.util.Collection<java.lang.Double>);
  public static com.google.common.primitives.ImmutableDoubleArray copyOf(java.lang.Iterable<java.lang.Double>);
  public static com.google.common.primitives.ImmutableDoubleArray copyOf(java.util.stream.DoubleStream);
  public static com.google.common.primitives.ImmutableDoubleArray$Builder builder(int);
  public static com.google.common.primitives.ImmutableDoubleArray$Builder builder();
  public int length();
  public boolean isEmpty();
  public double get(int);
  public int indexOf(double);
  public int lastIndexOf(double);
  public boolean contains(double);
  public void forEach(java.util.function.DoubleConsumer);
  public java.util.stream.DoubleStream stream();
  public double[] toArray();
  public com.google.common.primitives.ImmutableDoubleArray subArray(int, int);
  public java.util.List<java.lang.Double> asList();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
  public com.google.common.primitives.ImmutableDoubleArray trimmed();
}
```

## `com.google.common.primitives.ImmutableDoubleArray$Builder`

```java
public final class com.google.common.primitives.ImmutableDoubleArray$Builder {
  public com.google.common.primitives.ImmutableDoubleArray$Builder add(double);
  public com.google.common.primitives.ImmutableDoubleArray$Builder addAll(double[]);
  public com.google.common.primitives.ImmutableDoubleArray$Builder addAll(java.lang.Iterable<java.lang.Double>);
  public com.google.common.primitives.ImmutableDoubleArray$Builder addAll(java.util.Collection<java.lang.Double>);
  public com.google.common.primitives.ImmutableDoubleArray$Builder addAll(java.util.stream.DoubleStream);
  public com.google.common.primitives.ImmutableDoubleArray$Builder addAll(com.google.common.primitives.ImmutableDoubleArray);
  public com.google.common.primitives.ImmutableDoubleArray build();
}
```

## `com.google.common.primitives.ImmutableIntArray`

```java
public final class com.google.common.primitives.ImmutableIntArray implements java.io.Serializable {
  public static com.google.common.primitives.ImmutableIntArray of();
  public static com.google.common.primitives.ImmutableIntArray of(int);
  public static com.google.common.primitives.ImmutableIntArray of(int, int);
  public static com.google.common.primitives.ImmutableIntArray of(int, int, int);
  public static com.google.common.primitives.ImmutableIntArray of(int, int, int, int);
  public static com.google.common.primitives.ImmutableIntArray of(int, int, int, int, int);
  public static com.google.common.primitives.ImmutableIntArray of(int, int, int, int, int, int);
  public static com.google.common.primitives.ImmutableIntArray of(int, int...);
  public static com.google.common.primitives.ImmutableIntArray copyOf(int[]);
  public static com.google.common.primitives.ImmutableIntArray copyOf(java.util.Collection<java.lang.Integer>);
  public static com.google.common.primitives.ImmutableIntArray copyOf(java.lang.Iterable<java.lang.Integer>);
  public static com.google.common.primitives.ImmutableIntArray copyOf(java.util.stream.IntStream);
  public static com.google.common.primitives.ImmutableIntArray$Builder builder(int);
  public static com.google.common.primitives.ImmutableIntArray$Builder builder();
  public int length();
  public boolean isEmpty();
  public int get(int);
  public int indexOf(int);
  public int lastIndexOf(int);
  public boolean contains(int);
  public void forEach(java.util.function.IntConsumer);
  public java.util.stream.IntStream stream();
  public int[] toArray();
  public com.google.common.primitives.ImmutableIntArray subArray(int, int);
  public java.util.List<java.lang.Integer> asList();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
  public com.google.common.primitives.ImmutableIntArray trimmed();
}
```

## `com.google.common.primitives.ImmutableIntArray$Builder`

```java
public final class com.google.common.primitives.ImmutableIntArray$Builder {
  public com.google.common.primitives.ImmutableIntArray$Builder add(int);
  public com.google.common.primitives.ImmutableIntArray$Builder addAll(int[]);
  public com.google.common.primitives.ImmutableIntArray$Builder addAll(java.lang.Iterable<java.lang.Integer>);
  public com.google.common.primitives.ImmutableIntArray$Builder addAll(java.util.Collection<java.lang.Integer>);
  public com.google.common.primitives.ImmutableIntArray$Builder addAll(java.util.stream.IntStream);
  public com.google.common.primitives.ImmutableIntArray$Builder addAll(com.google.common.primitives.ImmutableIntArray);
  public com.google.common.primitives.ImmutableIntArray build();
}
```

## `com.google.common.primitives.ImmutableLongArray`

```java
public final class com.google.common.primitives.ImmutableLongArray implements java.io.Serializable {
  public static com.google.common.primitives.ImmutableLongArray of();
  public static com.google.common.primitives.ImmutableLongArray of(long);
  public static com.google.common.primitives.ImmutableLongArray of(long, long);
  public static com.google.common.primitives.ImmutableLongArray of(long, long, long);
  public static com.google.common.primitives.ImmutableLongArray of(long, long, long, long);
  public static com.google.common.primitives.ImmutableLongArray of(long, long, long, long, long);
  public static com.google.common.primitives.ImmutableLongArray of(long, long, long, long, long, long);
  public static com.google.common.primitives.ImmutableLongArray of(long, long...);
  public static com.google.common.primitives.ImmutableLongArray copyOf(long[]);
  public static com.google.common.primitives.ImmutableLongArray copyOf(java.util.Collection<java.lang.Long>);
  public static com.google.common.primitives.ImmutableLongArray copyOf(java.lang.Iterable<java.lang.Long>);
  public static com.google.common.primitives.ImmutableLongArray copyOf(java.util.stream.LongStream);
  public static com.google.common.primitives.ImmutableLongArray$Builder builder(int);
  public static com.google.common.primitives.ImmutableLongArray$Builder builder();
  public int length();
  public boolean isEmpty();
  public long get(int);
  public int indexOf(long);
  public int lastIndexOf(long);
  public boolean contains(long);
  public void forEach(java.util.function.LongConsumer);
  public java.util.stream.LongStream stream();
  public long[] toArray();
  public com.google.common.primitives.ImmutableLongArray subArray(int, int);
  public java.util.List<java.lang.Long> asList();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
  public com.google.common.primitives.ImmutableLongArray trimmed();
}
```

## `com.google.common.primitives.ImmutableLongArray$Builder`

```java
public final class com.google.common.primitives.ImmutableLongArray$Builder {
  public com.google.common.primitives.ImmutableLongArray$Builder add(long);
  public com.google.common.primitives.ImmutableLongArray$Builder addAll(long[]);
  public com.google.common.primitives.ImmutableLongArray$Builder addAll(java.lang.Iterable<java.lang.Long>);
  public com.google.common.primitives.ImmutableLongArray$Builder addAll(java.util.Collection<java.lang.Long>);
  public com.google.common.primitives.ImmutableLongArray$Builder addAll(java.util.stream.LongStream);
  public com.google.common.primitives.ImmutableLongArray$Builder addAll(com.google.common.primitives.ImmutableLongArray);
  public com.google.common.primitives.ImmutableLongArray build();
}
```

## `com.google.common.primitives.Ints`

```java
public final class com.google.common.primitives.Ints extends com.google.common.primitives.IntsMethodsForWeb {
  public static int hashCode(int);
  public static int checkedCast(long);
  public static int saturatedCast(long);
  public static int compare(int, int);
  public static boolean contains(int[], int);
  public static int indexOf(int[], int);
  public static int indexOf(int[], int[]);
  public static int lastIndexOf(int[], int);
  public static int min(int...);
  public static int max(int...);
  public static int constrainToRange(int, int, int);
  public static int[] concat(int[]...);
  public static byte[] toByteArray(int);
  public static int fromByteArray(byte[]);
  public static int fromBytes(byte, byte, byte, byte);
  public static com.google.common.base.Converter<java.lang.String, java.lang.Integer> stringConverter();
  public static int[] ensureCapacity(int[], int, int);
  public static java.lang.String join(java.lang.String, int...);
  public static java.util.Comparator<int[]> lexicographicalComparator();
  public static void sortDescending(int[]);
  public static void sortDescending(int[], int, int);
  public static void reverse(int[]);
  public static void reverse(int[], int, int);
  public static void rotate(int[], int);
  public static void rotate(int[], int, int, int);
  public static int[] toArray(java.util.Collection<? extends java.lang.Number>);
  public static java.util.List<java.lang.Integer> asList(int...);
  public static java.lang.Integer tryParse(java.lang.String);
  public static java.lang.Integer tryParse(java.lang.String, int);
}
```

## `com.google.common.primitives.Longs`

```java
public final class com.google.common.primitives.Longs {
  public static int hashCode(long);
  public static int compare(long, long);
  public static boolean contains(long[], long);
  public static int indexOf(long[], long);
  public static int indexOf(long[], long[]);
  public static int lastIndexOf(long[], long);
  public static long min(long...);
  public static long max(long...);
  public static long constrainToRange(long, long, long);
  public static long[] concat(long[]...);
  public static byte[] toByteArray(long);
  public static long fromByteArray(byte[]);
  public static long fromBytes(byte, byte, byte, byte, byte, byte, byte, byte);
  public static java.lang.Long tryParse(java.lang.String);
  public static java.lang.Long tryParse(java.lang.String, int);
  public static com.google.common.base.Converter<java.lang.String, java.lang.Long> stringConverter();
  public static long[] ensureCapacity(long[], int, int);
  public static java.lang.String join(java.lang.String, long...);
  public static java.util.Comparator<long[]> lexicographicalComparator();
  public static void sortDescending(long[]);
  public static void sortDescending(long[], int, int);
  public static void reverse(long[]);
  public static void reverse(long[], int, int);
  public static void rotate(long[], int);
  public static void rotate(long[], int, int, int);
  public static long[] toArray(java.util.Collection<? extends java.lang.Number>);
  public static java.util.List<java.lang.Long> asList(long...);
}
```

## `com.google.common.primitives.Primitives`

```java
public final class com.google.common.primitives.Primitives {
  public static java.util.Set<java.lang.Class<?>> allPrimitiveTypes();
  public static java.util.Set<java.lang.Class<?>> allWrapperTypes();
  public static boolean isWrapperType(java.lang.Class<?>);
  public static <T> java.lang.Class<T> wrap(java.lang.Class<T>);
  public static <T> java.lang.Class<T> unwrap(java.lang.Class<T>);
}
```

## `com.google.common.primitives.Shorts`

```java
public final class com.google.common.primitives.Shorts extends com.google.common.primitives.ShortsMethodsForWeb {
  public static int hashCode(short);
  public static short checkedCast(long);
  public static short saturatedCast(long);
  public static int compare(short, short);
  public static boolean contains(short[], short);
  public static int indexOf(short[], short);
  public static int indexOf(short[], short[]);
  public static int lastIndexOf(short[], short);
  public static short min(short...);
  public static short max(short...);
  public static short constrainToRange(short, short, short);
  public static short[] concat(short[]...);
  public static byte[] toByteArray(short);
  public static short fromByteArray(byte[]);
  public static short fromBytes(byte, byte);
  public static com.google.common.base.Converter<java.lang.String, java.lang.Short> stringConverter();
  public static short[] ensureCapacity(short[], int, int);
  public static java.lang.String join(java.lang.String, short...);
  public static java.util.Comparator<short[]> lexicographicalComparator();
  public static void sortDescending(short[]);
  public static void sortDescending(short[], int, int);
  public static void reverse(short[]);
  public static void reverse(short[], int, int);
  public static void rotate(short[], int);
  public static void rotate(short[], int, int, int);
  public static short[] toArray(java.util.Collection<? extends java.lang.Number>);
  public static java.util.List<java.lang.Short> asList(short...);
}
```

## `com.google.common.primitives.SignedBytes`

```java
public final class com.google.common.primitives.SignedBytes {
  public static byte checkedCast(long);
  public static byte saturatedCast(long);
  public static int compare(byte, byte);
  public static byte min(byte...);
  public static byte max(byte...);
  public static java.lang.String join(java.lang.String, byte...);
  public static java.util.Comparator<byte[]> lexicographicalComparator();
  public static void sortDescending(byte[]);
  public static void sortDescending(byte[], int, int);
}
```

## `com.google.common.primitives.UnsignedBytes`

```java
public final class com.google.common.primitives.UnsignedBytes {
  public static int toInt(byte);
  public static byte checkedCast(long);
  public static byte saturatedCast(long);
  public static int compare(byte, byte);
  public static byte min(byte...);
  public static byte max(byte...);
  public static java.lang.String toString(byte);
  public static java.lang.String toString(byte, int);
  public static byte parseUnsignedByte(java.lang.String);
  public static byte parseUnsignedByte(java.lang.String, int);
  public static java.lang.String join(java.lang.String, byte...);
  public static java.util.Comparator<byte[]> lexicographicalComparator();
  public static void sort(byte[]);
  public static void sort(byte[], int, int);
  public static void sortDescending(byte[]);
  public static void sortDescending(byte[], int, int);
}
```

## `com.google.common.primitives.UnsignedInteger`

```java
public final class com.google.common.primitives.UnsignedInteger extends java.lang.Number implements java.lang.Comparable<com.google.common.primitives.UnsignedInteger> {
  public static com.google.common.primitives.UnsignedInteger fromIntBits(int);
  public static com.google.common.primitives.UnsignedInteger valueOf(long);
  public static com.google.common.primitives.UnsignedInteger valueOf(java.math.BigInteger);
  public static com.google.common.primitives.UnsignedInteger valueOf(java.lang.String);
  public static com.google.common.primitives.UnsignedInteger valueOf(java.lang.String, int);
  public com.google.common.primitives.UnsignedInteger plus(com.google.common.primitives.UnsignedInteger);
  public com.google.common.primitives.UnsignedInteger minus(com.google.common.primitives.UnsignedInteger);
  public com.google.common.primitives.UnsignedInteger times(com.google.common.primitives.UnsignedInteger);
  public com.google.common.primitives.UnsignedInteger dividedBy(com.google.common.primitives.UnsignedInteger);
  public com.google.common.primitives.UnsignedInteger mod(com.google.common.primitives.UnsignedInteger);
  public int intValue();
  public long longValue();
  public float floatValue();
  public double doubleValue();
  public java.math.BigInteger bigIntegerValue();
  public int compareTo(com.google.common.primitives.UnsignedInteger);
  public int hashCode();
  public boolean equals(java.lang.Object);
  public java.lang.String toString();
  public java.lang.String toString(int);
  public int compareTo(java.lang.Object);
}
```

## `com.google.common.primitives.UnsignedInts`

```java
public final class com.google.common.primitives.UnsignedInts {
  public static int compare(int, int);
  public static long toLong(int);
  public static int checkedCast(long);
  public static int saturatedCast(long);
  public static int min(int...);
  public static int max(int...);
  public static java.lang.String join(java.lang.String, int...);
  public static java.util.Comparator<int[]> lexicographicalComparator();
  public static void sort(int[]);
  public static void sort(int[], int, int);
  public static void sortDescending(int[]);
  public static void sortDescending(int[], int, int);
  public static int divide(int, int);
  public static int remainder(int, int);
  public static int decode(java.lang.String);
  public static int parseUnsignedInt(java.lang.String);
  public static int parseUnsignedInt(java.lang.String, int);
  public static java.lang.String toString(int);
  public static java.lang.String toString(int, int);
}
```

## `com.google.common.primitives.UnsignedLong`

```java
public final class com.google.common.primitives.UnsignedLong extends java.lang.Number implements java.lang.Comparable<com.google.common.primitives.UnsignedLong> {
  public static com.google.common.primitives.UnsignedLong fromLongBits(long);
  public static com.google.common.primitives.UnsignedLong valueOf(long);
  public static com.google.common.primitives.UnsignedLong valueOf(java.math.BigInteger);
  public static com.google.common.primitives.UnsignedLong valueOf(java.lang.String);
  public static com.google.common.primitives.UnsignedLong valueOf(java.lang.String, int);
  public com.google.common.primitives.UnsignedLong plus(com.google.common.primitives.UnsignedLong);
  public com.google.common.primitives.UnsignedLong minus(com.google.common.primitives.UnsignedLong);
  public com.google.common.primitives.UnsignedLong times(com.google.common.primitives.UnsignedLong);
  public com.google.common.primitives.UnsignedLong dividedBy(com.google.common.primitives.UnsignedLong);
  public com.google.common.primitives.UnsignedLong mod(com.google.common.primitives.UnsignedLong);
  public int intValue();
  public long longValue();
  public float floatValue();
  public double doubleValue();
  public java.math.BigInteger bigIntegerValue();
  public int compareTo(com.google.common.primitives.UnsignedLong);
  public int hashCode();
  public boolean equals(java.lang.Object);
  public java.lang.String toString();
  public java.lang.String toString(int);
  public int compareTo(java.lang.Object);
}
```

## `com.google.common.primitives.UnsignedLongs`

```java
public final class com.google.common.primitives.UnsignedLongs {
  public static int compare(long, long);
  public static long min(long...);
  public static long max(long...);
  public static java.lang.String join(java.lang.String, long...);
  public static java.util.Comparator<long[]> lexicographicalComparator();
  public static void sort(long[]);
  public static void sort(long[], int, int);
  public static void sortDescending(long[]);
  public static void sortDescending(long[], int, int);
  public static long divide(long, long);
  public static long remainder(long, long);
  public static long parseUnsignedLong(java.lang.String);
  public static long parseUnsignedLong(java.lang.String, int);
  public static long decode(java.lang.String);
  public static java.lang.String toString(long);
  public static java.lang.String toString(long, int);
}
```
