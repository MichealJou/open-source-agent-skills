# cn.hutool.core.io.resource

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.io.resource.BytesResource`

```java
public class cn.hutool.core.io.resource.BytesResource implements cn.hutool.core.io.resource.Resource,java.io.Serializable {
  public cn.hutool.core.io.resource.BytesResource(byte[]);
  public cn.hutool.core.io.resource.BytesResource(byte[], java.lang.String);
  public java.lang.String getName();
  public java.net.URL getUrl();
  public java.io.InputStream getStream();
  public java.lang.String readStr(java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public byte[] readBytes() throws cn.hutool.core.io.IORuntimeException;
}
```

## `cn.hutool.core.io.resource.CharSequenceResource`

```java
public class cn.hutool.core.io.resource.CharSequenceResource implements cn.hutool.core.io.resource.Resource,java.io.Serializable {
  public cn.hutool.core.io.resource.CharSequenceResource(java.lang.CharSequence);
  public cn.hutool.core.io.resource.CharSequenceResource(java.lang.CharSequence, java.lang.String);
  public cn.hutool.core.io.resource.CharSequenceResource(java.lang.CharSequence, java.lang.CharSequence, java.nio.charset.Charset);
  public java.lang.String getName();
  public java.net.URL getUrl();
  public java.io.InputStream getStream();
  public java.io.BufferedReader getReader(java.nio.charset.Charset);
  public java.lang.String readStr(java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public byte[] readBytes() throws cn.hutool.core.io.IORuntimeException;
}
```

## `cn.hutool.core.io.resource.ClassPathResource`

```java
public class cn.hutool.core.io.resource.ClassPathResource extends cn.hutool.core.io.resource.UrlResource {
  public cn.hutool.core.io.resource.ClassPathResource(java.lang.String);
  public cn.hutool.core.io.resource.ClassPathResource(java.lang.String, java.lang.ClassLoader);
  public cn.hutool.core.io.resource.ClassPathResource(java.lang.String, java.lang.Class<?>);
  public cn.hutool.core.io.resource.ClassPathResource(java.lang.String, java.lang.ClassLoader, java.lang.Class<?>);
  public final java.lang.String getPath();
  public final java.lang.String getAbsolutePath();
  public final java.lang.ClassLoader getClassLoader();
  public java.lang.String toString();
}
```

## `cn.hutool.core.io.resource.FileObjectResource`

```java
public class cn.hutool.core.io.resource.FileObjectResource implements cn.hutool.core.io.resource.Resource {
  public cn.hutool.core.io.resource.FileObjectResource(javax.tools.FileObject);
  public javax.tools.FileObject getFileObject();
  public java.lang.String getName();
  public java.net.URL getUrl();
  public java.io.InputStream getStream();
  public java.io.BufferedReader getReader(java.nio.charset.Charset);
}
```

## `cn.hutool.core.io.resource.FileResource`

```java
public class cn.hutool.core.io.resource.FileResource implements cn.hutool.core.io.resource.Resource,java.io.Serializable {
  public cn.hutool.core.io.resource.FileResource(java.lang.String);
  public cn.hutool.core.io.resource.FileResource(java.nio.file.Path);
  public cn.hutool.core.io.resource.FileResource(java.io.File);
  public cn.hutool.core.io.resource.FileResource(java.io.File, java.lang.String);
  public java.lang.String getName();
  public java.net.URL getUrl();
  public java.io.InputStream getStream() throws cn.hutool.core.io.resource.NoResourceException;
  public java.io.File getFile();
  public boolean isModified();
  public java.lang.String toString();
}
```

## `cn.hutool.core.io.resource.InputStreamResource`

```java
public class cn.hutool.core.io.resource.InputStreamResource implements cn.hutool.core.io.resource.Resource,java.io.Serializable {
  public cn.hutool.core.io.resource.InputStreamResource(java.io.InputStream);
  public cn.hutool.core.io.resource.InputStreamResource(java.io.InputStream, java.lang.String);
  public java.lang.String getName();
  public java.net.URL getUrl();
  public java.io.InputStream getStream();
}
```

## `cn.hutool.core.io.resource.MultiFileResource`

```java
public class cn.hutool.core.io.resource.MultiFileResource extends cn.hutool.core.io.resource.MultiResource {
  public cn.hutool.core.io.resource.MultiFileResource(java.util.Collection<java.io.File>);
  public cn.hutool.core.io.resource.MultiFileResource(java.io.File...);
  public cn.hutool.core.io.resource.MultiFileResource add(java.io.File...);
  public cn.hutool.core.io.resource.MultiFileResource add(java.util.Collection<java.io.File>);
  public cn.hutool.core.io.resource.MultiFileResource add(cn.hutool.core.io.resource.Resource);
  public cn.hutool.core.io.resource.MultiResource add(cn.hutool.core.io.resource.Resource);
}
```

## `cn.hutool.core.io.resource.MultiResource`

```java
public class cn.hutool.core.io.resource.MultiResource implements cn.hutool.core.io.resource.Resource, java.lang.Iterable<cn.hutool.core.io.resource.Resource>, java.util.Iterator<cn.hutool.core.io.resource.Resource>, java.io.Serializable {
  public cn.hutool.core.io.resource.MultiResource(cn.hutool.core.io.resource.Resource...);
  public cn.hutool.core.io.resource.MultiResource(java.util.Collection<cn.hutool.core.io.resource.Resource>);
  public java.lang.String getName();
  public java.net.URL getUrl();
  public java.io.InputStream getStream();
  public boolean isModified();
  public java.io.BufferedReader getReader(java.nio.charset.Charset);
  public java.lang.String readStr(java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public java.lang.String readUtf8Str() throws cn.hutool.core.io.IORuntimeException;
  public byte[] readBytes() throws cn.hutool.core.io.IORuntimeException;
  public java.util.Iterator<cn.hutool.core.io.resource.Resource> iterator();
  public boolean hasNext();
  public synchronized cn.hutool.core.io.resource.Resource next();
  public void remove();
  public synchronized void reset();
  public cn.hutool.core.io.resource.MultiResource add(cn.hutool.core.io.resource.Resource);
  public java.lang.Object next();
}
```

## `cn.hutool.core.io.resource.NoResourceException`

```java
public class cn.hutool.core.io.resource.NoResourceException extends cn.hutool.core.io.IORuntimeException {
  public cn.hutool.core.io.resource.NoResourceException(java.lang.Throwable);
  public cn.hutool.core.io.resource.NoResourceException(java.lang.String);
  public cn.hutool.core.io.resource.NoResourceException(java.lang.String, java.lang.Object...);
  public cn.hutool.core.io.resource.NoResourceException(java.lang.String, java.lang.Throwable);
  public cn.hutool.core.io.resource.NoResourceException(java.lang.Throwable, java.lang.String, java.lang.Object...);
  public boolean causeInstanceOf(java.lang.Class<? extends java.lang.Throwable>);
}
```

## `cn.hutool.core.io.resource.Resource`

```java
public interface cn.hutool.core.io.resource.Resource {
  public abstract java.lang.String getName();
  public abstract java.net.URL getUrl();
  public abstract java.io.InputStream getStream();
  public default boolean isModified();
  public default void writeTo(java.io.OutputStream) throws cn.hutool.core.io.IORuntimeException;
  public default java.io.BufferedReader getReader(java.nio.charset.Charset);
  public default java.lang.String readStr(java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public default java.lang.String readUtf8Str() throws cn.hutool.core.io.IORuntimeException;
  public default byte[] readBytes() throws cn.hutool.core.io.IORuntimeException;
}
```

## `cn.hutool.core.io.resource.ResourceUtil`

```java
public class cn.hutool.core.io.resource.ResourceUtil {
  public cn.hutool.core.io.resource.ResourceUtil();
  public static java.lang.String readUtf8Str(java.lang.String);
  public static java.lang.String readStr(java.lang.String, java.nio.charset.Charset);
  public static byte[] readBytes(java.lang.String);
  public static java.io.InputStream getStream(java.lang.String) throws cn.hutool.core.io.resource.NoResourceException;
  public static java.io.InputStream getStreamSafe(java.lang.String);
  public static java.io.BufferedReader getUtf8Reader(java.lang.String);
  public static java.io.BufferedReader getReader(java.lang.String, java.nio.charset.Charset);
  public static java.net.URL getResource(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.util.List<java.net.URL> getResources(java.lang.String);
  public static java.util.List<java.net.URL> getResources(java.lang.String, cn.hutool.core.lang.Filter<java.net.URL>);
  public static cn.hutool.core.collection.EnumerationIter<java.net.URL> getResourceIter(java.lang.String);
  public static cn.hutool.core.collection.EnumerationIter<java.net.URL> getResourceIter(java.lang.String, java.lang.ClassLoader);
  public static java.net.URL getResource(java.lang.String, java.lang.Class<?>);
  public static cn.hutool.core.io.resource.Resource getResourceObj(java.lang.String);
}
```

## `cn.hutool.core.io.resource.StringResource`

```java
public class cn.hutool.core.io.resource.StringResource extends cn.hutool.core.io.resource.CharSequenceResource {
  public cn.hutool.core.io.resource.StringResource(java.lang.String);
  public cn.hutool.core.io.resource.StringResource(java.lang.String, java.lang.String);
  public cn.hutool.core.io.resource.StringResource(java.lang.String, java.lang.String, java.nio.charset.Charset);
}
```

## `cn.hutool.core.io.resource.UrlResource`

```java
public class cn.hutool.core.io.resource.UrlResource implements cn.hutool.core.io.resource.Resource,java.io.Serializable {
  public cn.hutool.core.io.resource.UrlResource(java.net.URI);
  public cn.hutool.core.io.resource.UrlResource(java.net.URL);
  public cn.hutool.core.io.resource.UrlResource(java.net.URL, java.lang.String);
  public cn.hutool.core.io.resource.UrlResource(java.io.File);
  public java.lang.String getName();
  public java.net.URL getUrl();
  public java.io.InputStream getStream() throws cn.hutool.core.io.resource.NoResourceException;
  public boolean isModified();
  public java.io.File getFile();
  public java.lang.String toString();
  public long size();
}
```

## `cn.hutool.core.io.resource.VfsResource`

```java
public class cn.hutool.core.io.resource.VfsResource implements cn.hutool.core.io.resource.Resource {
  public cn.hutool.core.io.resource.VfsResource(java.lang.Object);
  public boolean exists();
  public java.lang.String getName();
  public java.net.URL getUrl();
  public java.io.InputStream getStream();
  public boolean isModified();
  public long getLastModified();
  public long size();
}
```

## `cn.hutool.core.io.resource.WebAppResource`

```java
public class cn.hutool.core.io.resource.WebAppResource extends cn.hutool.core.io.resource.FileResource {
  public cn.hutool.core.io.resource.WebAppResource(java.lang.String);
}
```
