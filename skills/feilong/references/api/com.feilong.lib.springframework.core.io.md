# com.feilong.lib.springframework.core.io

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.springframework.core.io.AbstractFileResolvingResource`

```java
public abstract class com.feilong.lib.springframework.core.io.AbstractFileResolvingResource extends com.feilong.lib.springframework.core.io.AbstractResource {
  public com.feilong.lib.springframework.core.io.AbstractFileResolvingResource();
  public java.io.File getFile() throws java.io.IOException;
  public boolean exists();
  public boolean isReadable();
  public long contentLength() throws java.io.IOException;
  public long lastModified() throws java.io.IOException;
}
```

## `com.feilong.lib.springframework.core.io.AbstractResource`

```java
public abstract class com.feilong.lib.springframework.core.io.AbstractResource implements com.feilong.lib.springframework.core.io.Resource {
  public com.feilong.lib.springframework.core.io.AbstractResource();
  public boolean exists();
  public boolean isReadable();
  public boolean isOpen();
  public java.net.URL getURL() throws java.io.IOException;
  public java.net.URI getURI() throws java.io.IOException;
  public java.io.File getFile() throws java.io.IOException;
  public long contentLength() throws java.io.IOException;
  public long lastModified() throws java.io.IOException;
  public com.feilong.lib.springframework.core.io.Resource createRelative(java.lang.String) throws java.io.IOException;
  public java.lang.String getFilename();
  public java.lang.String toString();
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```

## `com.feilong.lib.springframework.core.io.ClassPathResource`

```java
public class com.feilong.lib.springframework.core.io.ClassPathResource extends com.feilong.lib.springframework.core.io.AbstractFileResolvingResource {
  public com.feilong.lib.springframework.core.io.ClassPathResource(java.lang.String);
  public com.feilong.lib.springframework.core.io.ClassPathResource(java.lang.String, java.lang.ClassLoader);
  public com.feilong.lib.springframework.core.io.ClassPathResource(java.lang.String, java.lang.Class<?>);
  public final java.lang.String getPath();
  public final java.lang.ClassLoader getClassLoader();
  public boolean exists();
  public java.io.InputStream getInputStream() throws java.io.IOException;
  public java.net.URL getURL() throws java.io.IOException;
  public com.feilong.lib.springframework.core.io.Resource createRelative(java.lang.String);
  public java.lang.String getFilename();
  public java.lang.String getDescription();
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```

## `com.feilong.lib.springframework.core.io.ContextResource`

```java
public interface com.feilong.lib.springframework.core.io.ContextResource extends com.feilong.lib.springframework.core.io.Resource {
  public abstract java.lang.String getPathWithinContext();
}
```

## `com.feilong.lib.springframework.core.io.DefaultResourceLoader`

```java
public class com.feilong.lib.springframework.core.io.DefaultResourceLoader implements com.feilong.lib.springframework.core.io.ResourceLoader {
  public com.feilong.lib.springframework.core.io.DefaultResourceLoader();
  public com.feilong.lib.springframework.core.io.DefaultResourceLoader(java.lang.ClassLoader);
  public void setClassLoader(java.lang.ClassLoader);
  public java.lang.ClassLoader getClassLoader();
  public void addProtocolResolver(com.feilong.lib.springframework.core.io.ProtocolResolver);
  public java.util.Collection<com.feilong.lib.springframework.core.io.ProtocolResolver> getProtocolResolvers();
  public com.feilong.lib.springframework.core.io.Resource getResource(java.lang.String);
}
```

## `com.feilong.lib.springframework.core.io.DefaultResourceLoader$ClassPathContextResource`

```java
public class com.feilong.lib.springframework.core.io.DefaultResourceLoader$ClassPathContextResource extends com.feilong.lib.springframework.core.io.ClassPathResource implements com.feilong.lib.springframework.core.io.ContextResource {
  public com.feilong.lib.springframework.core.io.DefaultResourceLoader$ClassPathContextResource(java.lang.String, java.lang.ClassLoader);
  public java.lang.String getPathWithinContext();
  public com.feilong.lib.springframework.core.io.Resource createRelative(java.lang.String);
}
```

## `com.feilong.lib.springframework.core.io.InputStreamSource`

```java
public interface com.feilong.lib.springframework.core.io.InputStreamSource {
  public abstract java.io.InputStream getInputStream() throws java.io.IOException;
}
```

## `com.feilong.lib.springframework.core.io.ProtocolResolver`

```java
public interface com.feilong.lib.springframework.core.io.ProtocolResolver {
  public abstract com.feilong.lib.springframework.core.io.Resource resolve(java.lang.String, com.feilong.lib.springframework.core.io.ResourceLoader);
}
```

## `com.feilong.lib.springframework.core.io.Resource`

```java
public interface com.feilong.lib.springframework.core.io.Resource extends com.feilong.lib.springframework.core.io.InputStreamSource {
  public abstract boolean exists();
  public abstract boolean isReadable();
  public abstract boolean isOpen();
  public abstract java.net.URL getURL() throws java.io.IOException;
  public abstract java.net.URI getURI() throws java.io.IOException;
  public abstract java.io.File getFile() throws java.io.IOException;
  public abstract long contentLength() throws java.io.IOException;
  public abstract long lastModified() throws java.io.IOException;
  public abstract com.feilong.lib.springframework.core.io.Resource createRelative(java.lang.String) throws java.io.IOException;
  public abstract java.lang.String getFilename();
  public abstract java.lang.String getDescription();
}
```

## `com.feilong.lib.springframework.core.io.ResourceLoader`

```java
public interface com.feilong.lib.springframework.core.io.ResourceLoader {
  public abstract com.feilong.lib.springframework.core.io.Resource getResource(java.lang.String);
  public abstract java.lang.ClassLoader getClassLoader();
}
```

## `com.feilong.lib.springframework.core.io.UrlResource`

```java
public class com.feilong.lib.springframework.core.io.UrlResource extends com.feilong.lib.springframework.core.io.AbstractFileResolvingResource {
  public com.feilong.lib.springframework.core.io.UrlResource(java.net.URI) throws java.net.MalformedURLException;
  public com.feilong.lib.springframework.core.io.UrlResource(java.net.URL);
  public com.feilong.lib.springframework.core.io.UrlResource(java.lang.String) throws java.net.MalformedURLException;
  public com.feilong.lib.springframework.core.io.UrlResource(java.lang.String, java.lang.String) throws java.net.MalformedURLException;
  public com.feilong.lib.springframework.core.io.UrlResource(java.lang.String, java.lang.String, java.lang.String) throws java.net.MalformedURLException;
  public java.io.InputStream getInputStream() throws java.io.IOException;
  public java.net.URL getURL() throws java.io.IOException;
  public java.net.URI getURI() throws java.io.IOException;
  public java.io.File getFile() throws java.io.IOException;
  public com.feilong.lib.springframework.core.io.Resource createRelative(java.lang.String) throws java.net.MalformedURLException;
  public java.lang.String getFilename();
  public java.lang.String getDescription();
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```

## `com.feilong.lib.springframework.core.io.VfsResource`

```java
public class com.feilong.lib.springframework.core.io.VfsResource extends com.feilong.lib.springframework.core.io.AbstractResource {
  public com.feilong.lib.springframework.core.io.VfsResource(java.lang.Object);
  public java.io.InputStream getInputStream() throws java.io.IOException;
  public boolean exists();
  public boolean isReadable();
  public java.net.URL getURL() throws java.io.IOException;
  public java.net.URI getURI() throws java.io.IOException;
  public java.io.File getFile() throws java.io.IOException;
  public long contentLength() throws java.io.IOException;
  public long lastModified() throws java.io.IOException;
  public com.feilong.lib.springframework.core.io.Resource createRelative(java.lang.String) throws java.io.IOException;
  public java.lang.String getFilename();
  public java.lang.String getDescription();
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```

## `com.feilong.lib.springframework.core.io.VfsUtils`

```java
public abstract class com.feilong.lib.springframework.core.io.VfsUtils {
  public com.feilong.lib.springframework.core.io.VfsUtils();
}
```
