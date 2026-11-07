# cn.hutool.extra.tokenizer.engine.jieba

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.tokenizer.engine.jieba.JiebaEngine`

```java
public class cn.hutool.extra.tokenizer.engine.jieba.JiebaEngine implements cn.hutool.extra.tokenizer.TokenizerEngine {
  public cn.hutool.extra.tokenizer.engine.jieba.JiebaEngine();
  public cn.hutool.extra.tokenizer.engine.jieba.JiebaEngine(com.huaban.analysis.jieba.JiebaSegmenter$SegMode);
  public cn.hutool.extra.tokenizer.Result parse(java.lang.CharSequence);
}
```

## `cn.hutool.extra.tokenizer.engine.jieba.JiebaResult`

```java
public class cn.hutool.extra.tokenizer.engine.jieba.JiebaResult implements cn.hutool.extra.tokenizer.Result {
  public cn.hutool.extra.tokenizer.engine.jieba.JiebaResult(java.util.List<com.huaban.analysis.jieba.SegToken>);
  public boolean hasNext();
  public cn.hutool.extra.tokenizer.Word next();
  public void remove();
  public java.lang.Object next();
}
```

## `cn.hutool.extra.tokenizer.engine.jieba.JiebaWord`

```java
public class cn.hutool.extra.tokenizer.engine.jieba.JiebaWord implements cn.hutool.extra.tokenizer.Word {
  public cn.hutool.extra.tokenizer.engine.jieba.JiebaWord(com.huaban.analysis.jieba.SegToken);
  public java.lang.String getText();
  public int getStartOffset();
  public int getEndOffset();
  public java.lang.String toString();
}
```
