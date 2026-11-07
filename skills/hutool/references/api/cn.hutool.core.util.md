# cn.hutool.core.util

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.util.ArrayUtil`

```java
public class cn.hutool.core.util.ArrayUtil extends cn.hutool.core.util.PrimitiveArrayUtil {
  public cn.hutool.core.util.ArrayUtil();
  public static <T> boolean isEmpty(T[]);
  public static <T> T[] defaultIfEmpty(T[], T[]);
  public static boolean isEmpty(java.lang.Object);
  public static <T> boolean isNotEmpty(T[]);
  public static boolean isNotEmpty(java.lang.Object);
  public static <T> boolean hasNull(T...);
  public static <T> boolean isAllNull(T...);
  public static <T> T firstNonNull(T...);
  public static <T> T firstMatch(cn.hutool.core.lang.Matcher<T>, T...);
  public static <T> int matchIndex(cn.hutool.core.lang.Matcher<T>, T...);
  public static <T> int matchIndex(cn.hutool.core.lang.Matcher<T>, int, T...);
  public static <T> T[] newArray(java.lang.Class<?>, int);
  public static java.lang.Object[] newArray(int);
  public static java.lang.Class<?> getComponentType(java.lang.Object);
  public static java.lang.Class<?> getComponentType(java.lang.Class<?>);
  public static java.lang.Class<?> getArrayType(java.lang.Class<?>);
  public static java.lang.Object[] cast(java.lang.Class<?>, java.lang.Object) throws java.lang.NullPointerException, java.lang.IllegalArgumentException;
  public static <T> T[] append(T[], T...);
  public static <T> java.lang.Object append(java.lang.Object, T...);
  public static <T> T[] setOrAppend(T[], int, T);
  public static java.lang.Object setOrAppend(java.lang.Object, int, java.lang.Object);
  public static <T> T[] replace(T[], int, T...);
  public static <T> T[] insert(T[], int, T...);
  public static <T> java.lang.Object insert(java.lang.Object, int, T...);
  public static <T> T[] resize(T[], int, java.lang.Class<?>);
  public static java.lang.Object resize(java.lang.Object, int);
  public static <T> T[] resize(T[], int);
  public static <T> T[] addAll(T[]...);
  public static java.lang.Object copy(java.lang.Object, int, java.lang.Object, int, int);
  public static java.lang.Object copy(java.lang.Object, java.lang.Object, int);
  public static <T> T[] clone(T[]);
  public static <T> T clone(T);
  public static <T> T[] edit(T[], cn.hutool.core.lang.Editor<T>);
  public static <T> T[] filter(T[], cn.hutool.core.lang.Filter<T>);
  public static <T> T[] removeNull(T[]);
  public static <T extends java.lang.CharSequence> T[] removeEmpty(T[]);
  public static <T extends java.lang.CharSequence> T[] removeBlank(T[]);
  public static java.lang.String[] nullToEmpty(java.lang.String[]);
  public static <K, V> java.util.Map<K, V> zip(K[], V[], boolean);
  public static <K, V> java.util.Map<K, V> zip(K[], V[]);
  public static <T> int indexOf(T[], java.lang.Object, int);
  public static <T> int indexOf(T[], java.lang.Object);
  public static int indexOfIgnoreCase(java.lang.CharSequence[], java.lang.CharSequence);
  public static <T> int lastIndexOf(T[], java.lang.Object);
  public static <T> int lastIndexOf(T[], java.lang.Object, int);
  public static <T> boolean contains(T[], T);
  public static <T> boolean containsAny(T[], T...);
  public static <T> boolean containsAll(T[], T...);
  public static boolean containsIgnoreCase(java.lang.CharSequence[], java.lang.CharSequence);
  public static java.lang.Object[] wrap(java.lang.Object);
  public static boolean isArray(java.lang.Object);
  public static <T> T get(java.lang.Object, int);
  public static <T> T[] getAny(java.lang.Object, int...);
  public static <T> T[] sub(T[], int, int);
  public static java.lang.Object[] sub(java.lang.Object, int, int);
  public static java.lang.Object[] sub(java.lang.Object, int, int, int);
  public static java.lang.String toString(java.lang.Object);
  public static int length(java.lang.Object) throws java.lang.IllegalArgumentException;
  public static <T> java.lang.String join(T[], java.lang.CharSequence);
  public static <T> java.lang.String join(T[], java.lang.CharSequence, java.lang.String, java.lang.String);
  public static <T> java.lang.String join(T[], java.lang.CharSequence, cn.hutool.core.lang.Editor<T>);
  public static java.lang.String join(java.lang.Object, java.lang.CharSequence);
  public static byte[] toArray(java.nio.ByteBuffer);
  public static <T> T[] toArray(java.util.Iterator<T>, java.lang.Class<T>);
  public static <T> T[] toArray(java.lang.Iterable<T>, java.lang.Class<T>);
  public static <T> T[] toArray(java.util.Collection<T>, java.lang.Class<T>);
  public static <T> T[] remove(T[], int) throws java.lang.IllegalArgumentException;
  public static <T> T[] removeEle(T[], T) throws java.lang.IllegalArgumentException;
  public static <T> T[] reverse(T[], int, int);
  public static <T> T[] reverse(T[]);
  public static <T extends java.lang.Comparable<? super T>> T min(T[]);
  public static <T extends java.lang.Comparable<? super T>> T min(T[], java.util.Comparator<T>);
  public static <T extends java.lang.Comparable<? super T>> T max(T[]);
  public static <T extends java.lang.Comparable<? super T>> T max(T[], java.util.Comparator<T>);
  public static <T> T[] shuffle(T[]);
  public static <T> T[] shuffle(T[], java.util.Random);
  public static <T> T[] swap(T[], int, int);
  public static java.lang.Object swap(java.lang.Object, int, int);
  public static int emptyCount(java.lang.Object...);
  public static boolean hasEmpty(java.lang.Object...);
  public static boolean isAllEmpty(java.lang.Object...);
  public static boolean isAllNotEmpty(java.lang.Object...);
  public static <T> boolean isAllNotNull(T...);
  public static <T> T[] distinct(T[]);
  public static <T, K> T[] distinct(T[], java.util.function.Function<T, K>, boolean);
  public static <T, R> R[] map(T[], java.lang.Class<R>, java.util.function.Function<? super T, ? extends R>);
  public static <T, R> R[] map(java.lang.Object, java.lang.Class<R>, java.util.function.Function<? super T, ? extends R>);
  public static <T, R> java.util.List<R> map(T[], java.util.function.Function<? super T, ? extends R>);
  public static <T, R> java.util.Set<R> mapToSet(T[], java.util.function.Function<? super T, ? extends R>);
  public static boolean equals(java.lang.Object, java.lang.Object);
  public static <T> boolean isSub(T[], T[]);
  public static <T> int indexOfSub(T[], T[]);
  public static <T> int indexOfSub(T[], int, T[]);
  public static <T> int lastIndexOfSub(T[], T[]);
  public static <T> int lastIndexOfSub(T[], int, T[]);
  public static <T> boolean isSorted(T[], java.util.Comparator<? super T>);
  public static <T extends java.lang.Comparable<? super T>> boolean isSorted(T[]);
  public static <T extends java.lang.Comparable<? super T>> boolean isSortedASC(T[]);
  public static <T extends java.lang.Comparable<? super T>> boolean isSortedDESC(T[]);
}
```

## `cn.hutool.core.util.BooleanUtil`

```java
public class cn.hutool.core.util.BooleanUtil {
  public cn.hutool.core.util.BooleanUtil();
  public static java.lang.Boolean negate(java.lang.Boolean);
  public static boolean isTrue(java.lang.Boolean);
  public static boolean isFalse(java.lang.Boolean);
  public static boolean negate(boolean);
  public static boolean toBoolean(java.lang.String);
  public static java.lang.Boolean toBooleanObject(java.lang.String);
  public static int toInt(boolean);
  public static java.lang.Integer toInteger(boolean);
  public static char toChar(boolean);
  public static java.lang.Character toCharacter(boolean);
  public static byte toByte(boolean);
  public static java.lang.Byte toByteObj(boolean);
  public static long toLong(boolean);
  public static java.lang.Long toLongObj(boolean);
  public static short toShort(boolean);
  public static java.lang.Short toShortObj(boolean);
  public static float toFloat(boolean);
  public static java.lang.Float toFloatObj(boolean);
  public static double toDouble(boolean);
  public static java.lang.Double toDoubleObj(boolean);
  public static java.lang.String toStringTrueFalse(boolean);
  public static java.lang.String toStringOnOff(boolean);
  public static java.lang.String toStringYesNo(boolean);
  public static java.lang.String toString(boolean, java.lang.String, java.lang.String);
  public static java.lang.String toString(java.lang.Boolean, java.lang.String, java.lang.String, java.lang.String);
  public static boolean and(boolean...);
  public static java.lang.Boolean andOfWrap(java.lang.Boolean...);
  public static boolean or(boolean...);
  public static java.lang.Boolean orOfWrap(java.lang.Boolean...);
  public static boolean xor(boolean...);
  public static boolean exactlyOneTrue(boolean...);
  public static java.lang.Boolean xorOfWrap(java.lang.Boolean...);
  public static boolean isBoolean(java.lang.Class<?>);
}
```

## `cn.hutool.core.util.ByteUtil`

```java
public class cn.hutool.core.util.ByteUtil {
  public cn.hutool.core.util.ByteUtil();
  public static byte intToByte(int);
  public static int byteToUnsignedInt(byte);
  public static short bytesToShort(byte[]);
  public static short bytesToShort(byte[], java.nio.ByteOrder);
  public static short bytesToShort(byte[], int, java.nio.ByteOrder);
  public static byte[] shortToBytes(short);
  public static byte[] shortToBytes(short, java.nio.ByteOrder);
  public static int bytesToInt(byte[]);
  public static int bytesToInt(byte[], java.nio.ByteOrder);
  public static int bytesToInt(byte[], int, java.nio.ByteOrder);
  public static byte[] intToBytes(int);
  public static byte[] intToBytes(int, java.nio.ByteOrder);
  public static byte[] longToBytes(long);
  public static byte[] longToBytes(long, java.nio.ByteOrder);
  public static long bytesToLong(byte[]);
  public static long bytesToLong(byte[], java.nio.ByteOrder);
  public static long bytesToLong(byte[], int, java.nio.ByteOrder);
  public static byte[] floatToBytes(float);
  public static byte[] floatToBytes(float, java.nio.ByteOrder);
  public static float bytesToFloat(byte[]);
  public static float bytesToFloat(byte[], java.nio.ByteOrder);
  public static byte[] doubleToBytes(double);
  public static byte[] doubleToBytes(double, java.nio.ByteOrder);
  public static double bytesToDouble(byte[]);
  public static double bytesToDouble(byte[], java.nio.ByteOrder);
  public static byte[] numberToBytes(java.lang.Number);
  public static byte[] numberToBytes(java.lang.Number, java.nio.ByteOrder);
  public static <T extends java.lang.Number> T bytesToNumber(byte[], java.lang.Class<T>, java.nio.ByteOrder) throws java.lang.IllegalArgumentException;
}
```

## `cn.hutool.core.util.CharUtil`

```java
public class cn.hutool.core.util.CharUtil implements cn.hutool.core.text.CharPool {
  public cn.hutool.core.util.CharUtil();
  public static boolean isAscii(char);
  public static boolean isAsciiPrintable(char);
  public static boolean isAsciiControl(char);
  public static boolean isLetter(char);
  public static boolean isLetterUpper(char);
  public static boolean isLetterLower(char);
  public static boolean isNumber(char);
  public static boolean isHexChar(char);
  public static boolean isLetterOrNumber(char);
  public static java.lang.String toString(char);
  public static boolean isCharClass(java.lang.Class<?>);
  public static boolean isChar(java.lang.Object);
  public static boolean isBlankChar(char);
  public static boolean isBlankChar(int);
  public static boolean isEmoji(char);
  public static boolean isFileSeparator(char);
  public static boolean equals(char, char, boolean);
  public static int getType(int);
  public static int digit16(int);
  public static char toCloseChar(char);
  public static char toCloseByNumber(int);
}
```

## `cn.hutool.core.util.CharsetUtil`

```java
public class cn.hutool.core.util.CharsetUtil {
  public cn.hutool.core.util.CharsetUtil();
  public static java.nio.charset.Charset charset(java.lang.String) throws java.nio.charset.UnsupportedCharsetException;
  public static java.nio.charset.Charset parse(java.lang.String);
  public static java.nio.charset.Charset parse(java.lang.String, java.nio.charset.Charset);
  public static java.lang.String convert(java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String convert(java.lang.String, java.nio.charset.Charset, java.nio.charset.Charset);
  public static java.io.File convert(java.io.File, java.nio.charset.Charset, java.nio.charset.Charset);
  public static java.lang.String systemCharsetName();
  public static java.nio.charset.Charset systemCharset();
  public static java.lang.String defaultCharsetName();
  public static java.nio.charset.Charset defaultCharset();
  public static java.nio.charset.Charset defaultCharset(java.io.InputStream, java.nio.charset.Charset...);
  public static java.nio.charset.Charset defaultCharset(int, java.io.InputStream, java.nio.charset.Charset...);
}
```

## `cn.hutool.core.util.ClassLoaderUtil`

```java
public class cn.hutool.core.util.ClassLoaderUtil {
  public cn.hutool.core.util.ClassLoaderUtil();
  public static java.lang.ClassLoader getContextClassLoader();
  public static java.lang.ClassLoader getSystemClassLoader();
  public static java.lang.ClassLoader getClassLoader();
  public static java.lang.Class<?> loadClass(java.lang.String) throws cn.hutool.core.exceptions.UtilException;
  public static java.lang.Class<?> loadClass(java.lang.String, boolean) throws cn.hutool.core.exceptions.UtilException;
  public static java.lang.Class<?> loadClass(java.lang.String, java.lang.ClassLoader, boolean) throws cn.hutool.core.exceptions.UtilException;
  public static java.lang.Class<?> loadPrimitiveClass(java.lang.String);
  public static cn.hutool.core.lang.JarClassLoader getJarClassLoader(java.io.File);
  public static java.lang.Class<?> loadClass(java.io.File, java.lang.String);
  public static boolean isPresent(java.lang.String);
  public static boolean isPresent(java.lang.String, java.lang.ClassLoader);
}
```

## `cn.hutool.core.util.ClassUtil`

```java
public class cn.hutool.core.util.ClassUtil {
  public cn.hutool.core.util.ClassUtil();
  public static <T> java.lang.Class<T> getClass(T);
  public static java.lang.Class<?> getEnclosingClass(java.lang.Class<?>);
  public static boolean isTopLevelClass(java.lang.Class<?>);
  public static java.lang.String getClassName(java.lang.Object, boolean);
  public static java.lang.String getClassName(java.lang.Class<?>, boolean);
  public static java.lang.String getShortClassName(java.lang.String);
  public static java.lang.Class<?>[] getClasses(java.lang.Object...);
  public static boolean equals(java.lang.Class<?>, java.lang.String, boolean);
  public static java.util.Set<java.lang.Class<?>> scanPackageByAnnotation(java.lang.String, java.lang.Class<? extends java.lang.annotation.Annotation>);
  public static java.util.Set<java.lang.Class<?>> scanPackageBySuper(java.lang.String, java.lang.Class<?>);
  public static java.util.Set<java.lang.Class<?>> scanPackage();
  public static java.util.Set<java.lang.Class<?>> scanPackage(java.lang.String);
  public static java.util.Set<java.lang.Class<?>> scanPackage(java.lang.String, cn.hutool.core.lang.Filter<java.lang.Class<?>>);
  public static java.util.Set<java.lang.String> getPublicMethodNames(java.lang.Class<?>);
  public static java.lang.reflect.Method[] getPublicMethods(java.lang.Class<?>);
  public static java.util.List<java.lang.reflect.Method> getPublicMethods(java.lang.Class<?>, cn.hutool.core.lang.Filter<java.lang.reflect.Method>);
  public static java.util.List<java.lang.reflect.Method> getPublicMethods(java.lang.Class<?>, java.lang.reflect.Method...);
  public static java.util.List<java.lang.reflect.Method> getPublicMethods(java.lang.Class<?>, java.lang.String...);
  public static java.lang.reflect.Method getPublicMethod(java.lang.Class<?>, java.lang.String, java.lang.Class<?>...) throws java.lang.SecurityException;
  public static java.util.Set<java.lang.String> getDeclaredMethodNames(java.lang.Class<?>);
  public static java.lang.reflect.Method[] getDeclaredMethods(java.lang.Class<?>);
  public static java.lang.reflect.Method getDeclaredMethodOfObj(java.lang.Object, java.lang.String, java.lang.Object...) throws java.lang.SecurityException;
  public static java.lang.reflect.Method getDeclaredMethod(java.lang.Class<?>, java.lang.String, java.lang.Class<?>...) throws java.lang.SecurityException;
  public static java.lang.reflect.Field getDeclaredField(java.lang.Class<?>, java.lang.String) throws java.lang.SecurityException;
  public static java.lang.reflect.Field[] getDeclaredFields(java.lang.Class<?>) throws java.lang.SecurityException;
  public static java.util.Set<java.lang.String> getClassPathResources();
  public static java.util.Set<java.lang.String> getClassPathResources(boolean);
  public static java.util.Set<java.lang.String> getClassPaths(java.lang.String);
  public static java.util.Set<java.lang.String> getClassPaths(java.lang.String, boolean);
  public static java.lang.String getClassPath();
  public static java.lang.String getClassPath(boolean);
  public static java.net.URL getClassPathURL();
  public static java.net.URL getResourceURL(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.util.List<java.net.URL> getResources(java.lang.String);
  public static java.net.URL getResourceUrl(java.lang.String, java.lang.Class<?>);
  public static java.lang.String[] getJavaClassPaths();
  public static java.lang.ClassLoader getContextClassLoader();
  public static java.lang.ClassLoader getClassLoader();
  public static boolean isAllAssignableFrom(java.lang.Class<?>[], java.lang.Class<?>[]);
  public static <T> java.lang.Class<T> loadClass(java.lang.String, boolean);
  public static <T> java.lang.Class<T> loadClass(java.lang.String);
  public static <T> T invoke(java.lang.String, java.lang.Object[]);
  public static <T> T invoke(java.lang.String, boolean, java.lang.Object...);
  public static <T> T invoke(java.lang.String, java.lang.String, java.lang.Object[]);
  public static <T> T invoke(java.lang.String, java.lang.String, boolean, java.lang.Object...);
  public static boolean isPrimitiveWrapper(java.lang.Class<?>);
  public static boolean isBasicType(java.lang.Class<?>);
  public static boolean isSimpleTypeOrArray(java.lang.Class<?>);
  public static boolean isSimpleValueType(java.lang.Class<?>);
  public static boolean isAssignable(java.lang.Class<?>, java.lang.Class<?>);
  public static boolean isPublic(java.lang.Class<?>);
  public static boolean isPublic(java.lang.reflect.Method);
  public static boolean isNotPublic(java.lang.Class<?>);
  public static boolean isNotPublic(java.lang.reflect.Method);
  public static boolean isStatic(java.lang.reflect.Method);
  public static java.lang.reflect.Method setAccessible(java.lang.reflect.Method);
  public static boolean isAbstract(java.lang.Class<?>);
  public static boolean isNormalClass(java.lang.Class<?>);
  public static boolean isEnum(java.lang.Class<?>);
  public static java.lang.Class<?> getTypeArgument(java.lang.Class<?>);
  public static java.lang.Class<?> getTypeArgument(java.lang.Class<?>, int);
  public static java.lang.String getPackage(java.lang.Class<?>);
  public static java.lang.String getPackagePath(java.lang.Class<?>);
  public static java.lang.Object getDefaultValue(java.lang.Class<?>);
  public static java.lang.Object getPrimitiveDefaultValue(java.lang.Class<?>);
  public static java.lang.Object[] getDefaultValues(java.lang.Class<?>...);
  public static boolean isJdkClass(java.lang.Class<?>);
  public static java.net.URL getLocation(java.lang.Class<?>);
  public static java.lang.String getLocationPath(java.lang.Class<?>);
  public static boolean isAbstractOrInterface(java.lang.Class<?>);
  public static boolean isInterface(java.lang.Class<?>);
}
```

## `cn.hutool.core.util.CoordinateUtil`

```java
public class cn.hutool.core.util.CoordinateUtil {
  public cn.hutool.core.util.CoordinateUtil();
  public static boolean outOfChina(double, double);
  public static cn.hutool.core.util.CoordinateUtil$Coordinate wgs84ToGcj02(double, double);
  public static cn.hutool.core.util.CoordinateUtil$Coordinate wgs84ToBd09(double, double);
  public static cn.hutool.core.util.CoordinateUtil$Coordinate gcj02ToWgs84(double, double);
  public static cn.hutool.core.util.CoordinateUtil$Coordinate gcj02ToBd09(double, double);
  public static cn.hutool.core.util.CoordinateUtil$Coordinate bd09ToGcj02(double, double);
  public static cn.hutool.core.util.CoordinateUtil$Coordinate bd09toWgs84(double, double);
  public static cn.hutool.core.util.CoordinateUtil$Coordinate wgs84ToMercator(double, double);
  public static cn.hutool.core.util.CoordinateUtil$Coordinate mercatorToWgs84(double, double);
}
```

## `cn.hutool.core.util.CoordinateUtil$Coordinate`

```java
public class cn.hutool.core.util.CoordinateUtil$Coordinate implements java.io.Serializable {
  public cn.hutool.core.util.CoordinateUtil$Coordinate(double, double);
  public double getLng();
  public cn.hutool.core.util.CoordinateUtil$Coordinate setLng(double);
  public double getLat();
  public cn.hutool.core.util.CoordinateUtil$Coordinate setLat(double);
  public cn.hutool.core.util.CoordinateUtil$Coordinate offset(cn.hutool.core.util.CoordinateUtil$Coordinate);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `cn.hutool.core.util.CreditCodeUtil`

```java
public class cn.hutool.core.util.CreditCodeUtil {
  public cn.hutool.core.util.CreditCodeUtil();
  public static boolean isCreditCodeSimple(java.lang.CharSequence);
  public static boolean isCreditCode(java.lang.CharSequence);
  public static java.lang.String randomCreditCode();
}
```

## `cn.hutool.core.util.DesensitizedUtil`

```java
public class cn.hutool.core.util.DesensitizedUtil {
  public cn.hutool.core.util.DesensitizedUtil();
  public static java.lang.String desensitized(java.lang.CharSequence, cn.hutool.core.util.DesensitizedUtil$DesensitizedType);
  public static java.lang.String clear();
  public static java.lang.String clearToNull();
  public static java.lang.Long userId();
  public static java.lang.String firstMask(java.lang.String);
  public static java.lang.String chineseName(java.lang.String);
  public static java.lang.String idCardNum(java.lang.String, int, int);
  public static java.lang.String fixedPhone(java.lang.String);
  public static java.lang.String mobilePhone(java.lang.String);
  public static java.lang.String address(java.lang.String, int);
  public static java.lang.String email(java.lang.String);
  public static java.lang.String password(java.lang.String);
  public static java.lang.String carLicense(java.lang.String);
  public static java.lang.String bankCard(java.lang.String);
  public static java.lang.String ipv4(java.lang.String);
  public static java.lang.String ipv6(java.lang.String);
  public static java.lang.String passport(java.lang.String);
  public static java.lang.String creditCode(java.lang.String);
}
```

## `cn.hutool.core.util.DesensitizedUtil$DesensitizedType`

```java
public final class cn.hutool.core.util.DesensitizedUtil$DesensitizedType extends java.lang.Enum<cn.hutool.core.util.DesensitizedUtil$DesensitizedType> {
  public static cn.hutool.core.util.DesensitizedUtil$DesensitizedType[] values();
  public static cn.hutool.core.util.DesensitizedUtil$DesensitizedType valueOf(java.lang.String);
}
```

## `cn.hutool.core.util.EnumUtil`

```java
public class cn.hutool.core.util.EnumUtil {
  public cn.hutool.core.util.EnumUtil();
  public static void clearCache();
  public static boolean isEnum(java.lang.Class<?>);
  public static boolean isEnum(java.lang.Object);
  public static java.lang.String toString(java.lang.Enum<?>);
  public static <E extends java.lang.Enum<E>> E getEnumAt(java.lang.Class<E>, int);
  public static <E extends java.lang.Enum<E>> E fromString(java.lang.Class<E>, java.lang.String);
  public static <E extends java.lang.Enum<E>> E fromString(java.lang.Class<E>, java.lang.String, E);
  public static <E extends java.lang.Enum<E>> E fromStringQuietly(java.lang.Class<E>, java.lang.String);
  public static <E extends java.lang.Enum<E>> E likeValueOf(java.lang.Class<E>, java.lang.Object);
  public static java.util.List<java.lang.String> getNames(java.lang.Class<? extends java.lang.Enum<?>>);
  public static java.util.List<java.lang.Object> getFieldValues(java.lang.Class<? extends java.lang.Enum<?>>, java.lang.String);
  public static java.util.List<java.lang.String> getFieldNames(java.lang.Class<? extends java.lang.Enum<?>>);
  public static <E extends java.lang.Enum<E>> E getBy(java.lang.Class<E>, java.util.function.Predicate<? super E>);
  public static <E extends java.lang.Enum<E>> E getBy(java.lang.Class<E>, java.util.function.Predicate<? super E>, E);
  public static <E extends java.lang.Enum<E>, C> E getBy(java.lang.Class<E>, cn.hutool.core.lang.func.Func1<E, C>, C);
  public static <E extends java.lang.Enum<E>, C> E getBy(java.lang.Class<E>, cn.hutool.core.lang.func.Func1<E, C>, C, E);
  public static <E extends java.lang.Enum<E>, C> E getBy(cn.hutool.core.lang.func.Func1<E, C>, C);
  public static <E extends java.lang.Enum<E>, C> E getBy(cn.hutool.core.lang.func.Func1<E, C>, C, E);
  public static <E extends java.lang.Enum<E>, F, C> F getFieldBy(cn.hutool.core.lang.func.Func1<E, F>, java.util.function.Function<E, C>, C);
  public static <E extends java.lang.Enum<E>> java.util.LinkedHashMap<java.lang.String, E> getEnumMap(java.lang.Class<E>);
  public static java.util.Map<java.lang.String, java.lang.Object> getNameFieldMap(java.lang.Class<? extends java.lang.Enum<?>>, java.lang.String);
  public static <E extends java.lang.Enum<E>> boolean contains(java.lang.Class<E>, java.lang.String);
  public static <E extends java.lang.Enum<E>> boolean notContains(java.lang.Class<E>, java.lang.String);
  public static boolean equalsIgnoreCase(java.lang.Enum<?>, java.lang.String);
  public static boolean equals(java.lang.Enum<?>, java.lang.String);
}
```

## `cn.hutool.core.util.EscapeUtil`

```java
public class cn.hutool.core.util.EscapeUtil {
  public cn.hutool.core.util.EscapeUtil();
  public static java.lang.String escapeXml(java.lang.CharSequence);
  public static java.lang.String unescapeXml(java.lang.CharSequence);
  public static java.lang.String escapeHtml4(java.lang.CharSequence);
  public static java.lang.String unescapeHtml4(java.lang.CharSequence);
  public static java.lang.String escape(java.lang.CharSequence);
  public static java.lang.String escapeAll(java.lang.CharSequence);
  public static java.lang.String escape(java.lang.CharSequence, cn.hutool.core.lang.Filter<java.lang.Character>);
  public static java.lang.String unescape(java.lang.String);
  public static java.lang.String safeUnescape(java.lang.String);
}
```

## `cn.hutool.core.util.HashUtil`

```java
public class cn.hutool.core.util.HashUtil {
  public cn.hutool.core.util.HashUtil();
  public static int additiveHash(java.lang.String, int);
  public static int rotatingHash(java.lang.String, int);
  public static int oneByOneHash(java.lang.String);
  public static int bernstein(java.lang.String);
  public static int universal(char[], int, int[]);
  public static int zobrist(char[], int, int[][]);
  public static int fnvHash(byte[]);
  public static int fnvHash(java.lang.String);
  public static int intHash(int);
  public static int rsHash(java.lang.String);
  public static int jsHash(java.lang.String);
  public static int pjwHash(java.lang.String);
  public static int elfHash(java.lang.String);
  public static int bkdrHash(java.lang.String);
  public static int sdbmHash(java.lang.String);
  public static int djbHash(java.lang.String);
  public static int dekHash(java.lang.String);
  public static int apHash(java.lang.String);
  public static long tianlHash(java.lang.String);
  public static int javaDefaultHash(java.lang.String);
  public static long mixHash(java.lang.String);
  public static int identityHashCode(java.lang.Object);
  public static int murmur32(byte[]);
  public static long murmur64(byte[]);
  public static long[] murmur128(byte[]);
  public static int cityHash32(byte[]);
  public static long cityHash64(byte[], long);
  public static long cityHash64(byte[], long, long);
  public static long cityHash64(byte[]);
  public static long[] cityHash128(byte[]);
  public static long[] cityHash128(byte[], cn.hutool.core.lang.hash.Number128);
  public static long metroHash64(byte[], long);
  public static long metroHash64(byte[]);
  public static long[] metroHash128(byte[], long);
  public static long[] metroHash128(byte[]);
  public static long hfHash(java.lang.String);
  public static long hfIpHash(java.lang.String);
}
```

## `cn.hutool.core.util.HexUtil`

```java
public class cn.hutool.core.util.HexUtil {
  public cn.hutool.core.util.HexUtil();
  public static boolean isHexNumber(java.lang.String);
  public static char[] encodeHex(byte[]);
  public static char[] encodeHex(java.lang.String, java.nio.charset.Charset);
  public static char[] encodeHex(byte[], boolean);
  public static java.lang.String encodeHexStr(byte[]);
  public static java.lang.String encodeHexStr(java.lang.String, java.nio.charset.Charset);
  public static java.lang.String encodeHexStr(java.lang.String);
  public static java.lang.String encodeHexStr(byte[], boolean);
  public static java.lang.String decodeHexStr(java.lang.String);
  public static java.lang.String decodeHexStr(java.lang.String, java.nio.charset.Charset);
  public static java.lang.String decodeHexStr(char[], java.nio.charset.Charset);
  public static byte[] decodeHex(java.lang.String);
  public static byte[] decodeHex(char[]);
  public static byte[] decodeHex(java.lang.CharSequence);
  public static java.lang.String encodeColor(java.awt.Color);
  public static java.lang.String encodeColor(java.awt.Color, java.lang.String);
  public static java.awt.Color decodeColor(java.lang.String);
  public static java.lang.String toUnicodeHex(int);
  public static java.lang.String toUnicodeHex(char);
  public static java.lang.String toHex(int);
  public static int hexToInt(java.lang.String);
  public static java.lang.String toHex(long);
  public static long hexToLong(java.lang.String);
  public static java.lang.String toHex(float);
  public static float hexToFloat(java.lang.String);
  public static java.lang.String toHex(double);
  public static double hexToDouble(java.lang.String);
  public static void appendHex(java.lang.StringBuilder, byte, boolean);
  public static java.math.BigInteger toBigInteger(java.lang.String);
  public static java.lang.String format(java.lang.String);
  public static java.lang.String format(java.lang.String, java.lang.String);
}
```

## `cn.hutool.core.util.IdUtil`

```java
public class cn.hutool.core.util.IdUtil {
  public cn.hutool.core.util.IdUtil();
  public static java.lang.String randomUUID();
  public static java.lang.String simpleUUID();
  public static java.lang.String fastUUID();
  public static java.lang.String fastSimpleUUID();
  public static java.lang.String objectId();
  public static cn.hutool.core.lang.Snowflake createSnowflake(long, long);
  public static cn.hutool.core.lang.Snowflake getSnowflake(long, long);
  public static cn.hutool.core.lang.Snowflake getSnowflake(long);
  public static cn.hutool.core.lang.Snowflake getSnowflake();
  public static long getDataCenterId(long);
  public static long getWorkerId(long, long);
  public static java.lang.String nanoId();
  public static java.lang.String nanoId(int);
  public static long getSnowflakeNextId();
  public static java.lang.String getSnowflakeNextIdStr();
}
```

## `cn.hutool.core.util.IdcardUtil`

```java
public class cn.hutool.core.util.IdcardUtil {
  public cn.hutool.core.util.IdcardUtil();
  public static java.lang.String convert15To18(java.lang.String);
  public static java.lang.String convert18To15(java.lang.String);
  public static boolean isValidCard(java.lang.String);
  public static boolean isValidCard18(java.lang.String);
  public static boolean isValidCard18(java.lang.String, boolean);
  public static boolean isValidCard15(java.lang.String);
  public static java.lang.String[] isValidCard10(java.lang.String);
  public static boolean isValidTWCard(java.lang.String);
  public static boolean isValidHKCard(java.lang.String);
  public static java.lang.String getBirthByIdCard(java.lang.String);
  public static java.lang.String getBirth(java.lang.String);
  public static cn.hutool.core.date.DateTime getBirthDate(java.lang.String);
  public static int getAgeByIdCard(java.lang.String);
  public static int getAgeByIdCard(java.lang.String, java.util.Date);
  public static java.lang.Short getYearByIdCard(java.lang.String);
  public static java.lang.Short getMonthByIdCard(java.lang.String);
  public static java.lang.Short getDayByIdCard(java.lang.String);
  public static int getGenderByIdCard(java.lang.String);
  public static java.lang.String getProvinceCodeByIdCard(java.lang.String);
  public static java.lang.String getProvinceByIdCard(java.lang.String);
  public static java.lang.String getCityCodeByIdCard(java.lang.String);
  public static java.lang.String getDistrictCodeByIdCard(java.lang.String);
  public static java.lang.String hide(java.lang.String, int, int);
  public static cn.hutool.core.util.IdcardUtil$Idcard getIdcardInfo(java.lang.String);
}
```

## `cn.hutool.core.util.IdcardUtil$Idcard`

```java
public class cn.hutool.core.util.IdcardUtil$Idcard implements java.io.Serializable {
  public cn.hutool.core.util.IdcardUtil$Idcard(java.lang.String);
  public java.lang.String getProvinceCode();
  public java.lang.String getProvince();
  public java.lang.String getCityCode();
  public cn.hutool.core.date.DateTime getBirthDate();
  public java.lang.Integer getGender();
  public int getAge();
  public java.lang.String toString();
}
```

## `cn.hutool.core.util.JAXBUtil`

```java
public class cn.hutool.core.util.JAXBUtil {
  public cn.hutool.core.util.JAXBUtil();
  public static java.lang.String beanToXml(java.lang.Object);
  public static java.lang.String beanToXml(java.lang.Object, java.nio.charset.Charset, boolean);
  public static <T> T xmlToBean(java.lang.String, java.lang.Class<T>);
  public static <T> T xmlToBean(java.io.File, java.nio.charset.Charset, java.lang.Class<T>);
  public static <T> T xmlToBean(java.io.Reader, java.lang.Class<T>);
}
```

## `cn.hutool.core.util.JNDIUtil`

```java
public class cn.hutool.core.util.JNDIUtil {
  public cn.hutool.core.util.JNDIUtil();
  public static javax.naming.directory.InitialDirContext createInitialDirContext(java.util.Map<java.lang.String, java.lang.String>);
  public static javax.naming.InitialContext createInitialContext(java.util.Map<java.lang.String, java.lang.String>);
  public static javax.naming.directory.Attributes getAttributes(java.lang.String, java.lang.String...);
}
```

## `cn.hutool.core.util.JdkUtil`

```java
public class cn.hutool.core.util.JdkUtil {
  public cn.hutool.core.util.JdkUtil();
}
```

## `cn.hutool.core.util.ModifierUtil`

```java
public class cn.hutool.core.util.ModifierUtil {
  public cn.hutool.core.util.ModifierUtil();
  public static boolean hasModifier(java.lang.Class<?>, cn.hutool.core.util.ModifierUtil$ModifierType...);
  public static boolean hasModifier(java.lang.reflect.Constructor<?>, cn.hutool.core.util.ModifierUtil$ModifierType...);
  public static boolean hasModifier(java.lang.reflect.Method, cn.hutool.core.util.ModifierUtil$ModifierType...);
  public static boolean hasModifier(java.lang.reflect.Field, cn.hutool.core.util.ModifierUtil$ModifierType...);
  public static boolean hasAllModifiers(java.lang.Class<?>, cn.hutool.core.util.ModifierUtil$ModifierType...);
  public static boolean hasAllModifiers(java.lang.reflect.Member, cn.hutool.core.util.ModifierUtil$ModifierType...);
  public static boolean isPublic(java.lang.reflect.Field);
  public static boolean isPublic(java.lang.reflect.Method);
  public static boolean isPublic(java.lang.Class<?>);
  public static boolean isPublic(java.lang.reflect.Constructor<?>);
  public static boolean isStatic(java.lang.reflect.Field);
  public static boolean isStatic(java.lang.reflect.Method);
  public static boolean isStatic(java.lang.Class<?>);
  public static boolean isSynthetic(java.lang.reflect.Field);
  public static boolean isSynthetic(java.lang.reflect.Method);
  public static boolean isSynthetic(java.lang.Class<?>);
  public static boolean isAbstract(java.lang.reflect.Method);
  public static void removeFinalModify(java.lang.reflect.Field);
}
```

## `cn.hutool.core.util.ModifierUtil$ModifierType`

```java
public final class cn.hutool.core.util.ModifierUtil$ModifierType extends java.lang.Enum<cn.hutool.core.util.ModifierUtil$ModifierType> {
  public static cn.hutool.core.util.ModifierUtil$ModifierType[] values();
  public static cn.hutool.core.util.ModifierUtil$ModifierType valueOf(java.lang.String);
  public int getValue();
}
```

## `cn.hutool.core.util.NumberUtil`

```java
public class cn.hutool.core.util.NumberUtil {
  public cn.hutool.core.util.NumberUtil();
  public static double add(float, float);
  public static double add(float, double);
  public static double add(double, float);
  public static double add(double, double);
  public static double add(long, double);
  public static double add(double, long);
  public static double add(long, long);
  public static double add(java.lang.Double, java.lang.Double);
  public static java.math.BigDecimal add(java.lang.Number, java.lang.Number);
  public static java.math.BigDecimal add(java.lang.Number...);
  public static java.math.BigDecimal add(java.lang.String...);
  public static java.math.BigDecimal add(java.math.BigDecimal...);
  public static double sub(float, float);
  public static double sub(float, double);
  public static double sub(double, float);
  public static double sub(double, double);
  public static double sub(java.lang.Double, java.lang.Double);
  public static java.math.BigDecimal sub(java.lang.Number, java.lang.Number);
  public static java.math.BigDecimal sub(java.lang.Number...);
  public static java.math.BigDecimal sub(java.lang.String...);
  public static java.math.BigDecimal sub(java.math.BigDecimal...);
  public static double mul(float, float);
  public static double mul(float, double);
  public static double mul(double, float);
  public static double mul(double, double);
  public static double mul(java.lang.Double, java.lang.Double);
  public static java.math.BigDecimal mul(java.lang.Number, java.lang.Number);
  public static java.math.BigDecimal mul(java.lang.Number...);
  public static java.math.BigDecimal mul(java.lang.String, java.lang.String);
  public static java.math.BigDecimal mul(java.lang.String...);
  public static java.math.BigDecimal mul(java.math.BigDecimal...);
  public static double div(float, float);
  public static double div(float, double);
  public static double div(double, float);
  public static double div(double, double);
  public static double div(java.lang.Double, java.lang.Double);
  public static java.math.BigDecimal div(java.lang.Number, java.lang.Number);
  public static java.math.BigDecimal div(java.lang.String, java.lang.String);
  public static double div(float, float, int);
  public static double div(float, double, int);
  public static double div(double, float, int);
  public static double div(double, double, int);
  public static double div(java.lang.Double, java.lang.Double, int);
  public static java.math.BigDecimal div(java.lang.Number, java.lang.Number, int);
  public static java.math.BigDecimal div(java.lang.String, java.lang.String, int);
  public static double div(float, float, int, java.math.RoundingMode);
  public static double div(float, double, int, java.math.RoundingMode);
  public static double div(double, float, int, java.math.RoundingMode);
  public static double div(double, double, int, java.math.RoundingMode);
  public static double div(java.lang.Double, java.lang.Double, int, java.math.RoundingMode);
  public static java.math.BigDecimal div(java.lang.Number, java.lang.Number, int, java.math.RoundingMode);
  public static java.math.BigDecimal div(java.lang.String, java.lang.String, int, java.math.RoundingMode);
  public static java.math.BigDecimal div(java.math.BigDecimal, java.math.BigDecimal, int, java.math.RoundingMode);
  public static int ceilDiv(int, int);
  public static java.math.BigDecimal round(double, int);
  public static java.lang.String roundStr(double, int);
  public static java.math.BigDecimal round(java.lang.String, int);
  public static java.math.BigDecimal round(java.math.BigDecimal, int);
  public static java.lang.String roundStr(java.lang.String, int);
  public static java.math.BigDecimal round(double, int, java.math.RoundingMode);
  public static java.lang.String roundStr(double, int, java.math.RoundingMode);
  public static java.math.BigDecimal round(java.lang.String, int, java.math.RoundingMode);
  public static java.math.BigDecimal round(java.math.BigDecimal, int, java.math.RoundingMode);
  public static java.lang.String roundStr(java.lang.String, int, java.math.RoundingMode);
  public static java.math.BigDecimal roundHalfEven(java.lang.Number, int);
  public static java.math.BigDecimal roundHalfEven(java.math.BigDecimal, int);
  public static java.math.BigDecimal roundDown(java.lang.Number, int);
  public static java.math.BigDecimal roundDown(java.math.BigDecimal, int);
  public static java.lang.String decimalFormat(java.lang.String, double);
  public static java.lang.String decimalFormat(java.lang.String, long);
  public static java.lang.String decimalFormat(java.lang.String, java.lang.Object);
  public static java.lang.String decimalFormat(java.lang.String, java.lang.Object, java.math.RoundingMode);
  public static java.lang.String decimalFormatMoney(double);
  public static java.lang.String formatPercent(double, int);
  public static boolean isNumber(java.lang.CharSequence);
  public static boolean isInteger(java.lang.String);
  public static boolean isLong(java.lang.String);
  public static boolean isDouble(java.lang.String);
  public static boolean isPrimes(int);
  public static int[] generateRandomNumber(int, int, int);
  public static int[] generateRandomNumber(int, int, int, int[]);
  public static java.lang.Integer[] generateBySet(int, int, int);
  public static int[] range(int);
  public static int[] range(int, int);
  public static int[] range(int, int, int);
  public static java.util.Collection<java.lang.Integer> appendRange(int, int, java.util.Collection<java.lang.Integer>);
  public static java.util.Collection<java.lang.Integer> appendRange(int, int, int, java.util.Collection<java.lang.Integer>);
  public static java.math.BigInteger factorial(java.math.BigInteger);
  public static java.math.BigInteger factorial(java.math.BigInteger, java.math.BigInteger);
  public static long factorial(long, long);
  public static long factorial(long);
  public static long sqrt(long);
  public static int processMultiple(int, int);
  public static int divisor(int, int);
  public static int multiple(int, int);
  public static java.lang.String getBinaryStr(java.lang.Number);
  public static int binaryToInt(java.lang.String);
  public static long binaryToLong(java.lang.String);
  public static int compare(char, char);
  public static int compare(double, double);
  public static int compare(int, int);
  public static int compare(long, long);
  public static int compare(short, short);
  public static int compare(byte, byte);
  public static boolean isGreater(java.math.BigDecimal, java.math.BigDecimal);
  public static boolean isGreaterOrEqual(java.math.BigDecimal, java.math.BigDecimal);
  public static boolean isLess(java.math.BigDecimal, java.math.BigDecimal);
  public static boolean isLessOrEqual(java.math.BigDecimal, java.math.BigDecimal);
  public static boolean isIn(java.math.BigDecimal, java.math.BigDecimal, java.math.BigDecimal);
  public static boolean equals(double, double);
  public static boolean equals(float, float);
  public static boolean equals(long, long);
  public static boolean equals(java.lang.Number, java.lang.Number);
  public static boolean equals(java.math.BigDecimal, java.math.BigDecimal);
  public static boolean equals(char, char, boolean);
  public static <T extends java.lang.Comparable<? super T>> T min(T[]);
  public static long min(long...);
  public static int min(int...);
  public static short min(short...);
  public static double min(double...);
  public static float min(float...);
  public static java.math.BigDecimal min(java.math.BigDecimal...);
  public static <T extends java.lang.Comparable<? super T>> T max(T[]);
  public static long max(long...);
  public static int max(int...);
  public static short max(short...);
  public static double max(double...);
  public static float max(float...);
  public static java.math.BigDecimal max(java.math.BigDecimal...);
  public static java.lang.String toStr(java.lang.Number, java.lang.String);
  public static java.lang.String toStr(java.lang.Number);
  public static java.lang.String toStr(java.lang.Number, boolean);
  public static java.lang.String toStr(java.math.BigDecimal);
  public static java.lang.String toStr(java.math.BigDecimal, boolean);
  public static java.math.BigDecimal toBigDecimal(java.lang.Number);
  public static java.math.BigDecimal toBigDecimal(java.lang.String);
  public static java.math.BigInteger toBigInteger(java.lang.Number);
  public static java.math.BigInteger toBigInteger(java.lang.String);
  public static int count(int, int);
  public static java.math.BigDecimal null2Zero(java.math.BigDecimal);
  public static int zero2One(int);
  public static int nullToZero(java.lang.Integer);
  public static long nullToZero(java.lang.Long);
  public static double nullToZero(java.lang.Double);
  public static float nullToZero(java.lang.Float);
  public static short nullToZero(java.lang.Short);
  public static byte nullToZero(java.lang.Byte);
  public static java.math.BigDecimal nullToZero(java.math.BigDecimal);
  public static java.math.BigInteger nullToZero(java.math.BigInteger);
  public static java.math.BigInteger newBigInteger(java.lang.String);
  public static boolean isBeside(long, long);
  public static boolean isBeside(int, int);
  public static int partValue(int, int);
  public static int partValue(int, int, boolean);
  public static java.math.BigDecimal pow(java.lang.Number, int);
  public static java.math.BigDecimal pow(java.math.BigDecimal, int);
  public static java.math.BigDecimal pow(java.math.BigDecimal, int, int, java.math.RoundingMode);
  public static boolean isPowerOfTwo(long);
  public static int parseInt(java.lang.String) throws java.lang.NumberFormatException;
  public static long parseLong(java.lang.String);
  public static float parseFloat(java.lang.String);
  public static double parseDouble(java.lang.String);
  public static java.lang.Number parseNumber(java.lang.String) throws java.lang.NumberFormatException;
  public static java.lang.Integer parseInt(java.lang.String, java.lang.Integer);
  public static java.lang.Long parseLong(java.lang.String, java.lang.Long);
  public static java.lang.Float parseFloat(java.lang.String, java.lang.Float);
  public static java.lang.Double parseDouble(java.lang.String, java.lang.Double);
  public static java.lang.Number parseNumber(java.lang.String, java.lang.Number);
  public static byte[] toBytes(int);
  public static int toInt(byte[]);
  public static byte[] toUnsignedByteArray(java.math.BigInteger);
  public static byte[] toUnsignedByteArray(int, java.math.BigInteger);
  public static java.math.BigInteger fromUnsignedByteArray(byte[]);
  public static java.math.BigInteger fromUnsignedByteArray(byte[], int, int);
  public static boolean isValidNumber(java.lang.Number);
  public static boolean isValid(double);
  public static boolean isValid(float);
  public static double calculate(java.lang.String);
  public static double toDouble(java.lang.Number);
  public static boolean isOdd(int);
  public static boolean isEven(int);
}
```

## `cn.hutool.core.util.ObjUtil`

```java
public class cn.hutool.core.util.ObjUtil extends cn.hutool.core.util.ObjectUtil {
  public cn.hutool.core.util.ObjUtil();
}
```

## `cn.hutool.core.util.ObjectUtil`

```java
public class cn.hutool.core.util.ObjectUtil {
  public cn.hutool.core.util.ObjectUtil();
  public static boolean equals(java.lang.Object, java.lang.Object);
  public static boolean equal(java.lang.Object, java.lang.Object);
  public static boolean notEqual(java.lang.Object, java.lang.Object);
  public static int length(java.lang.Object);
  public static boolean contains(java.lang.Object, java.lang.Object);
  public static boolean isNull(java.lang.Object);
  public static boolean isNotNull(java.lang.Object);
  public static boolean isEmpty(java.lang.Object);
  public static boolean isNotEmpty(java.lang.Object);
  public static <T> T defaultIfNull(T, T);
  public static <T> T defaultIfNull(T, java.util.function.Supplier<? extends T>);
  public static <T> T defaultIfNull(T, java.util.function.Function<T, ? extends T>);
  public static <T> T defaultIfNull(java.lang.Object, java.util.function.Supplier<? extends T>, T);
  public static <T, R> T defaultIfNull(R, java.util.function.Function<R, ? extends T>, T);
  public static <T, R> R apply(T, java.util.function.Function<T, R>);
  public static <T> void accept(T, java.util.function.Consumer<T>);
  public static <T> T defaultIfEmpty(java.lang.String, java.util.function.Supplier<? extends T>, T);
  public static <T> T defaultIfEmpty(java.lang.String, java.util.function.Function<java.lang.CharSequence, ? extends T>, T);
  public static <T extends java.lang.CharSequence> T defaultIfEmpty(T, T);
  public static <T extends java.lang.CharSequence> T defaultIfEmpty(T, java.util.function.Supplier<? extends T>);
  public static <T extends java.lang.CharSequence> T defaultIfEmpty(T, java.util.function.Function<T, ? extends T>);
  public static <T extends java.lang.CharSequence> T defaultIfBlank(T, T);
  public static <T extends java.lang.CharSequence> T defaultIfBlank(T, java.util.function.Supplier<? extends T>);
  public static <T extends java.lang.CharSequence> T defaultIfBlank(T, java.util.function.Function<T, ? extends T>);
  public static <T> T clone(T);
  public static <T> T cloneIfPossible(T);
  public static <T> T cloneByStream(T);
  public static <T> byte[] serialize(T);
  public static <T> T deserialize(byte[], java.lang.Class<?>...);
  public static boolean isBasicType(java.lang.Object);
  public static boolean isValidIfNumber(java.lang.Object);
  public static <T extends java.lang.Comparable<? super T>> int compare(T, T);
  public static <T extends java.lang.Comparable<? super T>> int compare(T, T, boolean);
  public static java.lang.Class<?> getTypeArgument(java.lang.Object);
  public static java.lang.Class<?> getTypeArgument(java.lang.Object, int);
  public static java.lang.String toString(java.lang.Object);
  public static int emptyCount(java.lang.Object...);
  public static boolean hasNull(java.lang.Object...);
  public static boolean hasEmpty(java.lang.Object...);
  public static boolean isAllEmpty(java.lang.Object...);
  public static boolean isAllNotEmpty(java.lang.Object...);
}
```

## `cn.hutool.core.util.PageUtil`

```java
public class cn.hutool.core.util.PageUtil {
  public cn.hutool.core.util.PageUtil();
  public static int getFirstPageNo();
  public static synchronized void setFirstPageNo(int);
  public static void setOneAsFirstPageNo();
  public static int getStart(int, int);
  public static int getEnd(int, int);
  public static int[] transToStartEnd(int, int);
  public static cn.hutool.core.lang.Segment<java.lang.Integer> toSegment(int, int);
  public static int totalPage(int, int);
  public static int totalPage(long, int);
  public static int[] rainbow(int, int, int);
  public static int[] rainbow(int, int);
}
```

## `cn.hutool.core.util.PhoneUtil`

```java
public class cn.hutool.core.util.PhoneUtil {
  public cn.hutool.core.util.PhoneUtil();
  public static boolean isMobile(java.lang.CharSequence);
  public static boolean isMobileHk(java.lang.CharSequence);
  public static boolean isMobileTw(java.lang.CharSequence);
  public static boolean isMobileMo(java.lang.CharSequence);
  public static boolean isTel(java.lang.CharSequence);
  public static boolean isTel400800(java.lang.CharSequence);
  public static boolean isPhone(java.lang.CharSequence);
  public static java.lang.CharSequence hideBefore(java.lang.CharSequence);
  public static java.lang.CharSequence hideBetween(java.lang.CharSequence);
  public static java.lang.CharSequence hideAfter(java.lang.CharSequence);
  public static java.lang.CharSequence subBefore(java.lang.CharSequence);
  public static java.lang.CharSequence subBetween(java.lang.CharSequence);
  public static java.lang.CharSequence subAfter(java.lang.CharSequence);
  public static java.lang.CharSequence subTelBefore(java.lang.CharSequence);
  public static java.lang.CharSequence subTelAfter(java.lang.CharSequence);
}
```

## `cn.hutool.core.util.PrimitiveArrayUtil`

```java
public class cn.hutool.core.util.PrimitiveArrayUtil {
  public cn.hutool.core.util.PrimitiveArrayUtil();
  public static boolean isEmpty(long[]);
  public static boolean isEmpty(int[]);
  public static boolean isEmpty(short[]);
  public static boolean isEmpty(char[]);
  public static boolean isEmpty(byte[]);
  public static boolean isEmpty(double[]);
  public static boolean isEmpty(float[]);
  public static boolean isEmpty(boolean[]);
  public static boolean isNotEmpty(long[]);
  public static boolean isNotEmpty(int[]);
  public static boolean isNotEmpty(short[]);
  public static boolean isNotEmpty(char[]);
  public static boolean isNotEmpty(byte[]);
  public static boolean isNotEmpty(double[]);
  public static boolean isNotEmpty(float[]);
  public static boolean isNotEmpty(boolean[]);
  public static byte[] resize(byte[], int);
  public static byte[] addAll(byte[]...);
  public static int[] addAll(int[]...);
  public static long[] addAll(long[]...);
  public static double[] addAll(double[]...);
  public static float[] addAll(float[]...);
  public static char[] addAll(char[]...);
  public static boolean[] addAll(boolean[]...);
  public static short[] addAll(short[]...);
  public static int[] range(int);
  public static int[] range(int, int);
  public static int[] range(int, int, int);
  public static byte[][] split(byte[], int);
  public static int indexOf(long[], long);
  public static int lastIndexOf(long[], long);
  public static boolean contains(long[], long);
  public static int indexOf(int[], int);
  public static int lastIndexOf(int[], int);
  public static boolean contains(int[], int);
  public static int indexOf(short[], short);
  public static int lastIndexOf(short[], short);
  public static boolean contains(short[], short);
  public static int indexOf(char[], char);
  public static int lastIndexOf(char[], char);
  public static boolean contains(char[], char);
  public static int indexOf(byte[], byte);
  public static int lastIndexOf(byte[], byte);
  public static boolean contains(byte[], byte);
  public static int indexOf(double[], double);
  public static int lastIndexOf(double[], double);
  public static boolean contains(double[], double);
  public static int indexOf(float[], float);
  public static int lastIndexOf(float[], float);
  public static boolean contains(float[], float);
  public static int indexOf(boolean[], boolean);
  public static int lastIndexOf(boolean[], boolean);
  public static boolean contains(boolean[], boolean);
  public static java.lang.Integer[] wrap(int...);
  public static int[] unWrap(java.lang.Integer...);
  public static java.lang.Long[] wrap(long...);
  public static long[] unWrap(java.lang.Long...);
  public static java.lang.Character[] wrap(char...);
  public static char[] unWrap(java.lang.Character...);
  public static java.lang.Byte[] wrap(byte...);
  public static byte[] unWrap(java.lang.Byte...);
  public static java.lang.Short[] wrap(short...);
  public static short[] unWrap(java.lang.Short...);
  public static java.lang.Float[] wrap(float...);
  public static float[] unWrap(java.lang.Float...);
  public static java.lang.Double[] wrap(double...);
  public static double[] unWrap(java.lang.Double...);
  public static java.lang.Boolean[] wrap(boolean...);
  public static boolean[] unWrap(java.lang.Boolean...);
  public static byte[] sub(byte[], int, int);
  public static int[] sub(int[], int, int);
  public static long[] sub(long[], int, int);
  public static short[] sub(short[], int, int);
  public static char[] sub(char[], int, int);
  public static double[] sub(double[], int, int);
  public static float[] sub(float[], int, int);
  public static boolean[] sub(boolean[], int, int);
  public static long[] remove(long[], int) throws java.lang.IllegalArgumentException;
  public static int[] remove(int[], int) throws java.lang.IllegalArgumentException;
  public static short[] remove(short[], int) throws java.lang.IllegalArgumentException;
  public static char[] remove(char[], int) throws java.lang.IllegalArgumentException;
  public static byte[] remove(byte[], int) throws java.lang.IllegalArgumentException;
  public static double[] remove(double[], int) throws java.lang.IllegalArgumentException;
  public static float[] remove(float[], int) throws java.lang.IllegalArgumentException;
  public static boolean[] remove(boolean[], int) throws java.lang.IllegalArgumentException;
  public static java.lang.Object remove(java.lang.Object, int) throws java.lang.IllegalArgumentException;
  public static long[] removeEle(long[], long) throws java.lang.IllegalArgumentException;
  public static int[] removeEle(int[], int) throws java.lang.IllegalArgumentException;
  public static short[] removeEle(short[], short) throws java.lang.IllegalArgumentException;
  public static char[] removeEle(char[], char) throws java.lang.IllegalArgumentException;
  public static byte[] removeEle(byte[], byte) throws java.lang.IllegalArgumentException;
  public static double[] removeEle(double[], double) throws java.lang.IllegalArgumentException;
  public static float[] removeEle(float[], float) throws java.lang.IllegalArgumentException;
  public static boolean[] removeEle(boolean[], boolean) throws java.lang.IllegalArgumentException;
  public static long[] reverse(long[], int, int);
  public static long[] reverse(long[]);
  public static int[] reverse(int[], int, int);
  public static int[] reverse(int[]);
  public static short[] reverse(short[], int, int);
  public static short[] reverse(short[]);
  public static char[] reverse(char[], int, int);
  public static char[] reverse(char[]);
  public static byte[] reverse(byte[], int, int);
  public static byte[] reverse(byte[]);
  public static double[] reverse(double[], int, int);
  public static double[] reverse(double[]);
  public static float[] reverse(float[], int, int);
  public static float[] reverse(float[]);
  public static boolean[] reverse(boolean[], int, int);
  public static boolean[] reverse(boolean[]);
  public static long min(long...);
  public static int min(int...);
  public static short min(short...);
  public static char min(char...);
  public static byte min(byte...);
  public static double min(double...);
  public static float min(float...);
  public static long max(long...);
  public static int max(int...);
  public static short max(short...);
  public static char max(char...);
  public static byte max(byte...);
  public static double max(double...);
  public static float max(float...);
  public static int[] shuffle(int[]);
  public static int[] shuffle(int[], java.util.Random);
  public static long[] shuffle(long[]);
  public static long[] shuffle(long[], java.util.Random);
  public static double[] shuffle(double[]);
  public static double[] shuffle(double[], java.util.Random);
  public static float[] shuffle(float[]);
  public static float[] shuffle(float[], java.util.Random);
  public static boolean[] shuffle(boolean[]);
  public static boolean[] shuffle(boolean[], java.util.Random);
  public static byte[] shuffle(byte[]);
  public static byte[] shuffle(byte[], java.util.Random);
  public static char[] shuffle(char[]);
  public static char[] shuffle(char[], java.util.Random);
  public static short[] shuffle(short[]);
  public static short[] shuffle(short[], java.util.Random);
  public static int[] swap(int[], int, int);
  public static long[] swap(long[], int, int);
  public static double[] swap(double[], int, int);
  public static float[] swap(float[], int, int);
  public static boolean[] swap(boolean[], int, int);
  public static byte[] swap(byte[], int, int);
  public static char[] swap(char[], int, int);
  public static short[] swap(short[], int, int);
  public static boolean isSorted(byte[]);
  public static boolean isSortedASC(byte[]);
  public static boolean isSortedDESC(byte[]);
  public static boolean isSorted(short[]);
  public static boolean isSortedASC(short[]);
  public static boolean isSortedDESC(short[]);
  public static boolean isSorted(char[]);
  public static boolean isSortedASC(char[]);
  public static boolean isSortedDESC(char[]);
  public static boolean isSorted(int[]);
  public static boolean isSortedASC(int[]);
  public static boolean isSortedDESC(int[]);
  public static boolean isSorted(long[]);
  public static boolean isSortedASC(long[]);
  public static boolean isSortedDESC(long[]);
  public static boolean isSorted(double[]);
  public static boolean isSortedASC(double[]);
  public static boolean isSortedDESC(double[]);
  public static boolean isSorted(float[]);
  public static boolean isSortedASC(float[]);
  public static boolean isSortedDESC(float[]);
}
```

## `cn.hutool.core.util.RadixUtil`

```java
public class cn.hutool.core.util.RadixUtil {
  public cn.hutool.core.util.RadixUtil();
  public static java.lang.String encode(java.lang.String, int);
  public static java.lang.String encode(java.lang.String, long);
  public static int decodeToInt(java.lang.String, java.lang.String);
  public static long decode(java.lang.String, java.lang.String);
}
```

## `cn.hutool.core.util.RandomUtil`

```java
public class cn.hutool.core.util.RandomUtil {
  public cn.hutool.core.util.RandomUtil();
  public static java.util.concurrent.ThreadLocalRandom getRandom();
  public static java.security.SecureRandom createSecureRandom(byte[]);
  public static java.security.SecureRandom getSecureRandom();
  public static java.security.SecureRandom getSecureRandom(byte[]);
  public static java.security.SecureRandom getSHA1PRNGRandom(byte[]);
  public static java.security.SecureRandom getSecureRandomStrong();
  public static java.util.Random getRandom(boolean);
  public static boolean randomBoolean();
  public static byte[] randomBytes(int);
  public static int randomInt();
  public static int randomInt(int);
  public static int randomInt(int, int);
  public static int randomInt(int, int, boolean, boolean);
  public static int[] randomInts(int);
  public static long randomLong();
  public static long randomLong(long);
  public static long randomLong(long, long);
  public static long randomLong(long, long, boolean, boolean);
  public static float randomFloat();
  public static float randomFloat(float);
  public static float randomFloat(float, float);
  public static double randomDouble(double, double);
  public static double randomDouble(double, double, int, java.math.RoundingMode);
  public static double randomDouble();
  public static double randomDouble(int, java.math.RoundingMode);
  public static double randomDouble(double);
  public static double randomDouble(double, int, java.math.RoundingMode);
  public static java.math.BigDecimal randomBigDecimal();
  public static java.math.BigDecimal randomBigDecimal(java.math.BigDecimal);
  public static java.math.BigDecimal randomBigDecimal(java.math.BigDecimal, java.math.BigDecimal);
  public static <T> T randomEle(java.util.List<T>);
  public static <T> T randomEle(java.util.List<T>, int);
  public static <T> T randomEle(T[]);
  public static <T> T randomEle(T[], int);
  public static <T> java.util.List<T> randomEles(java.util.List<T>, int);
  public static <T> java.util.List<T> randomEleList(java.util.List<T>, int);
  public static <T> java.util.Set<T> randomEleSet(java.util.Collection<T>, int);
  public static java.lang.String randomString(int);
  public static java.lang.String randomStringLower(int);
  public static java.lang.String randomStringUpper(int);
  public static java.lang.String randomStringWithoutStr(int, java.lang.String);
  public static java.lang.String randomStringLowerWithoutStr(int, java.lang.String);
  public static java.lang.String randomNumbers(int);
  public static java.lang.String randomString(java.lang.String, int);
  public static char randomChinese();
  public static char randomNumber();
  public static char randomChar();
  public static char randomChar(java.lang.String);
  public static <T> cn.hutool.core.lang.WeightRandom<T> weightRandom(cn.hutool.core.lang.WeightRandom$WeightObj<T>[]);
  public static <T> cn.hutool.core.lang.WeightRandom<T> weightRandom(java.lang.Iterable<cn.hutool.core.lang.WeightRandom$WeightObj<T>>);
  public static cn.hutool.core.date.DateTime randomDay(int, int);
  public static cn.hutool.core.date.DateTime randomDate(java.util.Date, cn.hutool.core.date.DateField, int, int);
}
```

## `cn.hutool.core.util.ReUtil`

```java
public class cn.hutool.core.util.ReUtil {
  public cn.hutool.core.util.ReUtil();
  public static java.lang.String getGroup0(java.lang.String, java.lang.CharSequence);
  public static java.lang.String getGroup1(java.lang.String, java.lang.CharSequence);
  public static java.lang.String get(java.lang.String, java.lang.CharSequence, int);
  public static java.lang.String get(java.lang.String, java.lang.CharSequence, java.lang.String);
  public static java.lang.String getGroup0(java.util.regex.Pattern, java.lang.CharSequence);
  public static java.lang.String getGroup1(java.util.regex.Pattern, java.lang.CharSequence);
  public static java.lang.String get(java.util.regex.Pattern, java.lang.CharSequence, int);
  public static java.lang.String get(java.util.regex.Pattern, java.lang.CharSequence, java.lang.String);
  public static void get(java.util.regex.Pattern, java.lang.CharSequence, java.util.function.Consumer<java.util.regex.Matcher>);
  public static java.util.List<java.lang.String> getAllGroups(java.util.regex.Pattern, java.lang.CharSequence);
  public static java.util.List<java.lang.String> getAllGroups(java.util.regex.Pattern, java.lang.CharSequence, boolean);
  public static java.util.List<java.lang.String> getAllGroups(java.util.regex.Pattern, java.lang.CharSequence, boolean, boolean);
  public static java.util.Map<java.lang.String, java.lang.String> getAllGroupNames(java.util.regex.Pattern, java.lang.CharSequence);
  public static java.lang.String extractMulti(java.util.regex.Pattern, java.lang.CharSequence, java.lang.String);
  public static java.lang.String extractMulti(java.lang.String, java.lang.CharSequence, java.lang.String);
  public static java.lang.String extractMultiAndDelPre(java.util.regex.Pattern, cn.hutool.core.lang.mutable.Mutable<java.lang.CharSequence>, java.lang.String);
  public static java.lang.String extractMultiAndDelPre(java.lang.String, cn.hutool.core.lang.mutable.Mutable<java.lang.CharSequence>, java.lang.String);
  public static java.lang.String delFirst(java.lang.String, java.lang.CharSequence);
  public static java.lang.String delFirst(java.util.regex.Pattern, java.lang.CharSequence);
  public static java.lang.String replaceFirst(java.util.regex.Pattern, java.lang.CharSequence, java.lang.String);
  public static java.lang.String delLast(java.lang.String, java.lang.CharSequence);
  public static java.lang.String delLast(java.util.regex.Pattern, java.lang.CharSequence);
  public static java.lang.String delAll(java.lang.String, java.lang.CharSequence);
  public static java.lang.String delAll(java.util.regex.Pattern, java.lang.CharSequence);
  public static java.lang.String delPre(java.lang.String, java.lang.CharSequence);
  public static java.lang.String delPre(java.util.regex.Pattern, java.lang.CharSequence);
  public static java.util.List<java.lang.String> findAllGroup0(java.lang.String, java.lang.CharSequence);
  public static java.util.List<java.lang.String> findAllGroup1(java.lang.String, java.lang.CharSequence);
  public static java.util.List<java.lang.String> findAll(java.lang.String, java.lang.CharSequence, int);
  public static <T extends java.util.Collection<java.lang.String>> T findAll(java.lang.String, java.lang.CharSequence, int, T);
  public static java.util.List<java.lang.String> findAllGroup0(java.util.regex.Pattern, java.lang.CharSequence);
  public static java.util.List<java.lang.String> findAllGroup1(java.util.regex.Pattern, java.lang.CharSequence);
  public static java.util.List<java.lang.String> findAll(java.util.regex.Pattern, java.lang.CharSequence, int);
  public static <T extends java.util.Collection<java.lang.String>> T findAll(java.util.regex.Pattern, java.lang.CharSequence, int, T);
  public static void findAll(java.util.regex.Pattern, java.lang.CharSequence, java.util.function.Consumer<java.util.regex.Matcher>);
  public static int count(java.lang.String, java.lang.CharSequence);
  public static int count(java.util.regex.Pattern, java.lang.CharSequence);
  public static boolean contains(java.lang.String, java.lang.CharSequence);
  public static boolean contains(java.util.regex.Pattern, java.lang.CharSequence);
  public static java.util.regex.MatchResult indexOf(java.lang.String, java.lang.CharSequence);
  public static java.util.regex.MatchResult indexOf(java.util.regex.Pattern, java.lang.CharSequence);
  public static java.util.regex.MatchResult lastIndexOf(java.lang.String, java.lang.CharSequence);
  public static java.util.regex.MatchResult lastIndexOf(java.util.regex.Pattern, java.lang.CharSequence);
  public static java.lang.Integer getFirstNumber(java.lang.CharSequence);
  public static boolean isMatch(java.lang.String, java.lang.CharSequence);
  public static boolean isMatch(java.util.regex.Pattern, java.lang.CharSequence);
  public static java.lang.String replaceAll(java.lang.CharSequence, java.lang.String, java.lang.String);
  public static java.lang.String replaceAll(java.lang.CharSequence, java.util.regex.Pattern, java.lang.String);
  public static java.lang.String replaceAll(java.lang.CharSequence, java.lang.String, cn.hutool.core.lang.func.Func1<java.util.regex.Matcher, java.lang.String>);
  public static java.lang.String replaceAll(java.lang.CharSequence, java.util.regex.Pattern, cn.hutool.core.lang.func.Func1<java.util.regex.Matcher, java.lang.String>);
  public static java.lang.String escape(char);
  public static java.lang.String escape(java.lang.CharSequence);
}
```

## `cn.hutool.core.util.ReferenceUtil`

```java
public class cn.hutool.core.util.ReferenceUtil {
  public cn.hutool.core.util.ReferenceUtil();
  public static <T> java.lang.ref.Reference<T> create(cn.hutool.core.util.ReferenceUtil$ReferenceType, T);
  public static <T> java.lang.ref.Reference<T> create(cn.hutool.core.util.ReferenceUtil$ReferenceType, T, java.lang.ref.ReferenceQueue<T>);
  public static <T> T get(java.lang.ref.Reference<T>);
  public static <T> T get(cn.hutool.core.lang.ref.Ref<T>);
}
```

## `cn.hutool.core.util.ReferenceUtil$ReferenceType`

```java
public final class cn.hutool.core.util.ReferenceUtil$ReferenceType extends java.lang.Enum<cn.hutool.core.util.ReferenceUtil$ReferenceType> {
  public static cn.hutool.core.util.ReferenceUtil$ReferenceType[] values();
  public static cn.hutool.core.util.ReferenceUtil$ReferenceType valueOf(java.lang.String);
}
```

## `cn.hutool.core.util.ReflectUtil`

```java
public class cn.hutool.core.util.ReflectUtil {
  public cn.hutool.core.util.ReflectUtil();
  public static <T> java.lang.reflect.Constructor<T> getConstructor(java.lang.Class<T>, java.lang.Class<?>...);
  public static <T> java.lang.reflect.Constructor<T>[] getConstructors(java.lang.Class<T>) throws java.lang.SecurityException;
  public static java.lang.reflect.Constructor<?>[] getConstructorsDirectly(java.lang.Class<?>) throws java.lang.SecurityException;
  public static boolean hasField(java.lang.Class<?>, java.lang.String) throws java.lang.SecurityException;
  public static java.lang.String getFieldName(java.lang.reflect.Field);
  public static java.lang.reflect.Field getField(java.lang.Class<?>, java.lang.String) throws java.lang.SecurityException;
  public static java.util.Map<java.lang.String, java.lang.reflect.Field> getFieldMap(java.lang.Class<?>);
  public static java.lang.reflect.Field[] getFields(java.lang.Class<?>) throws java.lang.SecurityException;
  public static java.lang.reflect.Field[] getFields(java.lang.Class<?>, cn.hutool.core.lang.Filter<java.lang.reflect.Field>) throws java.lang.SecurityException;
  public static java.lang.reflect.Field[] getFieldsDirectly(java.lang.Class<?>, boolean) throws java.lang.SecurityException;
  public static java.lang.Object getFieldValue(java.lang.Object, java.lang.String) throws cn.hutool.core.exceptions.UtilException;
  public static java.lang.Object getStaticFieldValue(java.lang.reflect.Field) throws cn.hutool.core.exceptions.UtilException;
  public static java.lang.Object getFieldValue(java.lang.Object, java.lang.reflect.Field) throws cn.hutool.core.exceptions.UtilException;
  public static java.lang.Object[] getFieldsValue(java.lang.Object);
  public static java.lang.Object[] getFieldsValue(java.lang.Object, cn.hutool.core.lang.Filter<java.lang.reflect.Field>);
  public static void setFieldValue(java.lang.Object, java.lang.String, java.lang.Object) throws cn.hutool.core.exceptions.UtilException;
  public static void setFieldValue(java.lang.Object, java.lang.reflect.Field, java.lang.Object) throws cn.hutool.core.exceptions.UtilException;
  public static boolean isOuterClassField(java.lang.reflect.Field);
  public static java.util.Set<java.lang.String> getPublicMethodNames(java.lang.Class<?>);
  public static java.lang.reflect.Method[] getPublicMethods(java.lang.Class<?>);
  public static java.util.List<java.lang.reflect.Method> getPublicMethods(java.lang.Class<?>, cn.hutool.core.lang.Filter<java.lang.reflect.Method>);
  public static java.util.List<java.lang.reflect.Method> getPublicMethods(java.lang.Class<?>, java.lang.reflect.Method...);
  public static java.util.List<java.lang.reflect.Method> getPublicMethods(java.lang.Class<?>, java.lang.String...);
  public static java.lang.reflect.Method getPublicMethod(java.lang.Class<?>, java.lang.String, java.lang.Class<?>...) throws java.lang.SecurityException;
  public static java.lang.reflect.Method getMethodOfObj(java.lang.Object, java.lang.String, java.lang.Object...) throws java.lang.SecurityException;
  public static java.lang.reflect.Method getMethodIgnoreCase(java.lang.Class<?>, java.lang.String, java.lang.Class<?>...) throws java.lang.SecurityException;
  public static java.lang.reflect.Method getMethod(java.lang.Class<?>, java.lang.String, java.lang.Class<?>...) throws java.lang.SecurityException;
  public static java.lang.reflect.Method getMethod(java.lang.Class<?>, boolean, java.lang.String, java.lang.Class<?>...) throws java.lang.SecurityException;
  public static java.lang.reflect.Method getMethodByName(java.lang.Class<?>, java.lang.String) throws java.lang.SecurityException;
  public static java.lang.reflect.Method getMethodByNameIgnoreCase(java.lang.Class<?>, java.lang.String) throws java.lang.SecurityException;
  public static java.lang.reflect.Method getMethodByName(java.lang.Class<?>, boolean, java.lang.String) throws java.lang.SecurityException;
  public static java.util.Set<java.lang.String> getMethodNames(java.lang.Class<?>) throws java.lang.SecurityException;
  public static java.lang.reflect.Method[] getMethods(java.lang.Class<?>, cn.hutool.core.lang.Filter<java.lang.reflect.Method>) throws java.lang.SecurityException;
  public static java.lang.reflect.Method[] getMethods(java.lang.Class<?>) throws java.lang.SecurityException;
  public static java.lang.reflect.Method[] getMethodsDirectly(java.lang.Class<?>, boolean, boolean) throws java.lang.SecurityException;
  public static boolean isEqualsMethod(java.lang.reflect.Method);
  public static boolean isHashCodeMethod(java.lang.reflect.Method);
  public static boolean isToStringMethod(java.lang.reflect.Method);
  public static boolean isEmptyParam(java.lang.reflect.Method);
  public static boolean isGetterOrSetterIgnoreCase(java.lang.reflect.Method);
  public static boolean isGetterOrSetter(java.lang.reflect.Method, boolean);
  public static <T> T newInstance(java.lang.String) throws cn.hutool.core.exceptions.UtilException;
  public static <T> T newInstance(java.lang.Class<T>, java.lang.Object...) throws cn.hutool.core.exceptions.UtilException;
  public static <T> T newInstanceIfPossible(java.lang.Class<T>);
  public static <T> T invokeStatic(java.lang.reflect.Method, java.lang.Object...) throws cn.hutool.core.exceptions.UtilException;
  public static <T> T invokeWithCheck(java.lang.Object, java.lang.reflect.Method, java.lang.Object...) throws cn.hutool.core.exceptions.UtilException;
  public static <T> T invoke(java.lang.Object, java.lang.reflect.Method, java.lang.Object...) throws cn.hutool.core.exceptions.InvocationTargetRuntimeException, cn.hutool.core.exceptions.UtilException;
  public static <T> T invokeRaw(java.lang.Object, java.lang.reflect.Method, java.lang.Object...) throws java.lang.reflect.InvocationTargetException, java.lang.IllegalAccessException;
  public static <T> T invoke(java.lang.Object, java.lang.String, java.lang.Object...) throws cn.hutool.core.exceptions.UtilException;
  public static <T extends java.lang.reflect.AccessibleObject> T setAccessible(T);
  public static void removeFinalModify(java.lang.reflect.Field);
}
```

## `cn.hutool.core.util.RuntimeUtil`

```java
public class cn.hutool.core.util.RuntimeUtil {
  public cn.hutool.core.util.RuntimeUtil();
  public static java.lang.String execForStr(java.lang.String...) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String execForStr(java.nio.charset.Charset, java.lang.String...) throws cn.hutool.core.io.IORuntimeException;
  public static java.util.List<java.lang.String> execForLines(java.lang.String...) throws cn.hutool.core.io.IORuntimeException;
  public static java.util.List<java.lang.String> execForLines(java.nio.charset.Charset, java.lang.String...) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.Process exec(java.lang.String...);
  public static java.lang.Process exec(java.lang.String[], java.lang.String...);
  public static java.lang.Process exec(java.lang.String[], java.io.File, java.lang.String...);
  public static java.util.List<java.lang.String> getResultLines(java.lang.Process);
  public static java.util.List<java.lang.String> getResultLines(java.lang.Process, java.nio.charset.Charset);
  public static java.lang.String getResult(java.lang.Process);
  public static java.lang.String getResult(java.lang.Process, java.nio.charset.Charset);
  public static java.lang.String getErrorResult(java.lang.Process);
  public static java.lang.String getErrorResult(java.lang.Process, java.nio.charset.Charset);
  public static void destroy(java.lang.Process);
  public static void addShutdownHook(java.lang.Runnable);
  public static int getProcessorCount();
  public static long getFreeMemory();
  public static long getTotalMemory();
  public static long getMaxMemory();
  public static long getUsableMemory();
  public static int getPid() throws cn.hutool.core.exceptions.UtilException;
}
```

## `cn.hutool.core.util.SerializeUtil`

```java
public class cn.hutool.core.util.SerializeUtil {
  public cn.hutool.core.util.SerializeUtil();
  public static <T> T clone(T);
  public static <T> byte[] serialize(T);
  public static <T> T deserialize(byte[], java.lang.Class<?>...);
}
```

## `cn.hutool.core.util.ServiceLoaderUtil`

```java
public class cn.hutool.core.util.ServiceLoaderUtil {
  public cn.hutool.core.util.ServiceLoaderUtil();
  public static <T> T loadFirstAvailable(java.lang.Class<T>);
  public static <T> T loadFirst(java.lang.Class<T>);
  public static <T> java.util.ServiceLoader<T> load(java.lang.Class<T>);
  public static <T> java.util.ServiceLoader<T> load(java.lang.Class<T>, java.lang.ClassLoader);
  public static <T> java.util.List<T> loadList(java.lang.Class<T>);
  public static <T> java.util.List<T> loadList(java.lang.Class<T>, java.lang.ClassLoader);
}
```

## `cn.hutool.core.util.StrUtil`

```java
public class cn.hutool.core.util.StrUtil extends cn.hutool.core.text.CharSequenceUtil implements cn.hutool.core.text.StrPool {
  public cn.hutool.core.util.StrUtil();
  public static boolean isBlankIfStr(java.lang.Object);
  public static boolean isEmptyIfStr(java.lang.Object);
  public static void trim(java.lang.String[]);
  public static java.lang.String utf8Str(java.lang.Object);
  public static java.lang.String str(java.lang.Object, java.lang.String);
  public static java.lang.String str(java.lang.Object, java.nio.charset.Charset);
  public static java.lang.String str(byte[], java.lang.String);
  public static java.lang.String str(byte[], java.nio.charset.Charset);
  public static java.lang.String str(java.lang.Byte[], java.lang.String);
  public static java.lang.String str(java.lang.Byte[], java.nio.charset.Charset);
  public static java.lang.String str(java.nio.ByteBuffer, java.lang.String);
  public static java.lang.String str(java.nio.ByteBuffer, java.nio.charset.Charset);
  public static java.lang.String toString(java.lang.Object);
  public static java.lang.String toStringOrNull(java.lang.Object);
  public static java.lang.String toStringOrEmpty(java.lang.Object);
  public static java.lang.StringBuilder builder();
  public static cn.hutool.core.text.StrBuilder strBuilder();
  public static java.lang.StringBuilder builder(int);
  public static cn.hutool.core.text.StrBuilder strBuilder(int);
  public static java.io.StringReader getReader(java.lang.CharSequence);
  public static java.io.StringWriter getWriter();
  public static java.lang.String reverse(java.lang.String);
  public static java.lang.String reverseByCodePoint(java.lang.String);
  public static java.lang.String fillBefore(java.lang.String, char, int);
  public static java.lang.String fillAfter(java.lang.String, char, int);
  public static java.lang.String fill(java.lang.String, char, int, boolean);
  public static double similar(java.lang.String, java.lang.String);
  public static java.lang.String similar(java.lang.String, java.lang.String, int);
  public static java.lang.String uuid();
  public static java.lang.String format(java.lang.CharSequence, java.util.Map<?, ?>);
  public static java.lang.String format(java.lang.CharSequence, java.util.Map<?, ?>, boolean);
  public static java.lang.String truncateUtf8(java.lang.String, int);
  public static java.lang.String truncateByByteLength(java.lang.String, java.nio.charset.Charset, int, int, boolean);
}
```

## `cn.hutool.core.util.SystemPropsUtil`

```java
public class cn.hutool.core.util.SystemPropsUtil {
  public cn.hutool.core.util.SystemPropsUtil();
  public static java.lang.String get(java.lang.String, java.lang.String);
  public static java.lang.String get(java.lang.String, boolean);
  public static java.lang.String get(java.lang.String);
  public static boolean getBoolean(java.lang.String, boolean);
  public static int getInt(java.lang.String, int);
  public static long getLong(java.lang.String, long);
  public static java.util.Properties getProps();
  public static void set(java.lang.String, java.lang.String);
}
```

## `cn.hutool.core.util.TypeUtil`

```java
public class cn.hutool.core.util.TypeUtil {
  public cn.hutool.core.util.TypeUtil();
  public static java.lang.Class<?> getClass(java.lang.reflect.Type);
  public static java.lang.reflect.Type getType(java.lang.reflect.Field);
  public static java.lang.reflect.Type getFieldType(java.lang.Class<?>, java.lang.String);
  public static java.lang.Class<?> getClass(java.lang.reflect.Field);
  public static java.lang.reflect.Type getFirstParamType(java.lang.reflect.Method);
  public static java.lang.Class<?> getFirstParamClass(java.lang.reflect.Method);
  public static java.lang.reflect.Type getParamType(java.lang.reflect.Method, int);
  public static java.lang.Class<?> getParamClass(java.lang.reflect.Method, int);
  public static java.lang.reflect.Type[] getParamTypes(java.lang.reflect.Method);
  public static java.lang.Class<?>[] getParamClasses(java.lang.reflect.Method);
  public static java.lang.reflect.Type getReturnType(java.lang.reflect.Method);
  public static java.lang.Class<?> getReturnClass(java.lang.reflect.Method);
  public static java.lang.reflect.Type getTypeArgument(java.lang.reflect.Type);
  public static java.lang.reflect.Type getTypeArgument(java.lang.reflect.Type, int);
  public static java.lang.reflect.Type[] getTypeArguments(java.lang.reflect.Type);
  public static java.lang.reflect.ParameterizedType toParameterizedType(java.lang.reflect.Type);
  public static java.lang.reflect.ParameterizedType toParameterizedType(java.lang.reflect.Type, int);
  public static java.lang.reflect.ParameterizedType[] getGenerics(java.lang.Class<?>);
  public static boolean isUnknown(java.lang.reflect.Type);
  public static boolean hasTypeVariable(java.lang.reflect.Type...);
  public static java.util.Map<java.lang.reflect.Type, java.lang.reflect.Type> getTypeMap(java.lang.Class<?>);
  public static java.lang.reflect.Type getActualType(java.lang.reflect.Type, java.lang.reflect.Field);
  public static java.lang.reflect.Type getActualType(java.lang.reflect.Type, java.lang.reflect.Type);
  public static java.lang.reflect.Type getActualType(java.lang.reflect.Type, java.lang.reflect.ParameterizedType);
  public static java.lang.reflect.Type[] getActualTypes(java.lang.reflect.Type, java.lang.reflect.Type...);
}
```

## `cn.hutool.core.util.URLUtil`

```java
public class cn.hutool.core.util.URLUtil extends cn.hutool.core.net.URLEncodeUtil {
  public cn.hutool.core.util.URLUtil();
  public static java.net.URL url(java.net.URI) throws cn.hutool.core.exceptions.UtilException;
  public static java.net.URL url(java.lang.String);
  public static java.net.URL url(java.lang.String, java.net.URLStreamHandler);
  public static java.net.URI getStringURI(java.lang.CharSequence);
  public static java.net.URL toUrlForHttp(java.lang.String);
  public static java.net.URL toUrlForHttp(java.lang.String, java.net.URLStreamHandler);
  public static java.lang.String encodeBlank(java.lang.CharSequence);
  public static java.net.URL getURL(java.lang.String);
  public static java.net.URL getURL(java.lang.String, java.lang.Class<?>);
  public static java.net.URL getURL(java.io.File);
  public static java.net.URL[] getURLs(java.io.File...);
  public static java.net.URI getHost(java.net.URL);
  public static java.lang.String completeUrl(java.lang.String, java.lang.String);
  public static java.lang.String decode(java.lang.String) throws cn.hutool.core.exceptions.UtilException;
  public static java.lang.String decode(java.lang.String, java.nio.charset.Charset);
  public static java.lang.String decode(java.lang.String, java.nio.charset.Charset, boolean);
  public static java.lang.String decode(java.lang.String, java.lang.String) throws cn.hutool.core.exceptions.UtilException;
  public static java.lang.String getPath(java.lang.String);
  public static java.lang.String getDecodedPath(java.net.URL);
  public static java.net.URI toURI(java.net.URL) throws cn.hutool.core.exceptions.UtilException;
  public static java.net.URI toURI(java.net.URL, boolean) throws cn.hutool.core.exceptions.UtilException;
  public static java.net.URI toURI(java.lang.String) throws cn.hutool.core.exceptions.UtilException;
  public static java.net.URI toURI(java.lang.String, boolean) throws cn.hutool.core.exceptions.UtilException;
  public static boolean isFileURL(java.net.URL);
  public static boolean isJarURL(java.net.URL);
  public static boolean isJarFileURL(java.net.URL);
  public static java.io.InputStream getStream(java.net.URL);
  public static java.io.BufferedReader getReader(java.net.URL, java.nio.charset.Charset);
  public static java.util.jar.JarFile getJarFile(java.net.URL);
  public static java.lang.String normalize(java.lang.String);
  public static java.lang.String normalize(java.lang.String, boolean);
  public static java.lang.String normalize(java.lang.String, boolean, boolean);
  public static java.lang.String buildQuery(java.util.Map<java.lang.String, ?>, java.nio.charset.Charset);
  public static long getContentLength(java.net.URL) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String getDataUriBase64(java.lang.String, java.lang.String);
  public static java.lang.String getDataUri(java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String getDataUri(java.lang.String, java.nio.charset.Charset, java.lang.String, java.lang.String);
  public static long size(java.net.URL);
  public static void useCachesIfNecessary(java.net.URLConnection);
}
```

## `cn.hutool.core.util.VersionUtil`

```java
public class cn.hutool.core.util.VersionUtil {
  public cn.hutool.core.util.VersionUtil();
  public static boolean anyMatch(java.lang.String, java.util.Collection<java.lang.String>);
  public static boolean anyMatch(java.lang.String, java.lang.String...);
  public static boolean isGreaterThan(java.lang.String, java.lang.String);
  public static boolean isGreaterThanOrEqual(java.lang.String, java.lang.String);
  public static boolean isLessThan(java.lang.String, java.lang.String);
  public static boolean isLessThanOrEqual(java.lang.String, java.lang.String);
  public static boolean matchEl(java.lang.String, java.lang.String);
  public static boolean matchEl(java.lang.String, java.lang.String, java.lang.String);
}
```

## `cn.hutool.core.util.XmlUtil`

```java
public class cn.hutool.core.util.XmlUtil {
  public cn.hutool.core.util.XmlUtil();
  public static synchronized void disableDefaultDocumentBuilderFactory();
  public static synchronized void setNamespaceAware(boolean);
  public static org.w3c.dom.Document readXML(java.io.File);
  public static org.w3c.dom.Document readXML(java.lang.String);
  public static org.w3c.dom.Document readXML(java.io.InputStream) throws cn.hutool.core.exceptions.UtilException;
  public static org.w3c.dom.Document readXML(java.io.Reader) throws cn.hutool.core.exceptions.UtilException;
  public static org.w3c.dom.Document readXML(org.xml.sax.InputSource);
  public static void readBySax(java.io.File, org.xml.sax.ContentHandler);
  public static void readBySax(java.io.Reader, org.xml.sax.ContentHandler);
  public static void readBySax(java.io.InputStream, org.xml.sax.ContentHandler);
  public static void readBySax(org.xml.sax.InputSource, org.xml.sax.ContentHandler);
  public static org.w3c.dom.Document parseXml(java.lang.String);
  public static java.lang.String toStr(org.w3c.dom.Node);
  public static java.lang.String toStr(org.w3c.dom.Document);
  public static java.lang.String toStr(org.w3c.dom.Node, boolean);
  public static java.lang.String toStr(org.w3c.dom.Document, boolean);
  public static java.lang.String toStr(org.w3c.dom.Node, java.lang.String, boolean);
  public static java.lang.String toStr(org.w3c.dom.Document, java.lang.String, boolean);
  public static java.lang.String toStr(org.w3c.dom.Node, java.lang.String, boolean, boolean);
  public static java.lang.String format(org.w3c.dom.Document);
  public static java.lang.String format(java.lang.String);
  public static void toFile(org.w3c.dom.Document, java.lang.String);
  public static void toFile(org.w3c.dom.Document, java.lang.String, java.lang.String);
  public static void write(org.w3c.dom.Node, java.io.Writer, java.lang.String, int);
  public static void write(org.w3c.dom.Node, java.io.Writer, java.lang.String, int, boolean);
  public static void write(org.w3c.dom.Node, java.io.OutputStream, java.lang.String, int);
  public static void write(org.w3c.dom.Node, java.io.OutputStream, java.lang.String, int, boolean);
  public static void transform(javax.xml.transform.Source, javax.xml.transform.Result, java.lang.String, int);
  public static void transform(javax.xml.transform.Source, javax.xml.transform.Result, java.lang.String, int, boolean);
  public static org.w3c.dom.Document createXml();
  public static javax.xml.parsers.DocumentBuilder createDocumentBuilder();
  public static javax.xml.parsers.DocumentBuilderFactory createDocumentBuilderFactory();
  public static org.w3c.dom.Document createXml(java.lang.String);
  public static org.w3c.dom.Document createXml(java.lang.String, java.lang.String);
  public static org.w3c.dom.Element getRootElement(org.w3c.dom.Document);
  public static org.w3c.dom.Document getOwnerDocument(org.w3c.dom.Node);
  public static java.lang.String cleanInvalid(java.lang.String);
  public static java.lang.String cleanComment(java.lang.String);
  public static java.util.List<org.w3c.dom.Element> getElements(org.w3c.dom.Element, java.lang.String);
  public static org.w3c.dom.Element getElement(org.w3c.dom.Element, java.lang.String);
  public static java.lang.String elementText(org.w3c.dom.Element, java.lang.String);
  public static java.lang.String elementText(org.w3c.dom.Element, java.lang.String, java.lang.String);
  public static java.util.List<org.w3c.dom.Element> transElements(org.w3c.dom.NodeList);
  public static java.util.List<org.w3c.dom.Element> transElements(org.w3c.dom.Element, org.w3c.dom.NodeList);
  public static void writeObjectAsXml(java.io.File, java.lang.Object);
  public static javax.xml.xpath.XPath createXPath();
  public static org.w3c.dom.Element getElementByXPath(java.lang.String, java.lang.Object);
  public static org.w3c.dom.NodeList getNodeListByXPath(java.lang.String, java.lang.Object);
  public static org.w3c.dom.Node getNodeByXPath(java.lang.String, java.lang.Object);
  public static java.lang.Object getByXPath(java.lang.String, java.lang.Object, javax.xml.namespace.QName);
  public static java.lang.Object getByXPath(java.lang.String, java.lang.Object, javax.xml.namespace.QName, javax.xml.namespace.NamespaceContext);
  public static java.lang.String escape(java.lang.String);
  public static java.lang.String unescape(java.lang.String);
  public static java.util.Map<java.lang.String, java.lang.Object> xmlToMap(java.lang.String);
  public static <T> T xmlToBean(org.w3c.dom.Node, java.lang.Class<T>);
  public static <T> T xmlToBean(org.w3c.dom.Node, java.lang.Class<T>, cn.hutool.core.bean.copier.CopyOptions);
  public static java.util.Map<java.lang.String, java.lang.Object> xmlToMap(org.w3c.dom.Node);
  public static java.util.Map<java.lang.String, java.lang.Object> xmlToMap(java.lang.String, java.util.Map<java.lang.String, java.lang.Object>);
  public static java.util.Map<java.lang.String, java.lang.Object> xmlToMap(org.w3c.dom.Node, java.util.Map<java.lang.String, java.lang.Object>);
  public static java.lang.String mapToXmlStr(java.util.Map<?, ?>);
  public static java.lang.String mapToXmlStr(java.util.Map<?, ?>, boolean);
  public static java.lang.String mapToXmlStr(java.util.Map<?, ?>, java.lang.String);
  public static java.lang.String mapToXmlStr(java.util.Map<?, ?>, java.lang.String, java.lang.String);
  public static java.lang.String mapToXmlStr(java.util.Map<?, ?>, java.lang.String, java.lang.String, boolean);
  public static java.lang.String mapToXmlStr(java.util.Map<?, ?>, java.lang.String, java.lang.String, boolean, boolean);
  public static java.lang.String mapToXmlStr(java.util.Map<?, ?>, java.lang.String, java.lang.String, java.lang.String, boolean, boolean);
  public static org.w3c.dom.Document mapToXml(java.util.Map<?, ?>, java.lang.String);
  public static org.w3c.dom.Document mapToXml(java.util.Map<?, ?>, java.lang.String, java.lang.String);
  public static org.w3c.dom.Document beanToXml(java.lang.Object);
  public static org.w3c.dom.Document beanToXml(java.lang.Object, java.lang.String);
  public static org.w3c.dom.Document beanToXml(java.lang.Object, java.lang.String, boolean);
  public static boolean isElement(org.w3c.dom.Node);
  public static org.w3c.dom.Element appendChild(org.w3c.dom.Node, java.lang.String);
  public static org.w3c.dom.Element appendChild(org.w3c.dom.Node, java.lang.String, java.lang.String);
  public static org.w3c.dom.Node appendText(org.w3c.dom.Node, java.lang.CharSequence);
  public static void append(org.w3c.dom.Node, java.lang.Object);
}
```

## `cn.hutool.core.util.XmlUtil$UniversalNamespaceCache`

```java
public class cn.hutool.core.util.XmlUtil$UniversalNamespaceCache implements javax.xml.namespace.NamespaceContext {
  public cn.hutool.core.util.XmlUtil$UniversalNamespaceCache(org.w3c.dom.Node, boolean);
  public java.lang.String getNamespaceURI(java.lang.String);
  public java.lang.String getPrefix(java.lang.String);
  public java.util.Iterator<java.lang.String> getPrefixes(java.lang.String);
}
```

## `cn.hutool.core.util.ZipUtil`

```java
public class cn.hutool.core.util.ZipUtil {
  public cn.hutool.core.util.ZipUtil();
  public static java.util.zip.ZipFile toZipFile(java.io.File, java.nio.charset.Charset);
  public static java.io.InputStream getStream(java.util.zip.ZipFile, java.util.zip.ZipEntry);
  public static java.util.zip.ZipOutputStream getZipOutputStream(java.io.OutputStream, java.nio.charset.Charset);
  public static void append(java.nio.file.Path, java.nio.file.Path, java.nio.file.CopyOption...) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File zip(java.lang.String) throws cn.hutool.core.exceptions.UtilException;
  public static java.io.File zip(java.lang.String, java.nio.charset.Charset) throws cn.hutool.core.exceptions.UtilException;
  public static java.io.File zip(java.io.File) throws cn.hutool.core.exceptions.UtilException;
  public static java.io.File zip(java.io.File, java.nio.charset.Charset) throws cn.hutool.core.exceptions.UtilException;
  public static java.io.File zip(java.lang.String, java.lang.String) throws cn.hutool.core.exceptions.UtilException;
  public static java.io.File zip(java.lang.String, java.lang.String, boolean) throws cn.hutool.core.exceptions.UtilException;
  public static java.io.File zip(java.lang.String, java.lang.String, java.nio.charset.Charset, boolean) throws cn.hutool.core.exceptions.UtilException;
  public static java.io.File zip(java.io.File, boolean, java.io.File...) throws cn.hutool.core.exceptions.UtilException;
  public static java.io.File zip(java.io.File, java.nio.charset.Charset, boolean, java.io.File...) throws cn.hutool.core.exceptions.UtilException;
  public static java.io.File zip(java.io.File, java.nio.charset.Charset, boolean, java.io.FileFilter, java.io.File...) throws cn.hutool.core.io.IORuntimeException;
  public static void zip(java.io.OutputStream, java.nio.charset.Charset, boolean, java.io.FileFilter, java.io.File...) throws cn.hutool.core.io.IORuntimeException;
  public static void zip(java.util.zip.ZipOutputStream, boolean, java.io.FileFilter, java.io.File...) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File zip(java.io.File, java.lang.String, java.lang.String) throws cn.hutool.core.exceptions.UtilException;
  public static java.io.File zip(java.io.File, java.lang.String, java.lang.String, java.nio.charset.Charset) throws cn.hutool.core.exceptions.UtilException;
  public static java.io.File zip(java.io.File, java.lang.String, java.io.InputStream) throws cn.hutool.core.exceptions.UtilException;
  public static java.io.File zip(java.io.File, java.lang.String, java.io.InputStream, java.nio.charset.Charset) throws cn.hutool.core.exceptions.UtilException;
  public static java.io.File zip(java.io.File, java.lang.String[], java.io.InputStream[]) throws cn.hutool.core.exceptions.UtilException;
  public static java.io.File zip(java.io.File, java.lang.String[], java.io.InputStream[], java.nio.charset.Charset) throws cn.hutool.core.exceptions.UtilException;
  public static void zip(java.io.OutputStream, java.lang.String[], java.io.InputStream[]);
  public static void zip(java.util.zip.ZipOutputStream, java.lang.String[], java.io.InputStream[]) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File zip(java.io.File, java.nio.charset.Charset, cn.hutool.core.io.resource.Resource...) throws cn.hutool.core.exceptions.UtilException;
  public static java.io.File unzip(java.lang.String) throws cn.hutool.core.exceptions.UtilException;
  public static java.io.File unzip(java.lang.String, java.nio.charset.Charset) throws cn.hutool.core.exceptions.UtilException;
  public static java.io.File unzip(java.io.File) throws cn.hutool.core.exceptions.UtilException;
  public static java.io.File unzip(java.io.File, java.nio.charset.Charset) throws cn.hutool.core.exceptions.UtilException;
  public static java.io.File unzip(java.lang.String, java.lang.String) throws cn.hutool.core.exceptions.UtilException;
  public static java.io.File unzip(java.lang.String, java.lang.String, java.nio.charset.Charset) throws cn.hutool.core.exceptions.UtilException;
  public static java.io.File unzip(java.io.File, java.io.File) throws cn.hutool.core.exceptions.UtilException;
  public static java.io.File unzip(java.io.File, java.io.File, java.nio.charset.Charset);
  public static java.io.File unzip(java.util.zip.ZipFile, java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File unzip(java.util.zip.ZipFile, java.io.File, long) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.InputStream get(java.io.File, java.nio.charset.Charset, java.lang.String);
  public static java.io.InputStream get(java.util.zip.ZipFile, java.lang.String);
  public static void read(java.util.zip.ZipFile, java.util.function.Consumer<java.util.zip.ZipEntry>);
  public static java.io.File unzip(java.io.InputStream, java.io.File, java.nio.charset.Charset) throws cn.hutool.core.exceptions.UtilException;
  public static java.io.File unzip(java.util.zip.ZipInputStream, java.io.File) throws cn.hutool.core.exceptions.UtilException;
  public static void read(java.util.zip.ZipInputStream, java.util.function.Consumer<java.util.zip.ZipEntry>);
  public static byte[] unzipFileBytes(java.lang.String, java.lang.String);
  public static byte[] unzipFileBytes(java.lang.String, java.nio.charset.Charset, java.lang.String);
  public static byte[] unzipFileBytes(java.io.File, java.lang.String);
  public static byte[] unzipFileBytes(java.io.File, java.nio.charset.Charset, java.lang.String);
  public static byte[] gzip(java.lang.String, java.lang.String) throws cn.hutool.core.exceptions.UtilException;
  public static byte[] gzip(byte[]) throws cn.hutool.core.exceptions.UtilException;
  public static byte[] gzip(java.io.File) throws cn.hutool.core.exceptions.UtilException;
  public static byte[] gzip(java.io.InputStream) throws cn.hutool.core.exceptions.UtilException;
  public static byte[] gzip(java.io.InputStream, int) throws cn.hutool.core.exceptions.UtilException;
  public static java.lang.String unGzip(byte[], java.lang.String) throws cn.hutool.core.exceptions.UtilException;
  public static byte[] unGzip(byte[]) throws cn.hutool.core.exceptions.UtilException;
  public static byte[] unGzip(java.io.InputStream) throws cn.hutool.core.exceptions.UtilException;
  public static byte[] unGzip(java.io.InputStream, int) throws cn.hutool.core.exceptions.UtilException;
  public static byte[] zlib(java.lang.String, java.lang.String, int);
  public static byte[] zlib(java.io.File, int);
  public static byte[] zlib(byte[], int);
  public static byte[] zlib(java.io.InputStream, int);
  public static byte[] zlib(java.io.InputStream, int, int);
  public static java.lang.String unZlib(byte[], java.lang.String);
  public static byte[] unZlib(byte[]);
  public static byte[] unZlib(java.io.InputStream);
  public static byte[] unZlib(java.io.InputStream, int);
  public static java.util.List<java.lang.String> listFileNames(java.util.zip.ZipFile, java.lang.String);
}
```
