# com.baomidou.mybatisplus.extension.parser

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.extension.parser.JsqlParserFunction`

```java
public interface com.baomidou.mybatisplus.extension.parser.JsqlParserFunction<T, R> {
  public abstract R apply(T) throws net.sf.jsqlparser.JSQLParserException;
}
```

## `com.baomidou.mybatisplus.extension.parser.JsqlParserGlobal`

```java
public class com.baomidou.mybatisplus.extension.parser.JsqlParserGlobal {
  public com.baomidou.mybatisplus.extension.parser.JsqlParserGlobal();
  public static void setExecutorService(java.util.concurrent.ExecutorService);
  public static void setExecutorService(java.util.concurrent.ExecutorService, boolean);
  public static void setExecutorService(java.util.concurrent.ExecutorService, java.lang.Thread);
  public static java.util.concurrent.ExecutorService getExecutorService();
  public static net.sf.jsqlparser.statement.Statement parse(java.lang.String) throws net.sf.jsqlparser.JSQLParserException;
  public static net.sf.jsqlparser.statement.Statements parseStatements(java.lang.String) throws net.sf.jsqlparser.JSQLParserException;
  public static void setParserSingleFunc(com.baomidou.mybatisplus.extension.parser.JsqlParserFunction<java.lang.String, net.sf.jsqlparser.statement.Statement>);
  public static void setParserMultiFunc(com.baomidou.mybatisplus.extension.parser.JsqlParserFunction<java.lang.String, net.sf.jsqlparser.statement.Statements>);
  public static void setJsqlParseCache(com.baomidou.mybatisplus.extension.parser.cache.JsqlParseCache);
}
```

## `com.baomidou.mybatisplus.extension.parser.JsqlParserSupport`

```java
public abstract class com.baomidou.mybatisplus.extension.parser.JsqlParserSupport {
  public com.baomidou.mybatisplus.extension.parser.JsqlParserSupport();
  public java.lang.String parserSingle(java.lang.String, java.lang.Object);
  public java.lang.String parserMulti(java.lang.String, java.lang.Object);
}
```
