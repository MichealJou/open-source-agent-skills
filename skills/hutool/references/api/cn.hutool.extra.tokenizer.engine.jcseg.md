# cn.hutool.extra.tokenizer.engine.jcseg

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.tokenizer.engine.jcseg.JcsegEngine`

```java
public class cn.hutool.extra.tokenizer.engine.jcseg.JcsegEngine implements cn.hutool.extra.tokenizer.TokenizerEngine {
  public cn.hutool.extra.tokenizer.engine.jcseg.JcsegEngine();
  public cn.hutool.extra.tokenizer.engine.jcseg.JcsegEngine(org.lionsoul.jcseg.ISegment);
  public cn.hutool.extra.tokenizer.Result parse(java.lang.CharSequence);
}
```

## `cn.hutool.extra.tokenizer.engine.jcseg.JcsegResult`

```java
public class cn.hutool.extra.tokenizer.engine.jcseg.JcsegResult extends cn.hutool.extra.tokenizer.AbstractResult {
  public cn.hutool.extra.tokenizer.engine.jcseg.JcsegResult(org.lionsoul.jcseg.ISegment);
}
```

## `cn.hutool.extra.tokenizer.engine.jcseg.JcsegWord`

```java
public class cn.hutool.extra.tokenizer.engine.jcseg.JcsegWord implements cn.hutool.extra.tokenizer.Word {
  public cn.hutool.extra.tokenizer.engine.jcseg.JcsegWord(org.lionsoul.jcseg.IWord);
  public java.lang.String getText();
  public int getStartOffset();
  public int getEndOffset();
  public java.lang.String toString();
}
```
