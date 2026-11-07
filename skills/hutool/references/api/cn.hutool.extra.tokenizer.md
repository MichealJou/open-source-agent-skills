# cn.hutool.extra.tokenizer

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.tokenizer.AbstractResult`

```java
public abstract class cn.hutool.extra.tokenizer.AbstractResult extends cn.hutool.core.collection.ComputeIter<cn.hutool.extra.tokenizer.Word> implements cn.hutool.extra.tokenizer.Result {
  public cn.hutool.extra.tokenizer.AbstractResult();
}
```

## `cn.hutool.extra.tokenizer.TokenizerEngine`

```java
public interface cn.hutool.extra.tokenizer.TokenizerEngine {
  public abstract cn.hutool.extra.tokenizer.Result parse(java.lang.CharSequence);
}
```

## `cn.hutool.extra.tokenizer.TokenizerException`

```java
public class cn.hutool.extra.tokenizer.TokenizerException extends java.lang.RuntimeException {
  public cn.hutool.extra.tokenizer.TokenizerException(java.lang.Throwable);
  public cn.hutool.extra.tokenizer.TokenizerException(java.lang.String);
  public cn.hutool.extra.tokenizer.TokenizerException(java.lang.String, java.lang.Object...);
  public cn.hutool.extra.tokenizer.TokenizerException(java.lang.String, java.lang.Throwable);
  public cn.hutool.extra.tokenizer.TokenizerException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.extra.tokenizer.TokenizerException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.extra.tokenizer.TokenizerUtil`

```java
public class cn.hutool.extra.tokenizer.TokenizerUtil {
  public cn.hutool.extra.tokenizer.TokenizerUtil();
  public static cn.hutool.extra.tokenizer.TokenizerEngine createEngine();
}
```

## `cn.hutool.extra.tokenizer.Word`

```java
public interface cn.hutool.extra.tokenizer.Word extends java.io.Serializable {
  public abstract java.lang.String getText();
  public abstract int getStartOffset();
  public abstract int getEndOffset();
}
```
