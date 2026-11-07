# com.google.common.io

版本：33.4.8-jre。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.google.common.io.BaseEncoding`

```java
public abstract class com.google.common.io.BaseEncoding {
  public java.lang.String encode(byte[]);
  public final java.lang.String encode(byte[], int, int);
  public abstract java.io.OutputStream encodingStream(java.io.Writer);
  public final com.google.common.io.ByteSink encodingSink(com.google.common.io.CharSink);
  public abstract boolean canDecode(java.lang.CharSequence);
  public final byte[] decode(java.lang.CharSequence);
  public abstract java.io.InputStream decodingStream(java.io.Reader);
  public final com.google.common.io.ByteSource decodingSource(com.google.common.io.CharSource);
  public abstract com.google.common.io.BaseEncoding omitPadding();
  public abstract com.google.common.io.BaseEncoding withPadChar(char);
  public abstract com.google.common.io.BaseEncoding withSeparator(java.lang.String, int);
  public abstract com.google.common.io.BaseEncoding upperCase();
  public abstract com.google.common.io.BaseEncoding lowerCase();
  public abstract com.google.common.io.BaseEncoding ignoreCase();
  public static com.google.common.io.BaseEncoding base64();
  public static com.google.common.io.BaseEncoding base64Url();
  public static com.google.common.io.BaseEncoding base32();
  public static com.google.common.io.BaseEncoding base32Hex();
  public static com.google.common.io.BaseEncoding base16();
}
```

## `com.google.common.io.ByteArrayDataInput`

```java
public interface com.google.common.io.ByteArrayDataInput extends java.io.DataInput {
  public abstract void readFully(byte[]);
  public abstract void readFully(byte[], int, int);
  public abstract int skipBytes(int);
  public abstract boolean readBoolean();
  public abstract byte readByte();
  public abstract int readUnsignedByte();
  public abstract short readShort();
  public abstract int readUnsignedShort();
  public abstract char readChar();
  public abstract int readInt();
  public abstract long readLong();
  public abstract float readFloat();
  public abstract double readDouble();
  public abstract java.lang.String readLine();
  public abstract java.lang.String readUTF();
}
```

## `com.google.common.io.ByteArrayDataOutput`

```java
public interface com.google.common.io.ByteArrayDataOutput extends java.io.DataOutput {
  public abstract void write(int);
  public abstract void write(byte[]);
  public abstract void write(byte[], int, int);
  public abstract void writeBoolean(boolean);
  public abstract void writeByte(int);
  public abstract void writeShort(int);
  public abstract void writeChar(int);
  public abstract void writeInt(int);
  public abstract void writeLong(long);
  public abstract void writeFloat(float);
  public abstract void writeDouble(double);
  public abstract void writeChars(java.lang.String);
  public abstract void writeUTF(java.lang.String);
  public abstract void writeBytes(java.lang.String);
  public abstract byte[] toByteArray();
}
```

## `com.google.common.io.ByteProcessor`

```java
public interface com.google.common.io.ByteProcessor<T> {
  public abstract boolean processBytes(byte[], int, int) throws java.io.IOException;
  public abstract T getResult();
}
```

## `com.google.common.io.ByteSink`

```java
public abstract class com.google.common.io.ByteSink {
  public com.google.common.io.CharSink asCharSink(java.nio.charset.Charset);
  public abstract java.io.OutputStream openStream() throws java.io.IOException;
  public java.io.OutputStream openBufferedStream() throws java.io.IOException;
  public void write(byte[]) throws java.io.IOException;
  public long writeFrom(java.io.InputStream) throws java.io.IOException;
}
```

## `com.google.common.io.ByteSource`

```java
public abstract class com.google.common.io.ByteSource {
  public com.google.common.io.CharSource asCharSource(java.nio.charset.Charset);
  public abstract java.io.InputStream openStream() throws java.io.IOException;
  public java.io.InputStream openBufferedStream() throws java.io.IOException;
  public com.google.common.io.ByteSource slice(long, long);
  public boolean isEmpty() throws java.io.IOException;
  public com.google.common.base.Optional<java.lang.Long> sizeIfKnown();
  public long size() throws java.io.IOException;
  public long copyTo(java.io.OutputStream) throws java.io.IOException;
  public long copyTo(com.google.common.io.ByteSink) throws java.io.IOException;
  public byte[] read() throws java.io.IOException;
  public <T> T read(com.google.common.io.ByteProcessor<T>) throws java.io.IOException;
  public com.google.common.hash.HashCode hash(com.google.common.hash.HashFunction) throws java.io.IOException;
  public boolean contentEquals(com.google.common.io.ByteSource) throws java.io.IOException;
  public static com.google.common.io.ByteSource concat(java.lang.Iterable<? extends com.google.common.io.ByteSource>);
  public static com.google.common.io.ByteSource concat(java.util.Iterator<? extends com.google.common.io.ByteSource>);
  public static com.google.common.io.ByteSource concat(com.google.common.io.ByteSource...);
  public static com.google.common.io.ByteSource wrap(byte[]);
  public static com.google.common.io.ByteSource empty();
}
```

## `com.google.common.io.ByteStreams`

```java
public final class com.google.common.io.ByteStreams {
  public static long copy(java.io.InputStream, java.io.OutputStream) throws java.io.IOException;
  public static long copy(java.nio.channels.ReadableByteChannel, java.nio.channels.WritableByteChannel) throws java.io.IOException;
  public static byte[] toByteArray(java.io.InputStream) throws java.io.IOException;
  public static long exhaust(java.io.InputStream) throws java.io.IOException;
  public static com.google.common.io.ByteArrayDataInput newDataInput(byte[]);
  public static com.google.common.io.ByteArrayDataInput newDataInput(byte[], int);
  public static com.google.common.io.ByteArrayDataInput newDataInput(java.io.ByteArrayInputStream);
  public static com.google.common.io.ByteArrayDataOutput newDataOutput();
  public static com.google.common.io.ByteArrayDataOutput newDataOutput(int);
  public static com.google.common.io.ByteArrayDataOutput newDataOutput(java.io.ByteArrayOutputStream);
  public static java.io.OutputStream nullOutputStream();
  public static java.io.InputStream limit(java.io.InputStream, long);
  public static void readFully(java.io.InputStream, byte[]) throws java.io.IOException;
  public static void readFully(java.io.InputStream, byte[], int, int) throws java.io.IOException;
  public static void skipFully(java.io.InputStream, long) throws java.io.IOException;
  public static <T> T readBytes(java.io.InputStream, com.google.common.io.ByteProcessor<T>) throws java.io.IOException;
  public static int read(java.io.InputStream, byte[], int, int) throws java.io.IOException;
}
```

## `com.google.common.io.CharSink`

```java
public abstract class com.google.common.io.CharSink {
  public abstract java.io.Writer openStream() throws java.io.IOException;
  public java.io.Writer openBufferedStream() throws java.io.IOException;
  public void write(java.lang.CharSequence) throws java.io.IOException;
  public void writeLines(java.lang.Iterable<? extends java.lang.CharSequence>) throws java.io.IOException;
  public void writeLines(java.lang.Iterable<? extends java.lang.CharSequence>, java.lang.String) throws java.io.IOException;
  public void writeLines(java.util.stream.Stream<? extends java.lang.CharSequence>) throws java.io.IOException;
  public void writeLines(java.util.stream.Stream<? extends java.lang.CharSequence>, java.lang.String) throws java.io.IOException;
  public long writeFrom(java.lang.Readable) throws java.io.IOException;
}
```

## `com.google.common.io.CharSource`

```java
public abstract class com.google.common.io.CharSource {
  public com.google.common.io.ByteSource asByteSource(java.nio.charset.Charset);
  public abstract java.io.Reader openStream() throws java.io.IOException;
  public java.io.BufferedReader openBufferedStream() throws java.io.IOException;
  public java.util.stream.Stream<java.lang.String> lines() throws java.io.IOException;
  public com.google.common.base.Optional<java.lang.Long> lengthIfKnown();
  public long length() throws java.io.IOException;
  public long copyTo(java.lang.Appendable) throws java.io.IOException;
  public long copyTo(com.google.common.io.CharSink) throws java.io.IOException;
  public java.lang.String read() throws java.io.IOException;
  public java.lang.String readFirstLine() throws java.io.IOException;
  public com.google.common.collect.ImmutableList<java.lang.String> readLines() throws java.io.IOException;
  public <T> T readLines(com.google.common.io.LineProcessor<T>) throws java.io.IOException;
  public void forEachLine(java.util.function.Consumer<? super java.lang.String>) throws java.io.IOException;
  public boolean isEmpty() throws java.io.IOException;
  public static com.google.common.io.CharSource concat(java.lang.Iterable<? extends com.google.common.io.CharSource>);
  public static com.google.common.io.CharSource concat(java.util.Iterator<? extends com.google.common.io.CharSource>);
  public static com.google.common.io.CharSource concat(com.google.common.io.CharSource...);
  public static com.google.common.io.CharSource wrap(java.lang.CharSequence);
  public static com.google.common.io.CharSource empty();
}
```

## `com.google.common.io.CharStreams`

```java
public final class com.google.common.io.CharStreams {
  public static long copy(java.lang.Readable, java.lang.Appendable) throws java.io.IOException;
  public static java.lang.String toString(java.lang.Readable) throws java.io.IOException;
  public static java.util.List<java.lang.String> readLines(java.lang.Readable) throws java.io.IOException;
  public static <T> T readLines(java.lang.Readable, com.google.common.io.LineProcessor<T>) throws java.io.IOException;
  public static long exhaust(java.lang.Readable) throws java.io.IOException;
  public static void skipFully(java.io.Reader, long) throws java.io.IOException;
  public static java.io.Writer nullWriter();
  public static java.io.Writer asWriter(java.lang.Appendable);
}
```

## `com.google.common.io.Closeables`

```java
public final class com.google.common.io.Closeables {
  public static void close(java.io.Closeable, boolean) throws java.io.IOException;
  public static void closeQuietly(java.io.InputStream);
  public static void closeQuietly(java.io.Reader);
}
```

## `com.google.common.io.Closer`

```java
public final class com.google.common.io.Closer implements java.io.Closeable {
  public static com.google.common.io.Closer create();
  public <C extends java.io.Closeable> C register(C);
  public java.lang.RuntimeException rethrow(java.lang.Throwable) throws java.io.IOException;
  public <X extends java.lang.Exception> java.lang.RuntimeException rethrow(java.lang.Throwable, java.lang.Class<X>) throws java.io.IOException, X;
  public <X1 extends java.lang.Exception, X2 extends java.lang.Exception> java.lang.RuntimeException rethrow(java.lang.Throwable, java.lang.Class<X1>, java.lang.Class<X2>) throws java.io.IOException, X1, X2;
  public void close() throws java.io.IOException;
}
```

## `com.google.common.io.CountingInputStream`

```java
public final class com.google.common.io.CountingInputStream extends java.io.FilterInputStream {
  public com.google.common.io.CountingInputStream(java.io.InputStream);
  public long getCount();
  public int read() throws java.io.IOException;
  public int read(byte[], int, int) throws java.io.IOException;
  public long skip(long) throws java.io.IOException;
  public synchronized void mark(int);
  public synchronized void reset() throws java.io.IOException;
}
```

## `com.google.common.io.CountingOutputStream`

```java
public final class com.google.common.io.CountingOutputStream extends java.io.FilterOutputStream {
  public com.google.common.io.CountingOutputStream(java.io.OutputStream);
  public long getCount();
  public void write(byte[], int, int) throws java.io.IOException;
  public void write(int) throws java.io.IOException;
  public void close() throws java.io.IOException;
}
```

## `com.google.common.io.FileBackedOutputStream`

```java
public final class com.google.common.io.FileBackedOutputStream extends java.io.OutputStream {
  public com.google.common.io.FileBackedOutputStream(int);
  public com.google.common.io.FileBackedOutputStream(int, boolean);
  public com.google.common.io.ByteSource asByteSource();
  public synchronized void reset() throws java.io.IOException;
  public synchronized void write(int) throws java.io.IOException;
  public synchronized void write(byte[]) throws java.io.IOException;
  public synchronized void write(byte[], int, int) throws java.io.IOException;
  public synchronized void close() throws java.io.IOException;
  public synchronized void flush() throws java.io.IOException;
}
```

## `com.google.common.io.FileWriteMode`

```java
public final class com.google.common.io.FileWriteMode extends java.lang.Enum<com.google.common.io.FileWriteMode> {
  public static com.google.common.io.FileWriteMode[] values();
  public static com.google.common.io.FileWriteMode valueOf(java.lang.String);
}
```

## `com.google.common.io.Files`

```java
public final class com.google.common.io.Files {
  public static java.io.BufferedReader newReader(java.io.File, java.nio.charset.Charset) throws java.io.FileNotFoundException;
  public static java.io.BufferedWriter newWriter(java.io.File, java.nio.charset.Charset) throws java.io.FileNotFoundException;
  public static com.google.common.io.ByteSource asByteSource(java.io.File);
  public static com.google.common.io.ByteSink asByteSink(java.io.File, com.google.common.io.FileWriteMode...);
  public static com.google.common.io.CharSource asCharSource(java.io.File, java.nio.charset.Charset);
  public static com.google.common.io.CharSink asCharSink(java.io.File, java.nio.charset.Charset, com.google.common.io.FileWriteMode...);
  public static byte[] toByteArray(java.io.File) throws java.io.IOException;
  public static java.lang.String toString(java.io.File, java.nio.charset.Charset) throws java.io.IOException;
  public static void write(byte[], java.io.File) throws java.io.IOException;
  public static void write(java.lang.CharSequence, java.io.File, java.nio.charset.Charset) throws java.io.IOException;
  public static void copy(java.io.File, java.io.OutputStream) throws java.io.IOException;
  public static void copy(java.io.File, java.io.File) throws java.io.IOException;
  public static void copy(java.io.File, java.nio.charset.Charset, java.lang.Appendable) throws java.io.IOException;
  public static void append(java.lang.CharSequence, java.io.File, java.nio.charset.Charset) throws java.io.IOException;
  public static boolean equal(java.io.File, java.io.File) throws java.io.IOException;
  public static java.io.File createTempDir();
  public static void touch(java.io.File) throws java.io.IOException;
  public static void createParentDirs(java.io.File) throws java.io.IOException;
  public static void move(java.io.File, java.io.File) throws java.io.IOException;
  public static java.lang.String readFirstLine(java.io.File, java.nio.charset.Charset) throws java.io.IOException;
  public static java.util.List<java.lang.String> readLines(java.io.File, java.nio.charset.Charset) throws java.io.IOException;
  public static <T> T readLines(java.io.File, java.nio.charset.Charset, com.google.common.io.LineProcessor<T>) throws java.io.IOException;
  public static <T> T readBytes(java.io.File, com.google.common.io.ByteProcessor<T>) throws java.io.IOException;
  public static com.google.common.hash.HashCode hash(java.io.File, com.google.common.hash.HashFunction) throws java.io.IOException;
  public static java.nio.MappedByteBuffer map(java.io.File) throws java.io.IOException;
  public static java.nio.MappedByteBuffer map(java.io.File, java.nio.channels.FileChannel$MapMode) throws java.io.IOException;
  public static java.nio.MappedByteBuffer map(java.io.File, java.nio.channels.FileChannel$MapMode, long) throws java.io.IOException;
  public static java.lang.String simplifyPath(java.lang.String);
  public static java.lang.String getFileExtension(java.lang.String);
  public static java.lang.String getNameWithoutExtension(java.lang.String);
  public static com.google.common.graph.Traverser<java.io.File> fileTraverser();
  public static com.google.common.base.Predicate<java.io.File> isDirectory();
  public static com.google.common.base.Predicate<java.io.File> isFile();
}
```

## `com.google.common.io.Flushables`

```java
public final class com.google.common.io.Flushables {
  public static void flush(java.io.Flushable, boolean) throws java.io.IOException;
  public static void flushQuietly(java.io.Flushable);
}
```

## `com.google.common.io.InsecureRecursiveDeleteException`

```java
public final class com.google.common.io.InsecureRecursiveDeleteException extends java.nio.file.FileSystemException {
  public com.google.common.io.InsecureRecursiveDeleteException(java.lang.String);
}
```

## `com.google.common.io.LineProcessor`

```java
public interface com.google.common.io.LineProcessor<T> {
  public abstract boolean processLine(java.lang.String) throws java.io.IOException;
  public abstract T getResult();
}
```

## `com.google.common.io.LineReader`

```java
public final class com.google.common.io.LineReader {
  public com.google.common.io.LineReader(java.lang.Readable);
  public java.lang.String readLine() throws java.io.IOException;
}
```

## `com.google.common.io.LittleEndianDataInputStream`

```java
public final class com.google.common.io.LittleEndianDataInputStream extends java.io.FilterInputStream implements java.io.DataInput {
  public com.google.common.io.LittleEndianDataInputStream(java.io.InputStream);
  public java.lang.String readLine();
  public void readFully(byte[]) throws java.io.IOException;
  public void readFully(byte[], int, int) throws java.io.IOException;
  public int skipBytes(int) throws java.io.IOException;
  public int readUnsignedByte() throws java.io.IOException;
  public int readUnsignedShort() throws java.io.IOException;
  public int readInt() throws java.io.IOException;
  public long readLong() throws java.io.IOException;
  public float readFloat() throws java.io.IOException;
  public double readDouble() throws java.io.IOException;
  public java.lang.String readUTF() throws java.io.IOException;
  public short readShort() throws java.io.IOException;
  public char readChar() throws java.io.IOException;
  public byte readByte() throws java.io.IOException;
  public boolean readBoolean() throws java.io.IOException;
}
```

## `com.google.common.io.LittleEndianDataOutputStream`

```java
public final class com.google.common.io.LittleEndianDataOutputStream extends java.io.FilterOutputStream implements java.io.DataOutput {
  public com.google.common.io.LittleEndianDataOutputStream(java.io.OutputStream);
  public void write(byte[], int, int) throws java.io.IOException;
  public void writeBoolean(boolean) throws java.io.IOException;
  public void writeByte(int) throws java.io.IOException;
  public void writeBytes(java.lang.String) throws java.io.IOException;
  public void writeChar(int) throws java.io.IOException;
  public void writeChars(java.lang.String) throws java.io.IOException;
  public void writeDouble(double) throws java.io.IOException;
  public void writeFloat(float) throws java.io.IOException;
  public void writeInt(int) throws java.io.IOException;
  public void writeLong(long) throws java.io.IOException;
  public void writeShort(int) throws java.io.IOException;
  public void writeUTF(java.lang.String) throws java.io.IOException;
  public void close() throws java.io.IOException;
}
```

## `com.google.common.io.MoreFiles`

```java
public final class com.google.common.io.MoreFiles {
  public static com.google.common.io.ByteSource asByteSource(java.nio.file.Path, java.nio.file.OpenOption...);
  public static com.google.common.io.ByteSink asByteSink(java.nio.file.Path, java.nio.file.OpenOption...);
  public static com.google.common.io.CharSource asCharSource(java.nio.file.Path, java.nio.charset.Charset, java.nio.file.OpenOption...);
  public static com.google.common.io.CharSink asCharSink(java.nio.file.Path, java.nio.charset.Charset, java.nio.file.OpenOption...);
  public static com.google.common.collect.ImmutableList<java.nio.file.Path> listFiles(java.nio.file.Path) throws java.io.IOException;
  public static com.google.common.graph.Traverser<java.nio.file.Path> fileTraverser();
  public static com.google.common.base.Predicate<java.nio.file.Path> isDirectory(java.nio.file.LinkOption...);
  public static com.google.common.base.Predicate<java.nio.file.Path> isRegularFile(java.nio.file.LinkOption...);
  public static boolean equal(java.nio.file.Path, java.nio.file.Path) throws java.io.IOException;
  public static void touch(java.nio.file.Path) throws java.io.IOException;
  public static void createParentDirectories(java.nio.file.Path, java.nio.file.attribute.FileAttribute<?>...) throws java.io.IOException;
  public static java.lang.String getFileExtension(java.nio.file.Path);
  public static java.lang.String getNameWithoutExtension(java.nio.file.Path);
  public static void deleteRecursively(java.nio.file.Path, com.google.common.io.RecursiveDeleteOption...) throws java.io.IOException;
  public static void deleteDirectoryContents(java.nio.file.Path, com.google.common.io.RecursiveDeleteOption...) throws java.io.IOException;
}
```

## `com.google.common.io.PatternFilenameFilter`

```java
public final class com.google.common.io.PatternFilenameFilter implements java.io.FilenameFilter {
  public com.google.common.io.PatternFilenameFilter(java.lang.String);
  public com.google.common.io.PatternFilenameFilter(java.util.regex.Pattern);
  public boolean accept(java.io.File, java.lang.String);
}
```

## `com.google.common.io.RecursiveDeleteOption`

```java
public final class com.google.common.io.RecursiveDeleteOption extends java.lang.Enum<com.google.common.io.RecursiveDeleteOption> {
  public static com.google.common.io.RecursiveDeleteOption[] values();
  public static com.google.common.io.RecursiveDeleteOption valueOf(java.lang.String);
}
```

## `com.google.common.io.Resources`

```java
public final class com.google.common.io.Resources {
  public static com.google.common.io.ByteSource asByteSource(java.net.URL);
  public static com.google.common.io.CharSource asCharSource(java.net.URL, java.nio.charset.Charset);
  public static byte[] toByteArray(java.net.URL) throws java.io.IOException;
  public static java.lang.String toString(java.net.URL, java.nio.charset.Charset) throws java.io.IOException;
  public static <T> T readLines(java.net.URL, java.nio.charset.Charset, com.google.common.io.LineProcessor<T>) throws java.io.IOException;
  public static java.util.List<java.lang.String> readLines(java.net.URL, java.nio.charset.Charset) throws java.io.IOException;
  public static void copy(java.net.URL, java.io.OutputStream) throws java.io.IOException;
  public static java.net.URL getResource(java.lang.String);
  public static java.net.URL getResource(java.lang.Class<?>, java.lang.String);
}
```
