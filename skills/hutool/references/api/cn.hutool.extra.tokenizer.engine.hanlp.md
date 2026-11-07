# cn.hutool.extra.tokenizer.engine.hanlp

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.tokenizer.engine.hanlp.HanLPEngine`

```java
public class cn.hutool.extra.tokenizer.engine.hanlp.HanLPEngine implements cn.hutool.extra.tokenizer.TokenizerEngine {
  public cn.hutool.extra.tokenizer.engine.hanlp.HanLPEngine();
  public cn.hutool.extra.tokenizer.engine.hanlp.HanLPEngine(com.hankcs.hanlp.seg.Segment);
  public cn.hutool.extra.tokenizer.Result parse(java.lang.CharSequence);
}
```

## `cn.hutool.extra.tokenizer.engine.hanlp.HanLPResult`

```java
public class cn.hutool.extra.tokenizer.engine.hanlp.HanLPResult implements cn.hutool.extra.tokenizer.Result {
  public cn.hutool.extra.tokenizer.engine.hanlp.HanLPResult(java.util.List<com.hankcs.hanlp.seg.common.Term>);
  public boolean hasNext();
  public cn.hutool.extra.tokenizer.Word next();
  public void remove();
  public java.lang.Object next();
}
```

## `cn.hutool.extra.tokenizer.engine.hanlp.HanLPWord`

```java
public class cn.hutool.extra.tokenizer.engine.hanlp.HanLPWord implements cn.hutool.extra.tokenizer.Word {
  public cn.hutool.extra.tokenizer.engine.hanlp.HanLPWord(com.hankcs.hanlp.seg.common.Term);
  public java.lang.String getText();
  public int getStartOffset();
  public int getEndOffset();
  public java.lang.String toString();
}
```
