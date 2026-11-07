# com.feilong.lib.org.apache.http.impl.io

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.impl.io.AbstractMessageParser`

```java
public abstract class com.feilong.lib.org.apache.http.impl.io.AbstractMessageParser<T extends com.feilong.lib.org.apache.http.HttpMessage> implements com.feilong.lib.org.apache.http.io.HttpMessageParser<T> {
  public com.feilong.lib.org.apache.http.impl.io.AbstractMessageParser(com.feilong.lib.org.apache.http.io.SessionInputBuffer, com.feilong.lib.org.apache.http.message.LineParser, com.feilong.lib.org.apache.http.config.MessageConstraints);
  public static com.feilong.lib.org.apache.http.Header[] parseHeaders(com.feilong.lib.org.apache.http.io.SessionInputBuffer, int, int, com.feilong.lib.org.apache.http.message.LineParser) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
  public static com.feilong.lib.org.apache.http.Header[] parseHeaders(com.feilong.lib.org.apache.http.io.SessionInputBuffer, int, int, com.feilong.lib.org.apache.http.message.LineParser, java.util.List<com.feilong.lib.org.apache.http.util.CharArrayBuffer>) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
  public T parse() throws java.io.IOException, com.feilong.lib.org.apache.http.HttpException;
}
```

## `com.feilong.lib.org.apache.http.impl.io.AbstractMessageWriter`

```java
public abstract class com.feilong.lib.org.apache.http.impl.io.AbstractMessageWriter<T extends com.feilong.lib.org.apache.http.HttpMessage> implements com.feilong.lib.org.apache.http.io.HttpMessageWriter<T> {
  public com.feilong.lib.org.apache.http.impl.io.AbstractMessageWriter(com.feilong.lib.org.apache.http.io.SessionOutputBuffer, com.feilong.lib.org.apache.http.message.LineFormatter, com.feilong.lib.org.apache.http.params.HttpParams);
  public com.feilong.lib.org.apache.http.impl.io.AbstractMessageWriter(com.feilong.lib.org.apache.http.io.SessionOutputBuffer, com.feilong.lib.org.apache.http.message.LineFormatter);
  public void write(T) throws java.io.IOException, com.feilong.lib.org.apache.http.HttpException;
}
```

## `com.feilong.lib.org.apache.http.impl.io.ChunkedInputStream`

```java
public class com.feilong.lib.org.apache.http.impl.io.ChunkedInputStream extends java.io.InputStream {
  public com.feilong.lib.org.apache.http.impl.io.ChunkedInputStream(com.feilong.lib.org.apache.http.io.SessionInputBuffer, com.feilong.lib.org.apache.http.config.MessageConstraints);
  public com.feilong.lib.org.apache.http.impl.io.ChunkedInputStream(com.feilong.lib.org.apache.http.io.SessionInputBuffer);
  public int available() throws java.io.IOException;
  public int read() throws java.io.IOException;
  public int read(byte[], int, int) throws java.io.IOException;
  public int read(byte[]) throws java.io.IOException;
  public void close() throws java.io.IOException;
  public com.feilong.lib.org.apache.http.Header[] getFooters();
}
```

## `com.feilong.lib.org.apache.http.impl.io.ChunkedOutputStream`

```java
public class com.feilong.lib.org.apache.http.impl.io.ChunkedOutputStream extends java.io.OutputStream {
  public com.feilong.lib.org.apache.http.impl.io.ChunkedOutputStream(com.feilong.lib.org.apache.http.io.SessionOutputBuffer, int) throws java.io.IOException;
  public com.feilong.lib.org.apache.http.impl.io.ChunkedOutputStream(com.feilong.lib.org.apache.http.io.SessionOutputBuffer) throws java.io.IOException;
  public com.feilong.lib.org.apache.http.impl.io.ChunkedOutputStream(int, com.feilong.lib.org.apache.http.io.SessionOutputBuffer);
  public void finish() throws java.io.IOException;
  public void write(int) throws java.io.IOException;
  public void write(byte[]) throws java.io.IOException;
  public void write(byte[], int, int) throws java.io.IOException;
  public void flush() throws java.io.IOException;
  public void close() throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.impl.io.ContentLengthInputStream`

```java
public class com.feilong.lib.org.apache.http.impl.io.ContentLengthInputStream extends java.io.InputStream {
  public com.feilong.lib.org.apache.http.impl.io.ContentLengthInputStream(com.feilong.lib.org.apache.http.io.SessionInputBuffer, long);
  public void close() throws java.io.IOException;
  public int available() throws java.io.IOException;
  public int read() throws java.io.IOException;
  public int read(byte[], int, int) throws java.io.IOException;
  public int read(byte[]) throws java.io.IOException;
  public long skip(long) throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.impl.io.ContentLengthOutputStream`

```java
public class com.feilong.lib.org.apache.http.impl.io.ContentLengthOutputStream extends java.io.OutputStream {
  public com.feilong.lib.org.apache.http.impl.io.ContentLengthOutputStream(com.feilong.lib.org.apache.http.io.SessionOutputBuffer, long);
  public void close() throws java.io.IOException;
  public void flush() throws java.io.IOException;
  public void write(byte[], int, int) throws java.io.IOException;
  public void write(byte[]) throws java.io.IOException;
  public void write(int) throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.impl.io.DefaultHttpRequestParser`

```java
public class com.feilong.lib.org.apache.http.impl.io.DefaultHttpRequestParser extends com.feilong.lib.org.apache.http.impl.io.AbstractMessageParser<com.feilong.lib.org.apache.http.HttpRequest> {
  public com.feilong.lib.org.apache.http.impl.io.DefaultHttpRequestParser(com.feilong.lib.org.apache.http.io.SessionInputBuffer, com.feilong.lib.org.apache.http.message.LineParser, com.feilong.lib.org.apache.http.HttpRequestFactory, com.feilong.lib.org.apache.http.config.MessageConstraints);
  public com.feilong.lib.org.apache.http.impl.io.DefaultHttpRequestParser(com.feilong.lib.org.apache.http.io.SessionInputBuffer, com.feilong.lib.org.apache.http.config.MessageConstraints);
  public com.feilong.lib.org.apache.http.impl.io.DefaultHttpRequestParser(com.feilong.lib.org.apache.http.io.SessionInputBuffer);
}
```

## `com.feilong.lib.org.apache.http.impl.io.DefaultHttpRequestParserFactory`

```java
public class com.feilong.lib.org.apache.http.impl.io.DefaultHttpRequestParserFactory implements com.feilong.lib.org.apache.http.io.HttpMessageParserFactory<com.feilong.lib.org.apache.http.HttpRequest> {
  public com.feilong.lib.org.apache.http.impl.io.DefaultHttpRequestParserFactory(com.feilong.lib.org.apache.http.message.LineParser, com.feilong.lib.org.apache.http.HttpRequestFactory);
  public com.feilong.lib.org.apache.http.impl.io.DefaultHttpRequestParserFactory();
  public com.feilong.lib.org.apache.http.io.HttpMessageParser<com.feilong.lib.org.apache.http.HttpRequest> create(com.feilong.lib.org.apache.http.io.SessionInputBuffer, com.feilong.lib.org.apache.http.config.MessageConstraints);
}
```

## `com.feilong.lib.org.apache.http.impl.io.DefaultHttpRequestWriter`

```java
public class com.feilong.lib.org.apache.http.impl.io.DefaultHttpRequestWriter extends com.feilong.lib.org.apache.http.impl.io.AbstractMessageWriter<com.feilong.lib.org.apache.http.HttpRequest> {
  public com.feilong.lib.org.apache.http.impl.io.DefaultHttpRequestWriter(com.feilong.lib.org.apache.http.io.SessionOutputBuffer, com.feilong.lib.org.apache.http.message.LineFormatter);
  public com.feilong.lib.org.apache.http.impl.io.DefaultHttpRequestWriter(com.feilong.lib.org.apache.http.io.SessionOutputBuffer);
}
```

## `com.feilong.lib.org.apache.http.impl.io.DefaultHttpRequestWriterFactory`

```java
public class com.feilong.lib.org.apache.http.impl.io.DefaultHttpRequestWriterFactory implements com.feilong.lib.org.apache.http.io.HttpMessageWriterFactory<com.feilong.lib.org.apache.http.HttpRequest> {
  public com.feilong.lib.org.apache.http.impl.io.DefaultHttpRequestWriterFactory(com.feilong.lib.org.apache.http.message.LineFormatter);
  public com.feilong.lib.org.apache.http.impl.io.DefaultHttpRequestWriterFactory();
  public com.feilong.lib.org.apache.http.io.HttpMessageWriter<com.feilong.lib.org.apache.http.HttpRequest> create(com.feilong.lib.org.apache.http.io.SessionOutputBuffer);
}
```

## `com.feilong.lib.org.apache.http.impl.io.DefaultHttpResponseParser`

```java
public class com.feilong.lib.org.apache.http.impl.io.DefaultHttpResponseParser extends com.feilong.lib.org.apache.http.impl.io.AbstractMessageParser<com.feilong.lib.org.apache.http.HttpResponse> {
  public com.feilong.lib.org.apache.http.impl.io.DefaultHttpResponseParser(com.feilong.lib.org.apache.http.io.SessionInputBuffer, com.feilong.lib.org.apache.http.message.LineParser, com.feilong.lib.org.apache.http.HttpResponseFactory, com.feilong.lib.org.apache.http.config.MessageConstraints);
  public com.feilong.lib.org.apache.http.impl.io.DefaultHttpResponseParser(com.feilong.lib.org.apache.http.io.SessionInputBuffer, com.feilong.lib.org.apache.http.config.MessageConstraints);
  public com.feilong.lib.org.apache.http.impl.io.DefaultHttpResponseParser(com.feilong.lib.org.apache.http.io.SessionInputBuffer);
}
```

## `com.feilong.lib.org.apache.http.impl.io.DefaultHttpResponseParserFactory`

```java
public class com.feilong.lib.org.apache.http.impl.io.DefaultHttpResponseParserFactory implements com.feilong.lib.org.apache.http.io.HttpMessageParserFactory<com.feilong.lib.org.apache.http.HttpResponse> {
  public com.feilong.lib.org.apache.http.impl.io.DefaultHttpResponseParserFactory(com.feilong.lib.org.apache.http.message.LineParser, com.feilong.lib.org.apache.http.HttpResponseFactory);
  public com.feilong.lib.org.apache.http.impl.io.DefaultHttpResponseParserFactory();
  public com.feilong.lib.org.apache.http.io.HttpMessageParser<com.feilong.lib.org.apache.http.HttpResponse> create(com.feilong.lib.org.apache.http.io.SessionInputBuffer, com.feilong.lib.org.apache.http.config.MessageConstraints);
}
```

## `com.feilong.lib.org.apache.http.impl.io.DefaultHttpResponseWriter`

```java
public class com.feilong.lib.org.apache.http.impl.io.DefaultHttpResponseWriter extends com.feilong.lib.org.apache.http.impl.io.AbstractMessageWriter<com.feilong.lib.org.apache.http.HttpResponse> {
  public com.feilong.lib.org.apache.http.impl.io.DefaultHttpResponseWriter(com.feilong.lib.org.apache.http.io.SessionOutputBuffer, com.feilong.lib.org.apache.http.message.LineFormatter);
  public com.feilong.lib.org.apache.http.impl.io.DefaultHttpResponseWriter(com.feilong.lib.org.apache.http.io.SessionOutputBuffer);
}
```

## `com.feilong.lib.org.apache.http.impl.io.DefaultHttpResponseWriterFactory`

```java
public class com.feilong.lib.org.apache.http.impl.io.DefaultHttpResponseWriterFactory implements com.feilong.lib.org.apache.http.io.HttpMessageWriterFactory<com.feilong.lib.org.apache.http.HttpResponse> {
  public com.feilong.lib.org.apache.http.impl.io.DefaultHttpResponseWriterFactory(com.feilong.lib.org.apache.http.message.LineFormatter);
  public com.feilong.lib.org.apache.http.impl.io.DefaultHttpResponseWriterFactory();
  public com.feilong.lib.org.apache.http.io.HttpMessageWriter<com.feilong.lib.org.apache.http.HttpResponse> create(com.feilong.lib.org.apache.http.io.SessionOutputBuffer);
}
```

## `com.feilong.lib.org.apache.http.impl.io.EmptyInputStream`

```java
public final class com.feilong.lib.org.apache.http.impl.io.EmptyInputStream extends java.io.InputStream {
  public int available();
  public void close();
  public void mark(int);
  public boolean markSupported();
  public int read();
  public int read(byte[]);
  public int read(byte[], int, int);
  public void reset();
  public long skip(long);
}
```

## `com.feilong.lib.org.apache.http.impl.io.HttpTransportMetricsImpl`

```java
public class com.feilong.lib.org.apache.http.impl.io.HttpTransportMetricsImpl implements com.feilong.lib.org.apache.http.io.HttpTransportMetrics {
  public com.feilong.lib.org.apache.http.impl.io.HttpTransportMetricsImpl();
  public long getBytesTransferred();
  public void setBytesTransferred(long);
  public void incrementBytesTransferred(long);
  public void reset();
}
```

## `com.feilong.lib.org.apache.http.impl.io.IdentityInputStream`

```java
public class com.feilong.lib.org.apache.http.impl.io.IdentityInputStream extends java.io.InputStream {
  public com.feilong.lib.org.apache.http.impl.io.IdentityInputStream(com.feilong.lib.org.apache.http.io.SessionInputBuffer);
  public int available() throws java.io.IOException;
  public void close() throws java.io.IOException;
  public int read() throws java.io.IOException;
  public int read(byte[], int, int) throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.impl.io.IdentityOutputStream`

```java
public class com.feilong.lib.org.apache.http.impl.io.IdentityOutputStream extends java.io.OutputStream {
  public com.feilong.lib.org.apache.http.impl.io.IdentityOutputStream(com.feilong.lib.org.apache.http.io.SessionOutputBuffer);
  public void close() throws java.io.IOException;
  public void flush() throws java.io.IOException;
  public void write(byte[], int, int) throws java.io.IOException;
  public void write(byte[]) throws java.io.IOException;
  public void write(int) throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.impl.io.SessionInputBufferImpl`

```java
public class com.feilong.lib.org.apache.http.impl.io.SessionInputBufferImpl implements com.feilong.lib.org.apache.http.io.SessionInputBuffer,com.feilong.lib.org.apache.http.io.BufferInfo {
  public com.feilong.lib.org.apache.http.impl.io.SessionInputBufferImpl(com.feilong.lib.org.apache.http.impl.io.HttpTransportMetricsImpl, int, int, com.feilong.lib.org.apache.http.config.MessageConstraints, java.nio.charset.CharsetDecoder);
  public com.feilong.lib.org.apache.http.impl.io.SessionInputBufferImpl(com.feilong.lib.org.apache.http.impl.io.HttpTransportMetricsImpl, int);
  public void bind(java.io.InputStream);
  public boolean isBound();
  public int capacity();
  public int length();
  public int available();
  public int fillBuffer() throws java.io.IOException;
  public boolean hasBufferedData();
  public void clear();
  public int read() throws java.io.IOException;
  public int read(byte[], int, int) throws java.io.IOException;
  public int read(byte[]) throws java.io.IOException;
  public int readLine(com.feilong.lib.org.apache.http.util.CharArrayBuffer) throws java.io.IOException;
  public java.lang.String readLine() throws java.io.IOException;
  public com.feilong.lib.org.apache.http.io.HttpTransportMetrics getMetrics();
}
```

## `com.feilong.lib.org.apache.http.impl.io.SessionOutputBufferImpl`

```java
public class com.feilong.lib.org.apache.http.impl.io.SessionOutputBufferImpl implements com.feilong.lib.org.apache.http.io.SessionOutputBuffer,com.feilong.lib.org.apache.http.io.BufferInfo {
  public com.feilong.lib.org.apache.http.impl.io.SessionOutputBufferImpl(com.feilong.lib.org.apache.http.impl.io.HttpTransportMetricsImpl, int, int, java.nio.charset.CharsetEncoder);
  public com.feilong.lib.org.apache.http.impl.io.SessionOutputBufferImpl(com.feilong.lib.org.apache.http.impl.io.HttpTransportMetricsImpl, int);
  public void bind(java.io.OutputStream);
  public boolean isBound();
  public int capacity();
  public int length();
  public int available();
  public void flush() throws java.io.IOException;
  public void write(byte[], int, int) throws java.io.IOException;
  public void write(byte[]) throws java.io.IOException;
  public void write(int) throws java.io.IOException;
  public void writeLine(java.lang.String) throws java.io.IOException;
  public void writeLine(com.feilong.lib.org.apache.http.util.CharArrayBuffer) throws java.io.IOException;
  public com.feilong.lib.org.apache.http.io.HttpTransportMetrics getMetrics();
}
```
