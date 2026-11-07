# com.feilong.context.fileparser

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.context.fileparser.FileParser`

```java
public interface com.feilong.context.fileparser.FileParser {
  public abstract void parse(java.lang.String);
}
```

## `com.feilong.context.fileparser.RequestFileParserDetector`

```java
public interface com.feilong.context.fileparser.RequestFileParserDetector {
  public abstract com.feilong.context.fileparser.FileParser detect(javax.servlet.http.HttpServletRequest);
}
```
