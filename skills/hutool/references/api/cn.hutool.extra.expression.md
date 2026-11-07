# cn.hutool.extra.expression

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.expression.ExpressionEngine`

```java
public interface cn.hutool.extra.expression.ExpressionEngine {
  public abstract java.lang.Object eval(java.lang.String, java.util.Map<java.lang.String, java.lang.Object>, java.util.Collection<java.lang.Class<?>>);
}
```

## `cn.hutool.extra.expression.ExpressionException`

```java
public class cn.hutool.extra.expression.ExpressionException extends java.lang.RuntimeException {
  public cn.hutool.extra.expression.ExpressionException(java.lang.Throwable);
  public cn.hutool.extra.expression.ExpressionException(java.lang.String);
  public cn.hutool.extra.expression.ExpressionException(java.lang.String, java.lang.Object...);
  public cn.hutool.extra.expression.ExpressionException(java.lang.String, java.lang.Throwable);
  public cn.hutool.extra.expression.ExpressionException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.extra.expression.ExpressionException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.extra.expression.ExpressionUtil`

```java
public class cn.hutool.extra.expression.ExpressionUtil {
  public cn.hutool.extra.expression.ExpressionUtil();
  public static cn.hutool.extra.expression.ExpressionEngine getEngine();
  public static java.lang.Object eval(java.lang.String, java.util.Map<java.lang.String, java.lang.Object>);
  public static java.lang.Object eval(java.lang.String, java.util.Map<java.lang.String, java.lang.Object>, java.util.Collection<java.lang.Class<?>>);
}
```
