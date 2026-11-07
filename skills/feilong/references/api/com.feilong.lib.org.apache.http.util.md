# com.feilong.lib.org.apache.http.util

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.util.Args`

```java
public class com.feilong.lib.org.apache.http.util.Args {
  public com.feilong.lib.org.apache.http.util.Args();
  public static void check(boolean, java.lang.String);
  public static void check(boolean, java.lang.String, java.lang.Object...);
  public static void check(boolean, java.lang.String, java.lang.Object);
  public static <T> T notNull(T, java.lang.String);
  public static <T extends java.lang.CharSequence> T notEmpty(T, java.lang.String);
  public static <T extends java.lang.CharSequence> T notBlank(T, java.lang.String);
  public static <T extends java.lang.CharSequence> T containsNoBlanks(T, java.lang.String);
  public static <E, T extends java.util.Collection<E>> T notEmpty(T, java.lang.String);
  public static int positive(int, java.lang.String);
  public static long positive(long, java.lang.String);
  public static int notNegative(int, java.lang.String);
  public static long notNegative(long, java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.util.Asserts`

```java
public class com.feilong.lib.org.apache.http.util.Asserts {
  public com.feilong.lib.org.apache.http.util.Asserts();
  public static void check(boolean, java.lang.String);
  public static void check(boolean, java.lang.String, java.lang.Object...);
  public static void check(boolean, java.lang.String, java.lang.Object);
  public static void notNull(java.lang.Object, java.lang.String);
  public static void notEmpty(java.lang.CharSequence, java.lang.String);
  public static void notBlank(java.lang.CharSequence, java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.util.ByteArrayBuffer`

```java
public final class com.feilong.lib.org.apache.http.util.ByteArrayBuffer implements java.io.Serializable {
  public com.feilong.lib.org.apache.http.util.ByteArrayBuffer(int);
  public void append(byte[], int, int);
  public void append(int);
  public void append(char[], int, int);
  public void append(com.feilong.lib.org.apache.http.util.CharArrayBuffer, int, int);
  public void clear();
  public byte[] toByteArray();
  public int byteAt(int);
  public int capacity();
  public int length();
  public void ensureCapacity(int);
  public byte[] buffer();
  public void setLength(int);
  public boolean isEmpty();
  public boolean isFull();
  public int indexOf(byte, int, int);
  public int indexOf(byte);
}
```

## `com.feilong.lib.org.apache.http.util.CharArrayBuffer`

```java
public final class com.feilong.lib.org.apache.http.util.CharArrayBuffer implements java.lang.CharSequence,java.io.Serializable {
  public com.feilong.lib.org.apache.http.util.CharArrayBuffer(int);
  public void append(char[], int, int);
  public void append(java.lang.String);
  public void append(com.feilong.lib.org.apache.http.util.CharArrayBuffer, int, int);
  public void append(com.feilong.lib.org.apache.http.util.CharArrayBuffer);
  public void append(char);
  public void append(byte[], int, int);
  public void append(com.feilong.lib.org.apache.http.util.ByteArrayBuffer, int, int);
  public void append(java.lang.Object);
  public void clear();
  public char[] toCharArray();
  public char charAt(int);
  public char[] buffer();
  public int capacity();
  public int length();
  public void ensureCapacity(int);
  public void setLength(int);
  public boolean isEmpty();
  public boolean isFull();
  public int indexOf(int, int, int);
  public int indexOf(int);
  public java.lang.String substring(int, int);
  public java.lang.String substringTrimmed(int, int);
  public java.lang.CharSequence subSequence(int, int);
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.util.CharsetUtils`

```java
public class com.feilong.lib.org.apache.http.util.CharsetUtils {
  public com.feilong.lib.org.apache.http.util.CharsetUtils();
  public static java.nio.charset.Charset lookup(java.lang.String);
  public static java.nio.charset.Charset get(java.lang.String) throws java.io.UnsupportedEncodingException;
}
```

## `com.feilong.lib.org.apache.http.util.EncodingUtils`

```java
public final class com.feilong.lib.org.apache.http.util.EncodingUtils {
  public static java.lang.String getString(byte[], int, int, java.lang.String);
  public static java.lang.String getString(byte[], java.lang.String);
  public static byte[] getBytes(java.lang.String, java.lang.String);
  public static byte[] getAsciiBytes(java.lang.String);
  public static java.lang.String getAsciiString(byte[], int, int);
  public static java.lang.String getAsciiString(byte[]);
}
```

## `com.feilong.lib.org.apache.http.util.EntityUtils`

```java
public final class com.feilong.lib.org.apache.http.util.EntityUtils {
  public static void consumeQuietly(com.feilong.lib.org.apache.http.HttpEntity);
  public static void consume(com.feilong.lib.org.apache.http.HttpEntity) throws java.io.IOException;
  public static void updateEntity(com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.HttpEntity) throws java.io.IOException;
  public static byte[] toByteArray(com.feilong.lib.org.apache.http.HttpEntity) throws java.io.IOException;
  public static java.lang.String toString(com.feilong.lib.org.apache.http.HttpEntity, java.nio.charset.Charset) throws java.io.IOException, com.feilong.lib.org.apache.http.ParseException;
  public static java.lang.String toString(com.feilong.lib.org.apache.http.HttpEntity, java.lang.String) throws java.io.IOException, com.feilong.lib.org.apache.http.ParseException;
  public static java.lang.String toString(com.feilong.lib.org.apache.http.HttpEntity) throws java.io.IOException, com.feilong.lib.org.apache.http.ParseException;
}
```

## `com.feilong.lib.org.apache.http.util.LangUtils`

```java
public final class com.feilong.lib.org.apache.http.util.LangUtils {
  public static int hashCode(int, int);
  public static int hashCode(int, boolean);
  public static int hashCode(int, java.lang.Object);
  public static boolean equals(java.lang.Object, java.lang.Object);
  public static boolean equals(java.lang.Object[], java.lang.Object[]);
}
```

## `com.feilong.lib.org.apache.http.util.NetUtils`

```java
public final class com.feilong.lib.org.apache.http.util.NetUtils {
  public com.feilong.lib.org.apache.http.util.NetUtils();
  public static void formatAddress(java.lang.StringBuilder, java.net.SocketAddress);
}
```

## `com.feilong.lib.org.apache.http.util.TextUtils`

```java
public final class com.feilong.lib.org.apache.http.util.TextUtils {
  public com.feilong.lib.org.apache.http.util.TextUtils();
  public static boolean isEmpty(java.lang.CharSequence);
  public static boolean isBlank(java.lang.CharSequence);
  public static boolean containsBlanks(java.lang.CharSequence);
}
```
