# cn.hutool.extra.tokenizer.engine.word

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.tokenizer.engine.word.WordEngine`

```java
public class cn.hutool.extra.tokenizer.engine.word.WordEngine implements cn.hutool.extra.tokenizer.TokenizerEngine {
  public cn.hutool.extra.tokenizer.engine.word.WordEngine();
  public cn.hutool.extra.tokenizer.engine.word.WordEngine(org.apdplat.word.segmentation.SegmentationAlgorithm);
  public cn.hutool.extra.tokenizer.engine.word.WordEngine(org.apdplat.word.segmentation.Segmentation);
  public cn.hutool.extra.tokenizer.Result parse(java.lang.CharSequence);
}
```

## `cn.hutool.extra.tokenizer.engine.word.WordResult`

```java
public class cn.hutool.extra.tokenizer.engine.word.WordResult implements cn.hutool.extra.tokenizer.Result {
  public cn.hutool.extra.tokenizer.engine.word.WordResult(java.util.List<org.apdplat.word.segmentation.Word>);
  public boolean hasNext();
  public cn.hutool.extra.tokenizer.Word next();
  public void remove();
  public java.lang.Object next();
}
```

## `cn.hutool.extra.tokenizer.engine.word.WordWord`

```java
public class cn.hutool.extra.tokenizer.engine.word.WordWord implements cn.hutool.extra.tokenizer.Word {
  public cn.hutool.extra.tokenizer.engine.word.WordWord(org.apdplat.word.segmentation.Word);
  public java.lang.String getText();
  public int getStartOffset();
  public int getEndOffset();
  public java.lang.String toString();
}
```
