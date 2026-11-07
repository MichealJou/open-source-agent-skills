# cn.hutool.extra.compress

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.compress.CompressException`

```java
public class cn.hutool.extra.compress.CompressException extends java.lang.RuntimeException {
  public cn.hutool.extra.compress.CompressException(java.lang.Throwable);
  public cn.hutool.extra.compress.CompressException(java.lang.String);
  public cn.hutool.extra.compress.CompressException(java.lang.String, java.lang.Object...);
  public cn.hutool.extra.compress.CompressException(java.lang.String, java.lang.Throwable);
  public cn.hutool.extra.compress.CompressException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.extra.compress.CompressException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.extra.compress.CompressUtil`

```java
public class cn.hutool.extra.compress.CompressUtil {
  public cn.hutool.extra.compress.CompressUtil();
  public static org.apache.commons.compress.compressors.CompressorOutputStream getOut(java.lang.String, java.io.OutputStream);
  public static org.apache.commons.compress.compressors.CompressorInputStream getIn(java.lang.String, java.io.InputStream);
  public static cn.hutool.extra.compress.archiver.Archiver createArchiver(java.nio.charset.Charset, java.lang.String, java.io.File);
  public static cn.hutool.extra.compress.archiver.Archiver createArchiver(java.nio.charset.Charset, java.lang.String, java.io.OutputStream);
  public static cn.hutool.extra.compress.extractor.Extractor createExtractor(java.nio.charset.Charset, java.io.File);
  public static cn.hutool.extra.compress.extractor.Extractor createExtractor(java.nio.charset.Charset, java.lang.String, java.io.File);
  public static cn.hutool.extra.compress.extractor.Extractor createExtractor(java.nio.charset.Charset, java.io.InputStream);
  public static cn.hutool.extra.compress.extractor.Extractor createExtractor(java.nio.charset.Charset, java.lang.String, java.io.InputStream);
}
```
