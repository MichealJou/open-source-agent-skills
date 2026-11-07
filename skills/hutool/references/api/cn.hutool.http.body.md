# cn.hutool.http.body

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.http.body.BytesBody`

```java
public class cn.hutool.http.body.BytesBody implements cn.hutool.http.body.RequestBody {
  public static cn.hutool.http.body.BytesBody create(byte[]);
  public cn.hutool.http.body.BytesBody(byte[]);
  public void write(java.io.OutputStream);
}
```

## `cn.hutool.http.body.FormUrlEncodedBody`

```java
public class cn.hutool.http.body.FormUrlEncodedBody extends cn.hutool.http.body.BytesBody {
  public static cn.hutool.http.body.FormUrlEncodedBody create(java.util.Map<java.lang.String, java.lang.Object>, java.nio.charset.Charset);
  public cn.hutool.http.body.FormUrlEncodedBody(java.util.Map<java.lang.String, java.lang.Object>, java.nio.charset.Charset);
  public java.lang.String toString();
}
```

## `cn.hutool.http.body.MultipartBody`

```java
public class cn.hutool.http.body.MultipartBody implements cn.hutool.http.body.RequestBody {
  public static cn.hutool.http.body.MultipartBody create(java.util.Map<java.lang.String, java.lang.Object>, java.nio.charset.Charset);
  public java.lang.String getContentType();
  public cn.hutool.http.body.MultipartBody(java.util.Map<java.lang.String, java.lang.Object>, java.nio.charset.Charset);
  public void write(java.io.OutputStream);
  public java.lang.String toString();
}
```

## `cn.hutool.http.body.RequestBody`

```java
public interface cn.hutool.http.body.RequestBody {
  public abstract void write(java.io.OutputStream);
  public default void writeClose(java.io.OutputStream);
}
```

## `cn.hutool.http.body.ResourceBody`

```java
public class cn.hutool.http.body.ResourceBody implements cn.hutool.http.body.RequestBody {
  public static cn.hutool.http.body.ResourceBody create(cn.hutool.core.io.resource.Resource);
  public cn.hutool.http.body.ResourceBody(cn.hutool.core.io.resource.Resource);
  public void write(java.io.OutputStream);
  public java.lang.String toString();
}
```
