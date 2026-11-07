# com.feilong.lib.lang3

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.lang3.AnnotationUtils`

```java
public class com.feilong.lib.lang3.AnnotationUtils {
  public com.feilong.lib.lang3.AnnotationUtils();
  public static java.lang.String toString(java.lang.annotation.Annotation);
}
```

## `com.feilong.lib.lang3.ArrayUtils`

```java
public class com.feilong.lib.lang3.ArrayUtils {
  public com.feilong.lib.lang3.ArrayUtils();
  public static boolean[] add(boolean[], boolean);
  public static byte[] add(byte[], byte);
  public static char[] add(char[], char);
  public static double[] add(double[], double);
  public static float[] add(float[], float);
  public static int[] add(int[], int);
  public static long[] add(long[], long);
  public static short[] add(short[], short);
  public static <T> T[] add(T[], T);
  public static boolean[] addAll(boolean[], boolean...);
  public static byte[] addAll(byte[], byte...);
  public static char[] addAll(char[], char...);
  public static double[] addAll(double[], double...);
  public static float[] addAll(float[], float...);
  public static int[] addAll(int[], int...);
  public static long[] addAll(long[], long...);
  public static short[] addAll(short[], short...);
  public static <T> T[] addAll(T[], T...);
  public static boolean[] addFirst(boolean[], boolean);
  public static byte[] addFirst(byte[], byte);
  public static char[] addFirst(char[], char);
  public static double[] addFirst(double[], double);
  public static float[] addFirst(float[], float);
  public static int[] addFirst(int[], int);
  public static long[] addFirst(long[], long);
  public static short[] addFirst(short[], short);
  public static <T> T[] addFirst(T[], T);
  public static boolean[] clone(boolean[]);
  public static byte[] clone(byte[]);
  public static char[] clone(char[]);
  public static double[] clone(double[]);
  public static float[] clone(float[]);
  public static int[] clone(int[]);
  public static long[] clone(long[]);
  public static short[] clone(short[]);
  public static <T> T[] clone(T[]);
  public static boolean contains(boolean[], boolean);
  public static boolean contains(byte[], byte);
  public static boolean contains(char[], char);
  public static boolean contains(double[], double);
  public static boolean contains(double[], double, double);
  public static boolean contains(float[], float);
  public static boolean contains(int[], int);
  public static boolean contains(long[], long);
  public static boolean contains(java.lang.Object[], java.lang.Object);
  public static boolean contains(short[], short);
  public static int getLength(java.lang.Object);
  public static java.util.BitSet indexesOf(boolean[], boolean);
  public static java.util.BitSet indexesOf(boolean[], boolean, int);
  public static java.util.BitSet indexesOf(byte[], byte);
  public static java.util.BitSet indexesOf(byte[], byte, int);
  public static java.util.BitSet indexesOf(char[], char);
  public static java.util.BitSet indexesOf(char[], char, int);
  public static java.util.BitSet indexesOf(double[], double);
  public static java.util.BitSet indexesOf(double[], double, double);
  public static java.util.BitSet indexesOf(double[], double, int);
  public static java.util.BitSet indexesOf(double[], double, int, double);
  public static java.util.BitSet indexesOf(float[], float);
  public static java.util.BitSet indexesOf(float[], float, int);
  public static java.util.BitSet indexesOf(int[], int);
  public static java.util.BitSet indexesOf(int[], int, int);
  public static java.util.BitSet indexesOf(long[], long);
  public static java.util.BitSet indexesOf(long[], long, int);
  public static java.util.BitSet indexesOf(java.lang.Object[], java.lang.Object);
  public static java.util.BitSet indexesOf(java.lang.Object[], java.lang.Object, int);
  public static java.util.BitSet indexesOf(short[], short);
  public static java.util.BitSet indexesOf(short[], short, int);
  public static int indexOf(boolean[], boolean);
  public static int indexOf(boolean[], boolean, int);
  public static int indexOf(byte[], byte);
  public static int indexOf(byte[], byte, int);
  public static int indexOf(char[], char);
  public static int indexOf(char[], char, int);
  public static int indexOf(double[], double);
  public static int indexOf(double[], double, double);
  public static int indexOf(double[], double, int);
  public static int indexOf(double[], double, int, double);
  public static int indexOf(float[], float);
  public static int indexOf(float[], float, int);
  public static int indexOf(int[], int);
  public static int indexOf(int[], int, int);
  public static int indexOf(long[], long);
  public static int indexOf(long[], long, int);
  public static int indexOf(java.lang.Object[], java.lang.Object);
  public static int indexOf(java.lang.Object[], java.lang.Object, int);
  public static int indexOf(short[], short);
  public static int indexOf(short[], short, int);
  public static boolean[] insert(int, boolean[], boolean...);
  public static byte[] insert(int, byte[], byte...);
  public static char[] insert(int, char[], char...);
  public static double[] insert(int, double[], double...);
  public static float[] insert(int, float[], float...);
  public static int[] insert(int, int[], int...);
  public static long[] insert(int, long[], long...);
  public static short[] insert(int, short[], short...);
  public static <T> T[] insert(int, T[], T...);
  public static <T> boolean isArrayIndexValid(T[], int);
  public static boolean isEmpty(boolean[]);
  public static boolean isEmpty(byte[]);
  public static boolean isEmpty(char[]);
  public static boolean isEmpty(double[]);
  public static boolean isEmpty(float[]);
  public static boolean isEmpty(int[]);
  public static boolean isEmpty(long[]);
  public static boolean isEmpty(java.lang.Object[]);
  public static boolean isEmpty(short[]);
  public static boolean isNotEmpty(boolean[]);
  public static boolean isNotEmpty(byte[]);
  public static boolean isNotEmpty(char[]);
  public static boolean isNotEmpty(double[]);
  public static boolean isNotEmpty(float[]);
  public static boolean isNotEmpty(int[]);
  public static boolean isNotEmpty(long[]);
  public static boolean isNotEmpty(short[]);
  public static <T> boolean isNotEmpty(T[]);
  public static boolean isSameLength(boolean[], boolean[]);
  public static boolean isSameLength(byte[], byte[]);
  public static boolean isSameLength(char[], char[]);
  public static boolean isSameLength(double[], double[]);
  public static boolean isSameLength(float[], float[]);
  public static boolean isSameLength(int[], int[]);
  public static boolean isSameLength(long[], long[]);
  public static boolean isSameLength(java.lang.Object[], java.lang.Object[]);
  public static boolean isSameLength(short[], short[]);
  public static boolean isSameType(java.lang.Object, java.lang.Object);
  public static boolean isSorted(boolean[]);
  public static boolean isSorted(double[]);
  public static boolean isSorted(float[]);
  public static boolean isSorted(int[]);
  public static boolean isSorted(long[]);
  public static boolean isSorted(short[]);
  public static <T extends java.lang.Comparable<? super T>> boolean isSorted(T[]);
  public static <T> boolean isSorted(T[], java.util.Comparator<T>);
  public static int lastIndexOf(boolean[], boolean);
  public static int lastIndexOf(boolean[], boolean, int);
  public static int lastIndexOf(byte[], byte);
  public static int lastIndexOf(byte[], byte, int);
  public static int lastIndexOf(char[], char);
  public static int lastIndexOf(char[], char, int);
  public static int lastIndexOf(double[], double);
  public static int lastIndexOf(double[], double, double);
  public static int lastIndexOf(double[], double, int);
  public static int lastIndexOf(double[], double, int, double);
  public static int lastIndexOf(float[], float);
  public static int lastIndexOf(float[], float, int);
  public static int lastIndexOf(int[], int);
  public static int lastIndexOf(int[], int, int);
  public static int lastIndexOf(long[], long);
  public static int lastIndexOf(long[], long, int);
  public static int lastIndexOf(java.lang.Object[], java.lang.Object);
  public static int lastIndexOf(java.lang.Object[], java.lang.Object, int);
  public static int lastIndexOf(short[], short);
  public static int lastIndexOf(short[], short, int);
  public static boolean[] nullToEmpty(boolean[]);
  public static java.lang.Boolean[] nullToEmpty(java.lang.Boolean[]);
  public static byte[] nullToEmpty(byte[]);
  public static java.lang.Byte[] nullToEmpty(java.lang.Byte[]);
  public static char[] nullToEmpty(char[]);
  public static java.lang.Character[] nullToEmpty(java.lang.Character[]);
  public static java.lang.Class<?>[] nullToEmpty(java.lang.Class<?>[]);
  public static double[] nullToEmpty(double[]);
  public static java.lang.Double[] nullToEmpty(java.lang.Double[]);
  public static float[] nullToEmpty(float[]);
  public static java.lang.Float[] nullToEmpty(java.lang.Float[]);
  public static int[] nullToEmpty(int[]);
  public static java.lang.Integer[] nullToEmpty(java.lang.Integer[]);
  public static long[] nullToEmpty(long[]);
  public static java.lang.Long[] nullToEmpty(java.lang.Long[]);
  public static java.lang.Object[] nullToEmpty(java.lang.Object[]);
  public static short[] nullToEmpty(short[]);
  public static java.lang.Short[] nullToEmpty(java.lang.Short[]);
  public static java.lang.String[] nullToEmpty(java.lang.String[]);
  public static <T> T[] nullToEmpty(T[], java.lang.Class<T[]>);
  public static boolean[] remove(boolean[], int);
  public static byte[] remove(byte[], int);
  public static char[] remove(char[], int);
  public static double[] remove(double[], int);
  public static float[] remove(float[], int);
  public static int[] remove(int[], int);
  public static long[] remove(long[], int);
  public static short[] remove(short[], int);
  public static <T> T[] remove(T[], int);
  public static boolean[] removeAll(boolean[], int...);
  public static byte[] removeAll(byte[], int...);
  public static char[] removeAll(char[], int...);
  public static double[] removeAll(double[], int...);
  public static float[] removeAll(float[], int...);
  public static int[] removeAll(int[], int...);
  public static long[] removeAll(long[], int...);
  public static short[] removeAll(short[], int...);
  public static <T> T[] removeAll(T[], int...);
  public static boolean[] removeElement(boolean[], boolean);
  public static byte[] removeElement(byte[], byte);
  public static char[] removeElement(char[], char);
  public static double[] removeElement(double[], double);
  public static float[] removeElement(float[], float);
  public static int[] removeElement(int[], int);
  public static long[] removeElement(long[], long);
  public static short[] removeElement(short[], short);
  public static <T> T[] removeElement(T[], java.lang.Object);
  public static void reverse(boolean[]);
  public static void reverse(boolean[], int, int);
  public static void reverse(byte[]);
  public static void reverse(byte[], int, int);
  public static void reverse(char[]);
  public static void reverse(char[], int, int);
  public static void reverse(double[]);
  public static void reverse(double[], int, int);
  public static void reverse(float[]);
  public static void reverse(float[], int, int);
  public static void reverse(int[]);
  public static void reverse(int[], int, int);
  public static void reverse(long[]);
  public static void reverse(long[], int, int);
  public static void shift(boolean[], int);
  public static void shift(boolean[], int, int, int);
  public static void shift(byte[], int);
  public static void shift(byte[], int, int, int);
  public static void shift(char[], int);
  public static void shift(char[], int, int, int);
  public static void shift(double[], int);
  public static void shift(double[], int, int, int);
  public static void shift(float[], int);
  public static void shift(float[], int, int, int);
  public static void shift(int[], int);
  public static void shift(int[], int, int, int);
  public static void shift(long[], int);
  public static void shift(long[], int, int, int);
  public static void shift(java.lang.Object[], int);
  public static void shift(java.lang.Object[], int, int, int);
  public static void shift(short[], int);
  public static void shift(short[], int, int, int);
  public static void shuffle(boolean[]);
  public static void shuffle(boolean[], java.util.Random);
  public static void shuffle(byte[]);
  public static void shuffle(byte[], java.util.Random);
  public static void shuffle(char[]);
  public static void shuffle(char[], java.util.Random);
  public static void shuffle(double[]);
  public static void shuffle(double[], java.util.Random);
  public static void shuffle(float[]);
  public static void shuffle(float[], java.util.Random);
  public static void shuffle(int[]);
  public static void shuffle(int[], java.util.Random);
  public static void shuffle(long[]);
  public static void shuffle(long[], java.util.Random);
  public static void shuffle(java.lang.Object[]);
  public static void shuffle(java.lang.Object[], java.util.Random);
  public static void shuffle(short[]);
  public static void shuffle(short[], java.util.Random);
  public static boolean[] subarray(boolean[], int, int);
  public static byte[] subarray(byte[], int, int);
  public static char[] subarray(char[], int, int);
  public static double[] subarray(double[], int, int);
  public static float[] subarray(float[], int, int);
  public static int[] subarray(int[], int, int);
  public static long[] subarray(long[], int, int);
  public static short[] subarray(short[], int, int);
  public static <T> T[] subarray(T[], int, int);
  public static void swap(boolean[], int, int);
  public static void swap(boolean[], int, int, int);
  public static void swap(byte[], int, int);
  public static void swap(byte[], int, int, int);
  public static void swap(char[], int, int);
  public static void swap(char[], int, int, int);
  public static void swap(double[], int, int);
  public static void swap(double[], int, int, int);
  public static void swap(float[], int, int);
  public static void swap(float[], int, int, int);
  public static void swap(int[], int, int);
  public static void swap(int[], int, int, int);
  public static void swap(long[], int, int);
  public static void swap(long[], int, int, int);
  public static void swap(java.lang.Object[], int, int);
  public static void swap(java.lang.Object[], int, int, int);
  public static void swap(short[], int, int);
  public static void swap(short[], int, int, int);
  public static <T> T[] toArray(T...);
  public static java.util.Map<java.lang.Object, java.lang.Object> toMap(java.lang.Object[]);
  public static java.lang.Boolean[] toObject(boolean[]);
  public static java.lang.Byte[] toObject(byte[]);
  public static java.lang.Character[] toObject(char[]);
  public static java.lang.Double[] toObject(double[]);
  public static java.lang.Float[] toObject(float[]);
  public static java.lang.Integer[] toObject(int[]);
  public static java.lang.Long[] toObject(long[]);
  public static java.lang.Short[] toObject(short[]);
  public static boolean[] toPrimitive(java.lang.Boolean[]);
  public static boolean[] toPrimitive(java.lang.Boolean[], boolean);
  public static byte[] toPrimitive(java.lang.Byte[]);
  public static byte[] toPrimitive(java.lang.Byte[], byte);
  public static char[] toPrimitive(java.lang.Character[]);
  public static char[] toPrimitive(java.lang.Character[], char);
  public static double[] toPrimitive(java.lang.Double[]);
  public static double[] toPrimitive(java.lang.Double[], double);
  public static float[] toPrimitive(java.lang.Float[]);
  public static float[] toPrimitive(java.lang.Float[], float);
  public static int[] toPrimitive(java.lang.Integer[]);
  public static int[] toPrimitive(java.lang.Integer[], int);
  public static long[] toPrimitive(java.lang.Long[]);
  public static long[] toPrimitive(java.lang.Long[], long);
  public static java.lang.Object toPrimitive(java.lang.Object);
  public static short[] toPrimitive(java.lang.Short[]);
  public static short[] toPrimitive(java.lang.Short[], short);
  public static java.lang.String toString(java.lang.Object);
  public static java.lang.String toString(java.lang.Object, java.lang.String);
  public static java.lang.String[] toStringArray(java.lang.Object[]);
  public static java.lang.String[] toStringArray(java.lang.Object[], java.lang.String);
}
```

## `com.feilong.lib.lang3.BooleanUtils`

```java
public class com.feilong.lib.lang3.BooleanUtils {
  public com.feilong.lib.lang3.BooleanUtils();
  public static java.lang.Boolean negate(java.lang.Boolean);
  public static boolean isTrue(java.lang.Boolean);
  public static boolean isNotTrue(java.lang.Boolean);
  public static boolean isFalse(java.lang.Boolean);
  public static boolean isNotFalse(java.lang.Boolean);
  public static boolean toBoolean(java.lang.Boolean);
  public static boolean toBooleanDefaultIfNull(java.lang.Boolean, boolean);
  public static boolean toBoolean(int);
  public static java.lang.Boolean toBooleanObject(int);
  public static java.lang.Boolean toBooleanObject(java.lang.Integer);
  public static boolean toBoolean(int, int, int);
  public static boolean toBoolean(java.lang.Integer, java.lang.Integer, java.lang.Integer);
  public static java.lang.Boolean toBooleanObject(int, int, int, int);
  public static java.lang.Boolean toBooleanObject(java.lang.Integer, java.lang.Integer, java.lang.Integer, java.lang.Integer);
  public static int toInteger(boolean);
  public static java.lang.Integer toIntegerObject(boolean);
  public static java.lang.Integer toIntegerObject(java.lang.Boolean);
  public static int toInteger(boolean, int, int);
  public static int toInteger(java.lang.Boolean, int, int, int);
  public static java.lang.Integer toIntegerObject(boolean, java.lang.Integer, java.lang.Integer);
  public static java.lang.Integer toIntegerObject(java.lang.Boolean, java.lang.Integer, java.lang.Integer, java.lang.Integer);
  public static java.lang.Boolean toBooleanObject(java.lang.String);
  public static java.lang.Boolean toBooleanObject(java.lang.String, java.lang.String, java.lang.String, java.lang.String);
  public static boolean toBoolean(java.lang.String);
  public static boolean toBoolean(java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String toStringTrueFalse(java.lang.Boolean);
  public static java.lang.String toStringOnOff(java.lang.Boolean);
  public static java.lang.String toStringYesNo(java.lang.Boolean);
  public static java.lang.String toString(java.lang.Boolean, java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String toStringTrueFalse(boolean);
  public static java.lang.String toStringOnOff(boolean);
  public static java.lang.String toStringYesNo(boolean);
  public static java.lang.String toString(boolean, java.lang.String, java.lang.String);
  public static boolean and(boolean...);
  public static java.lang.Boolean and(java.lang.Boolean...);
  public static boolean or(boolean...);
  public static java.lang.Boolean or(java.lang.Boolean...);
  public static boolean xor(boolean...);
  public static java.lang.Boolean xor(java.lang.Boolean...);
  public static int compare(boolean, boolean);
}
```

## `com.feilong.lib.lang3.CharSequenceUtils`

```java
public class com.feilong.lib.lang3.CharSequenceUtils {
  public com.feilong.lib.lang3.CharSequenceUtils();
  public static java.lang.CharSequence subSequence(java.lang.CharSequence, int);
}
```

## `com.feilong.lib.lang3.CharUtils`

```java
public class com.feilong.lib.lang3.CharUtils {
  public com.feilong.lib.lang3.CharUtils();
  public static java.lang.String toString(char);
  public static java.lang.String toString(java.lang.Character);
}
```

## `com.feilong.lib.lang3.ClassUtils`

```java
public class com.feilong.lib.lang3.ClassUtils {
  public com.feilong.lib.lang3.ClassUtils();
  public static java.lang.String getShortClassName(java.lang.Object, java.lang.String);
  public static java.lang.String getShortClassName(java.lang.Class<?>);
  public static java.lang.String getShortClassName(java.lang.String);
  public static java.lang.String getSimpleName(java.lang.Class<?>);
  public static java.lang.String getSimpleName(java.lang.Class<?>, java.lang.String);
  public static java.lang.String getSimpleName(java.lang.Object);
  public static java.lang.String getSimpleName(java.lang.Object, java.lang.String);
  public static java.lang.String getName(java.lang.Class<?>);
  public static java.lang.String getName(java.lang.Class<?>, java.lang.String);
  public static java.lang.String getName(java.lang.Object);
  public static java.lang.String getName(java.lang.Object, java.lang.String);
  public static java.lang.String getPackageName(java.lang.Object, java.lang.String);
  public static java.lang.String getPackageName(java.lang.Class<?>);
  public static java.lang.String getPackageName(java.lang.String);
  public static java.lang.String getAbbreviatedName(java.lang.Class<?>, int);
  public static java.lang.String getAbbreviatedName(java.lang.String, int);
  public static java.util.List<java.lang.Class<?>> getAllSuperclasses(java.lang.Class<?>);
  public static java.util.List<java.lang.Class<?>> getAllInterfaces(java.lang.Class<?>);
  public static java.util.List<java.lang.Class<?>> convertClassNamesToClasses(java.util.List<java.lang.String>);
  public static java.util.List<java.lang.String> convertClassesToClassNames(java.util.List<java.lang.Class<?>>);
  public static boolean isAssignable(java.lang.Class<?>[], java.lang.Class<?>...);
  public static boolean isAssignable(java.lang.Class<?>[], java.lang.Class<?>[], boolean);
  public static boolean isPrimitiveOrWrapper(java.lang.Class<?>);
  public static boolean isPrimitiveWrapper(java.lang.Class<?>);
  public static boolean isAssignable(java.lang.Class<?>, java.lang.Class<?>);
  public static boolean isAssignable(java.lang.Class<?>, java.lang.Class<?>, boolean);
  public static java.lang.Class<?> primitiveToWrapper(java.lang.Class<?>);
  public static java.lang.Class<?>[] primitivesToWrappers(java.lang.Class<?>...);
  public static java.lang.Class<?> wrapperToPrimitive(java.lang.Class<?>);
  public static java.lang.Class<?>[] wrappersToPrimitives(java.lang.Class<?>...);
  public static boolean isInnerClass(java.lang.Class<?>);
  public static java.lang.Class<?> getClass(java.lang.ClassLoader, java.lang.String, boolean) throws java.lang.ClassNotFoundException;
  public static java.lang.Class<?> getClass(java.lang.ClassLoader, java.lang.String) throws java.lang.ClassNotFoundException;
  public static java.lang.Class<?> getClass(java.lang.String) throws java.lang.ClassNotFoundException;
  public static java.lang.Class<?> getClass(java.lang.String, boolean) throws java.lang.ClassNotFoundException;
  public static java.lang.reflect.Method getPublicMethod(java.lang.Class<?>, java.lang.String, java.lang.Class<?>...) throws java.lang.NoSuchMethodException;
  public static java.lang.Class<?>[] toClass(java.lang.Object...);
  public static java.lang.String getShortCanonicalName(java.lang.Object, java.lang.String);
  public static java.lang.String getCanonicalName(java.lang.Class<?>);
  public static java.lang.String getCanonicalName(java.lang.Class<?>, java.lang.String);
  public static java.lang.String getCanonicalName(java.lang.Object);
  public static java.lang.String getCanonicalName(java.lang.Object, java.lang.String);
  public static java.lang.String getShortCanonicalName(java.lang.Class<?>);
  public static java.lang.String getShortCanonicalName(java.lang.String);
  public static java.lang.String getPackageCanonicalName(java.lang.Object, java.lang.String);
  public static java.lang.String getPackageCanonicalName(java.lang.Class<?>);
  public static java.lang.String getPackageCanonicalName(java.lang.String);
}
```

## `com.feilong.lib.lang3.EnumUtils`

```java
public class com.feilong.lib.lang3.EnumUtils {
  public com.feilong.lib.lang3.EnumUtils();
  public static <E extends java.lang.Enum<E>> E getEnum(java.lang.Class<E>, java.lang.String);
  public static <E extends java.lang.Enum<E>> E getEnum(java.lang.Class<E>, java.lang.String, E);
  public static <E extends java.lang.Enum<E>> E getEnumIgnoreCase(java.lang.Class<E>, java.lang.String);
  public static <E extends java.lang.Enum<E>> E getEnumIgnoreCase(java.lang.Class<E>, java.lang.String, E);
  public static <E extends java.lang.Enum<E>> java.util.List<E> getEnumList(java.lang.Class<E>);
  public static <E extends java.lang.Enum<E>> java.util.Map<java.lang.String, E> getEnumMap(java.lang.Class<E>);
}
```

## `com.feilong.lib.lang3.LocaleUtils`

```java
public class com.feilong.lib.lang3.LocaleUtils {
  public com.feilong.lib.lang3.LocaleUtils();
  public static java.util.Locale toLocale(java.lang.String);
}
```

## `com.feilong.lib.lang3.NotImplementedException`

```java
public class com.feilong.lib.lang3.NotImplementedException extends java.lang.UnsupportedOperationException {
  public com.feilong.lib.lang3.NotImplementedException(java.lang.String);
  public com.feilong.lib.lang3.NotImplementedException(java.lang.String, java.lang.String);
  public java.lang.String getCode();
}
```

## `com.feilong.lib.lang3.ObjectUtils`

```java
public class com.feilong.lib.lang3.ObjectUtils {
  public com.feilong.lib.lang3.ObjectUtils();
  public static <T> T firstNonNull(T...);
  public static <T> T getFirstNonNull(java.util.function.Supplier<T>...);
  public static <T> T getIfNull(T, java.util.function.Supplier<T>);
  public static boolean anyNotNull(java.lang.Object...);
  public static boolean allNotNull(java.lang.Object...);
  public static <T extends java.lang.Comparable<? super T>> int compare(T, T);
  public static <T extends java.lang.Comparable<? super T>> int compare(T, T, boolean);
  public static <T> T clone(T);
  public static <T> T cloneIfPossible(T);
}
```

## `com.feilong.lib.lang3.RandomStringUtils`

```java
public class com.feilong.lib.lang3.RandomStringUtils {
  public com.feilong.lib.lang3.RandomStringUtils();
  public static java.lang.String random(int, int, int, boolean, boolean, char[], java.util.Random);
  public static java.lang.String random(int, java.lang.String);
  public static java.lang.String random(int, char...);
}
```

## `com.feilong.lib.lang3.SerializationUtils`

```java
public class com.feilong.lib.lang3.SerializationUtils {
  public com.feilong.lib.lang3.SerializationUtils();
  public static <T extends java.io.Serializable> T clone(T);
  public static void serialize(java.io.Serializable, java.io.OutputStream);
  public static byte[] serialize(java.io.Serializable);
  public static <T> T deserialize(java.io.InputStream);
  public static <T> T deserialize(byte[]);
}
```

## `com.feilong.lib.lang3.StringUtils`

```java
public class com.feilong.lib.lang3.StringUtils {
  public static java.lang.String abbreviate(java.lang.String, int);
  public static java.lang.String abbreviate(java.lang.String, java.lang.String, int);
  public static java.lang.String abbreviate(java.lang.String, java.lang.String, int, int);
  public static java.lang.String abbreviateMiddle(java.lang.String, java.lang.String, int);
  public static java.lang.String capitalize(java.lang.String);
  public static java.lang.String center(java.lang.String, int);
  public static java.lang.String center(java.lang.String, int, char);
  public static java.lang.String center(java.lang.String, int, java.lang.String);
  public static java.lang.String chomp(java.lang.String);
  public static java.lang.String chop(java.lang.String);
  public static int compare(java.lang.String, java.lang.String);
  public static int compare(java.lang.String, java.lang.String, boolean);
  public static int compareIgnoreCase(java.lang.String, java.lang.String);
  public static int compareIgnoreCase(java.lang.String, java.lang.String, boolean);
  public static boolean contains(java.lang.CharSequence, java.lang.CharSequence);
  public static boolean contains(java.lang.CharSequence, int);
  public static boolean containsAny(java.lang.CharSequence, char...);
  public static boolean containsAny(java.lang.CharSequence, java.lang.CharSequence);
  public static boolean containsAny(java.lang.CharSequence, java.lang.CharSequence...);
  public static boolean containsIgnoreCase(java.lang.CharSequence, java.lang.CharSequence);
  public static boolean containsNone(java.lang.CharSequence, char...);
  public static boolean containsNone(java.lang.CharSequence, java.lang.String);
  public static boolean containsWhitespace(java.lang.CharSequence);
  public static int countMatches(java.lang.CharSequence, char);
  public static int countMatches(java.lang.CharSequence, java.lang.CharSequence);
  public static <T extends java.lang.CharSequence> T defaultIfBlank(T, T);
  public static <T extends java.lang.CharSequence> T defaultIfEmpty(T, T);
  public static java.lang.String defaultString(java.lang.String);
  public static java.lang.String defaultString(java.lang.String, java.lang.String);
  public static java.lang.String deleteWhitespace(java.lang.String);
  public static boolean endsWith(java.lang.CharSequence, java.lang.CharSequence);
  public static boolean endsWithAny(java.lang.CharSequence, java.lang.CharSequence...);
  public static boolean endsWithIgnoreCase(java.lang.CharSequence, java.lang.CharSequence);
  public static boolean equals(java.lang.CharSequence, java.lang.CharSequence);
  public static boolean equalsAny(java.lang.CharSequence, java.lang.CharSequence...);
  public static boolean equalsAnyIgnoreCase(java.lang.CharSequence, java.lang.CharSequence...);
  public static boolean equalsIgnoreCase(java.lang.CharSequence, java.lang.CharSequence);
  public static byte[] getBytes(java.lang.String, java.nio.charset.Charset);
  public static byte[] getBytes(java.lang.String, java.lang.String) throws java.io.UnsupportedEncodingException;
  public static java.lang.String getCommonPrefix(java.lang.String...);
  public static java.lang.String getDigits(java.lang.String);
  public static <T extends java.lang.CharSequence> T getIfBlank(T, java.util.function.Supplier<T>);
  public static <T extends java.lang.CharSequence> T getIfEmpty(T, java.util.function.Supplier<T>);
  public static int indexOf(java.lang.CharSequence, java.lang.CharSequence);
  public static int indexOf(java.lang.CharSequence, java.lang.CharSequence, int);
  public static int indexOf(java.lang.CharSequence, int);
  public static int indexOf(java.lang.CharSequence, int, int);
  public static int indexOfAny(java.lang.CharSequence, char...);
  public static int indexOfAnyBut(java.lang.CharSequence, java.lang.CharSequence);
  public static int indexOfDifference(java.lang.CharSequence...);
  public static int indexOfDifference(java.lang.CharSequence, java.lang.CharSequence);
  public static int indexOfIgnoreCase(java.lang.CharSequence, java.lang.CharSequence);
  public static int indexOfIgnoreCase(java.lang.CharSequence, java.lang.CharSequence, int);
  public static boolean isAllBlank(java.lang.CharSequence...);
  public static boolean isAllEmpty(java.lang.CharSequence...);
  public static boolean isAllLowerCase(java.lang.CharSequence);
  public static boolean isAllUpperCase(java.lang.CharSequence);
  public static boolean isAlpha(java.lang.CharSequence);
  public static boolean isAlphanumeric(java.lang.CharSequence);
  public static boolean isAlphanumericSpace(java.lang.CharSequence);
  public static boolean isAlphaSpace(java.lang.CharSequence);
  public static boolean isAnyBlank(java.lang.CharSequence...);
  public static boolean isAnyEmpty(java.lang.CharSequence...);
  public static boolean isBlank(java.lang.CharSequence);
  public static boolean isEmpty(java.lang.CharSequence);
  public static boolean isNoneBlank(java.lang.CharSequence...);
  public static boolean isNoneEmpty(java.lang.CharSequence...);
  public static boolean isNotBlank(java.lang.CharSequence);
  public static boolean isNotEmpty(java.lang.CharSequence);
  public static boolean isNumeric(java.lang.CharSequence);
  public static boolean isNumericSpace(java.lang.CharSequence);
  public static boolean isWhitespace(java.lang.CharSequence);
  public static java.lang.String join(byte[], char, int, int);
  public static java.lang.String join(char[], char, int, int);
  public static java.lang.String join(double[], char);
  public static java.lang.String join(double[], char, int, int);
  public static java.lang.String join(java.lang.Iterable<?>, char);
  public static java.lang.String join(java.lang.Iterable<?>, java.lang.String);
  public static java.lang.String join(java.util.Iterator<?>, char);
  public static java.lang.String join(java.util.Iterator<?>, java.lang.String);
  public static java.lang.String join(java.util.List<?>, char, int, int);
  public static java.lang.String join(java.util.List<?>, java.lang.String, int, int);
  public static java.lang.String join(java.lang.Object[], char);
  public static java.lang.String join(java.lang.Object[], char, int, int);
  public static java.lang.String join(java.lang.Object[], java.lang.String);
  public static java.lang.String join(java.lang.Object[], java.lang.String, int, int);
  public static <T> java.lang.String join(T...);
  public static java.lang.String joinWith(java.lang.String, java.lang.Object...);
  public static int lastIndexOf(java.lang.CharSequence, java.lang.CharSequence);
  public static int lastIndexOf(java.lang.CharSequence, java.lang.CharSequence, int);
  public static int lastIndexOf(java.lang.CharSequence, int);
  public static int lastIndexOf(java.lang.CharSequence, int, int);
  public static int lastIndexOfAny(java.lang.CharSequence, java.lang.CharSequence...);
  public static int lastIndexOfIgnoreCase(java.lang.CharSequence, java.lang.CharSequence);
  public static int lastIndexOfIgnoreCase(java.lang.CharSequence, java.lang.CharSequence, int);
  public static int lastOrdinalIndexOf(java.lang.CharSequence, java.lang.CharSequence, int);
  public static java.lang.String left(java.lang.String, int);
  public static java.lang.String leftPad(java.lang.String, int);
  public static java.lang.String leftPad(java.lang.String, int, char);
  public static java.lang.String leftPad(java.lang.String, int, java.lang.String);
  public static int length(java.lang.CharSequence);
  public static java.lang.String lowerCase(java.lang.String);
  public static java.lang.String lowerCase(java.lang.String, java.util.Locale);
  public static java.lang.String mid(java.lang.String, int, int);
  public static java.lang.String normalizeSpace(java.lang.String);
  public static int ordinalIndexOf(java.lang.CharSequence, java.lang.CharSequence, int);
  public static java.lang.String prependIfMissing(java.lang.String, java.lang.CharSequence, java.lang.CharSequence...);
  public static java.lang.String prependIfMissingIgnoreCase(java.lang.String, java.lang.CharSequence, java.lang.CharSequence...);
  public static java.lang.String remove(java.lang.String, char);
  public static java.lang.String remove(java.lang.String, java.lang.String);
  public static java.lang.String removeEnd(java.lang.String, java.lang.String);
  public static java.lang.String removeEndIgnoreCase(java.lang.String, java.lang.String);
  public static java.lang.String removeIgnoreCase(java.lang.String, java.lang.String);
  public static java.lang.String removeStart(java.lang.String, java.lang.String);
  public static java.lang.String removeStartIgnoreCase(java.lang.String, java.lang.String);
  public static java.lang.String repeat(char, int);
  public static java.lang.String repeat(java.lang.String, int);
  public static java.lang.String replace(java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String replace(java.lang.String, java.lang.String, java.lang.String, int);
  public static java.lang.String replaceChars(java.lang.String, char, char);
  public static java.lang.String replaceChars(java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String replaceEach(java.lang.String, java.lang.String[], java.lang.String[]);
  public static java.lang.String replaceEachRepeatedly(java.lang.String, java.lang.String[], java.lang.String[]);
  public static java.lang.String replaceIgnoreCase(java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String replaceIgnoreCase(java.lang.String, java.lang.String, java.lang.String, int);
  public static java.lang.String replaceOnce(java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String replaceOnceIgnoreCase(java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String reverse(java.lang.String);
  public static java.lang.String right(java.lang.String, int);
  public static java.lang.String rightPad(java.lang.String, int);
  public static java.lang.String rightPad(java.lang.String, int, char);
  public static java.lang.String rightPad(java.lang.String, int, java.lang.String);
  public static java.lang.String[] split(java.lang.String);
  public static java.lang.String[] split(java.lang.String, char);
  public static java.lang.String[] split(java.lang.String, java.lang.String);
  public static java.lang.String[] split(java.lang.String, java.lang.String, int);
  public static java.lang.String[] splitByCharacterType(java.lang.String);
  public static java.lang.String[] splitByCharacterTypeCamelCase(java.lang.String);
  public static java.lang.String[] splitByWholeSeparator(java.lang.String, java.lang.String);
  public static java.lang.String[] splitByWholeSeparator(java.lang.String, java.lang.String, int);
  public static java.lang.String[] splitByWholeSeparatorPreserveAllTokens(java.lang.String, java.lang.String);
  public static java.lang.String[] splitByWholeSeparatorPreserveAllTokens(java.lang.String, java.lang.String, int);
  public static java.lang.String[] splitPreserveAllTokens(java.lang.String);
  public static java.lang.String[] splitPreserveAllTokens(java.lang.String, char);
  public static java.lang.String[] splitPreserveAllTokens(java.lang.String, java.lang.String);
  public static java.lang.String[] splitPreserveAllTokens(java.lang.String, java.lang.String, int);
  public static boolean startsWith(java.lang.CharSequence, java.lang.CharSequence);
  public static boolean startsWithAny(java.lang.CharSequence, java.lang.CharSequence...);
  public static boolean startsWithIgnoreCase(java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String strip(java.lang.String);
  public static java.lang.String strip(java.lang.String, java.lang.String);
  public static java.lang.String stripAccents(java.lang.String);
  public static java.lang.String[] stripAll(java.lang.String...);
  public static java.lang.String[] stripAll(java.lang.String[], java.lang.String);
  public static java.lang.String stripEnd(java.lang.String, java.lang.String);
  public static java.lang.String stripStart(java.lang.String, java.lang.String);
  public static java.lang.String stripToEmpty(java.lang.String);
  public static java.lang.String stripToNull(java.lang.String);
  public static java.lang.String substring(java.lang.String, int);
  public static java.lang.String substring(java.lang.String, int, int);
  public static java.lang.String substringAfter(java.lang.String, java.lang.String);
  public static java.lang.String substringAfterLast(java.lang.String, java.lang.String);
  public static java.lang.String substringBefore(java.lang.String, java.lang.String);
  public static java.lang.String substringBeforeLast(java.lang.String, java.lang.String);
  public static java.lang.String substringBetween(java.lang.String, java.lang.String);
  public static java.lang.String substringBetween(java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String[] substringsBetween(java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String swapCase(java.lang.String);
  public static java.lang.String toEncodedString(byte[], java.nio.charset.Charset);
  public static java.lang.String toString(byte[], java.lang.String) throws java.io.UnsupportedEncodingException;
  public static java.lang.String trim(java.lang.String);
  public static java.lang.String trimToEmpty(java.lang.String);
  public static java.lang.String trimToNull(java.lang.String);
  public static java.lang.String uncapitalize(java.lang.String);
  public static java.lang.String unwrap(java.lang.String, char);
  public static java.lang.String unwrap(java.lang.String, java.lang.String);
  public static java.lang.String upperCase(java.lang.String);
  public static java.lang.String upperCase(java.lang.String, java.util.Locale);
  public static java.lang.String valueOf(char[]);
  public static java.lang.String wrap(java.lang.String, char);
  public static java.lang.String wrap(java.lang.String, java.lang.String);
  public static java.lang.String wrapIfMissing(java.lang.String, char);
  public static java.lang.String wrapIfMissing(java.lang.String, java.lang.String);
  public com.feilong.lib.lang3.StringUtils();
}
```

## `com.feilong.lib.lang3.Validate`

```java
public class com.feilong.lib.lang3.Validate {
  public com.feilong.lib.lang3.Validate();
  public static void isTrue(boolean, java.lang.String, java.lang.Object...);
  public static <T> T notNull(T, java.lang.String, java.lang.Object...);
}
```
