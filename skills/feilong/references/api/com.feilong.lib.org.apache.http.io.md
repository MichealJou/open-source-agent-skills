# com.feilong.lib.org.apache.http.io

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.io.BufferInfo`

```java
public interface com.feilong.lib.org.apache.http.io.BufferInfo {
  public abstract int length();
  public abstract int capacity();
  public abstract int available();
}
```

## `com.feilong.lib.org.apache.http.io.HttpMessageParser`

```java
public interface com.feilong.lib.org.apache.http.io.HttpMessageParser<T extends com.feilong.lib.org.apache.http.HttpMessage> {
  public abstract T parse() throws java.io.IOException, com.feilong.lib.org.apache.http.HttpException;
}
```

## `com.feilong.lib.org.apache.http.io.HttpMessageParserFactory`

```java
public interface com.feilong.lib.org.apache.http.io.HttpMessageParserFactory<T extends com.feilong.lib.org.apache.http.HttpMessage> {
  public abstract com.feilong.lib.org.apache.http.io.HttpMessageParser<T> create(com.feilong.lib.org.apache.http.io.SessionInputBuffer, com.feilong.lib.org.apache.http.config.MessageConstraints);
}
```

## `com.feilong.lib.org.apache.http.io.HttpMessageWriter`

```java
public interface com.feilong.lib.org.apache.http.io.HttpMessageWriter<T extends com.feilong.lib.org.apache.http.HttpMessage> {
  public abstract void write(T) throws java.io.IOException, com.feilong.lib.org.apache.http.HttpException;
}
```

## `com.feilong.lib.org.apache.http.io.HttpMessageWriterFactory`

```java
public interface com.feilong.lib.org.apache.http.io.HttpMessageWriterFactory<T extends com.feilong.lib.org.apache.http.HttpMessage> {
  public abstract com.feilong.lib.org.apache.http.io.HttpMessageWriter<T> create(com.feilong.lib.org.apache.http.io.SessionOutputBuffer);
}
```

## `com.feilong.lib.org.apache.http.io.HttpTransportMetrics`

```java
public interface com.feilong.lib.org.apache.http.io.HttpTransportMetrics {
  public abstract long getBytesTransferred();
  public abstract void reset();
}
```

## `com.feilong.lib.org.apache.http.io.SessionInputBuffer`

```java
public interface com.feilong.lib.org.apache.http.io.SessionInputBuffer {
  public abstract int read(byte[], int, int) throws java.io.IOException;
  public abstract int read(byte[]) throws java.io.IOException;
  public abstract int read() throws java.io.IOException;
  public abstract int readLine(com.feilong.lib.org.apache.http.util.CharArrayBuffer) throws java.io.IOException;
  public abstract java.lang.String readLine() throws java.io.IOException;
  public abstract com.feilong.lib.org.apache.http.io.HttpTransportMetrics getMetrics();
}
```

## `com.feilong.lib.org.apache.http.io.SessionOutputBuffer`

```java
public interface com.feilong.lib.org.apache.http.io.SessionOutputBuffer {
  public abstract void write(byte[], int, int) throws java.io.IOException;
  public abstract void write(byte[]) throws java.io.IOException;
  public abstract void write(int) throws java.io.IOException;
  public abstract void writeLine(java.lang.String) throws java.io.IOException;
  public abstract void writeLine(com.feilong.lib.org.apache.http.util.CharArrayBuffer) throws java.io.IOException;
  public abstract void flush() throws java.io.IOException;
  public abstract com.feilong.lib.org.apache.http.io.HttpTransportMetrics getMetrics();
}
```
