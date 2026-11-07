# com.google.common.hash

版本：33.4.8-jre。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.google.common.hash.BloomFilter`

```java
public final class com.google.common.hash.BloomFilter<T> implements com.google.common.base.Predicate<T>, java.io.Serializable {
  public com.google.common.hash.BloomFilter<T> copy();
  public boolean mightContain(T);
  public boolean apply(T);
  public boolean test(T);
  public boolean put(T);
  public double expectedFpp();
  public long approximateElementCount();
  public boolean isCompatible(com.google.common.hash.BloomFilter<T>);
  public void putAll(com.google.common.hash.BloomFilter<T>);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public static <T> java.util.stream.Collector<T, ?, com.google.common.hash.BloomFilter<T>> toBloomFilter(com.google.common.hash.Funnel<? super T>, long);
  public static <T> java.util.stream.Collector<T, ?, com.google.common.hash.BloomFilter<T>> toBloomFilter(com.google.common.hash.Funnel<? super T>, long, double);
  public static <T> com.google.common.hash.BloomFilter<T> create(com.google.common.hash.Funnel<? super T>, int, double);
  public static <T> com.google.common.hash.BloomFilter<T> create(com.google.common.hash.Funnel<? super T>, long, double);
  public static <T> com.google.common.hash.BloomFilter<T> create(com.google.common.hash.Funnel<? super T>, int);
  public static <T> com.google.common.hash.BloomFilter<T> create(com.google.common.hash.Funnel<? super T>, long);
  public void writeTo(java.io.OutputStream) throws java.io.IOException;
  public static <T> com.google.common.hash.BloomFilter<T> readFrom(java.io.InputStream, com.google.common.hash.Funnel<? super T>) throws java.io.IOException;
}
```

## `com.google.common.hash.Funnel`

```java
public interface com.google.common.hash.Funnel<T> extends java.io.Serializable {
  public abstract void funnel(T, com.google.common.hash.PrimitiveSink);
}
```

## `com.google.common.hash.Funnels`

```java
public final class com.google.common.hash.Funnels {
  public static com.google.common.hash.Funnel<byte[]> byteArrayFunnel();
  public static com.google.common.hash.Funnel<java.lang.CharSequence> unencodedCharsFunnel();
  public static com.google.common.hash.Funnel<java.lang.CharSequence> stringFunnel(java.nio.charset.Charset);
  public static com.google.common.hash.Funnel<java.lang.Integer> integerFunnel();
  public static <E> com.google.common.hash.Funnel<java.lang.Iterable<? extends E>> sequentialFunnel(com.google.common.hash.Funnel<E>);
  public static com.google.common.hash.Funnel<java.lang.Long> longFunnel();
  public static java.io.OutputStream asOutputStream(com.google.common.hash.PrimitiveSink);
}
```

## `com.google.common.hash.HashCode`

```java
public abstract class com.google.common.hash.HashCode {
  public abstract int bits();
  public abstract int asInt();
  public abstract long asLong();
  public abstract long padToLong();
  public abstract byte[] asBytes();
  public int writeBytesTo(byte[], int, int);
  public static com.google.common.hash.HashCode fromInt(int);
  public static com.google.common.hash.HashCode fromLong(long);
  public static com.google.common.hash.HashCode fromBytes(byte[]);
  public static com.google.common.hash.HashCode fromString(java.lang.String);
  public final boolean equals(java.lang.Object);
  public final int hashCode();
  public final java.lang.String toString();
}
```

## `com.google.common.hash.HashFunction`

```java
public interface com.google.common.hash.HashFunction {
  public abstract com.google.common.hash.Hasher newHasher();
  public abstract com.google.common.hash.Hasher newHasher(int);
  public abstract com.google.common.hash.HashCode hashInt(int);
  public abstract com.google.common.hash.HashCode hashLong(long);
  public abstract com.google.common.hash.HashCode hashBytes(byte[]);
  public abstract com.google.common.hash.HashCode hashBytes(byte[], int, int);
  public abstract com.google.common.hash.HashCode hashBytes(java.nio.ByteBuffer);
  public abstract com.google.common.hash.HashCode hashUnencodedChars(java.lang.CharSequence);
  public abstract com.google.common.hash.HashCode hashString(java.lang.CharSequence, java.nio.charset.Charset);
  public abstract <T> com.google.common.hash.HashCode hashObject(T, com.google.common.hash.Funnel<? super T>);
  public abstract int bits();
}
```

## `com.google.common.hash.Hasher`

```java
public interface com.google.common.hash.Hasher extends com.google.common.hash.PrimitiveSink {
  public abstract com.google.common.hash.Hasher putByte(byte);
  public abstract com.google.common.hash.Hasher putBytes(byte[]);
  public abstract com.google.common.hash.Hasher putBytes(byte[], int, int);
  public abstract com.google.common.hash.Hasher putBytes(java.nio.ByteBuffer);
  public abstract com.google.common.hash.Hasher putShort(short);
  public abstract com.google.common.hash.Hasher putInt(int);
  public abstract com.google.common.hash.Hasher putLong(long);
  public abstract com.google.common.hash.Hasher putFloat(float);
  public abstract com.google.common.hash.Hasher putDouble(double);
  public abstract com.google.common.hash.Hasher putBoolean(boolean);
  public abstract com.google.common.hash.Hasher putChar(char);
  public abstract com.google.common.hash.Hasher putUnencodedChars(java.lang.CharSequence);
  public abstract com.google.common.hash.Hasher putString(java.lang.CharSequence, java.nio.charset.Charset);
  public abstract <T> com.google.common.hash.Hasher putObject(T, com.google.common.hash.Funnel<? super T>);
  public abstract com.google.common.hash.HashCode hash();
  public abstract int hashCode();
  public default com.google.common.hash.PrimitiveSink putString(java.lang.CharSequence, java.nio.charset.Charset);
  public default com.google.common.hash.PrimitiveSink putUnencodedChars(java.lang.CharSequence);
  public default com.google.common.hash.PrimitiveSink putChar(char);
  public default com.google.common.hash.PrimitiveSink putBoolean(boolean);
  public default com.google.common.hash.PrimitiveSink putDouble(double);
  public default com.google.common.hash.PrimitiveSink putFloat(float);
  public default com.google.common.hash.PrimitiveSink putLong(long);
  public default com.google.common.hash.PrimitiveSink putInt(int);
  public default com.google.common.hash.PrimitiveSink putShort(short);
  public default com.google.common.hash.PrimitiveSink putBytes(java.nio.ByteBuffer);
  public default com.google.common.hash.PrimitiveSink putBytes(byte[], int, int);
  public default com.google.common.hash.PrimitiveSink putBytes(byte[]);
  public default com.google.common.hash.PrimitiveSink putByte(byte);
}
```

## `com.google.common.hash.Hashing`

```java
public final class com.google.common.hash.Hashing {
  public static com.google.common.hash.HashFunction goodFastHash(int);
  public static com.google.common.hash.HashFunction murmur3_32(int);
  public static com.google.common.hash.HashFunction murmur3_32();
  public static com.google.common.hash.HashFunction murmur3_32_fixed(int);
  public static com.google.common.hash.HashFunction murmur3_32_fixed();
  public static com.google.common.hash.HashFunction murmur3_128(int);
  public static com.google.common.hash.HashFunction murmur3_128();
  public static com.google.common.hash.HashFunction sipHash24();
  public static com.google.common.hash.HashFunction sipHash24(long, long);
  public static com.google.common.hash.HashFunction md5();
  public static com.google.common.hash.HashFunction sha1();
  public static com.google.common.hash.HashFunction sha256();
  public static com.google.common.hash.HashFunction sha384();
  public static com.google.common.hash.HashFunction sha512();
  public static com.google.common.hash.HashFunction hmacMd5(java.security.Key);
  public static com.google.common.hash.HashFunction hmacMd5(byte[]);
  public static com.google.common.hash.HashFunction hmacSha1(java.security.Key);
  public static com.google.common.hash.HashFunction hmacSha1(byte[]);
  public static com.google.common.hash.HashFunction hmacSha256(java.security.Key);
  public static com.google.common.hash.HashFunction hmacSha256(byte[]);
  public static com.google.common.hash.HashFunction hmacSha512(java.security.Key);
  public static com.google.common.hash.HashFunction hmacSha512(byte[]);
  public static com.google.common.hash.HashFunction crc32c();
  public static com.google.common.hash.HashFunction crc32();
  public static com.google.common.hash.HashFunction adler32();
  public static com.google.common.hash.HashFunction farmHashFingerprint64();
  public static com.google.common.hash.HashFunction fingerprint2011();
  public static int consistentHash(com.google.common.hash.HashCode, int);
  public static int consistentHash(long, int);
  public static com.google.common.hash.HashCode combineOrdered(java.lang.Iterable<com.google.common.hash.HashCode>);
  public static com.google.common.hash.HashCode combineUnordered(java.lang.Iterable<com.google.common.hash.HashCode>);
  public static com.google.common.hash.HashFunction concatenating(com.google.common.hash.HashFunction, com.google.common.hash.HashFunction, com.google.common.hash.HashFunction...);
  public static com.google.common.hash.HashFunction concatenating(java.lang.Iterable<com.google.common.hash.HashFunction>);
}
```

## `com.google.common.hash.HashingInputStream`

```java
public final class com.google.common.hash.HashingInputStream extends java.io.FilterInputStream {
  public com.google.common.hash.HashingInputStream(com.google.common.hash.HashFunction, java.io.InputStream);
  public int read() throws java.io.IOException;
  public int read(byte[], int, int) throws java.io.IOException;
  public boolean markSupported();
  public void mark(int);
  public void reset() throws java.io.IOException;
  public com.google.common.hash.HashCode hash();
}
```

## `com.google.common.hash.HashingOutputStream`

```java
public final class com.google.common.hash.HashingOutputStream extends java.io.FilterOutputStream {
  public com.google.common.hash.HashingOutputStream(com.google.common.hash.HashFunction, java.io.OutputStream);
  public void write(int) throws java.io.IOException;
  public void write(byte[], int, int) throws java.io.IOException;
  public com.google.common.hash.HashCode hash();
  public void close() throws java.io.IOException;
}
```

## `com.google.common.hash.PrimitiveSink`

```java
public interface com.google.common.hash.PrimitiveSink {
  public abstract com.google.common.hash.PrimitiveSink putByte(byte);
  public abstract com.google.common.hash.PrimitiveSink putBytes(byte[]);
  public abstract com.google.common.hash.PrimitiveSink putBytes(byte[], int, int);
  public abstract com.google.common.hash.PrimitiveSink putBytes(java.nio.ByteBuffer);
  public abstract com.google.common.hash.PrimitiveSink putShort(short);
  public abstract com.google.common.hash.PrimitiveSink putInt(int);
  public abstract com.google.common.hash.PrimitiveSink putLong(long);
  public abstract com.google.common.hash.PrimitiveSink putFloat(float);
  public abstract com.google.common.hash.PrimitiveSink putDouble(double);
  public abstract com.google.common.hash.PrimitiveSink putBoolean(boolean);
  public abstract com.google.common.hash.PrimitiveSink putChar(char);
  public abstract com.google.common.hash.PrimitiveSink putUnencodedChars(java.lang.CharSequence);
  public abstract com.google.common.hash.PrimitiveSink putString(java.lang.CharSequence, java.nio.charset.Charset);
}
```
