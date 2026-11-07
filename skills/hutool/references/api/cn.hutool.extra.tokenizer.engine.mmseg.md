# cn.hutool.extra.tokenizer.engine.mmseg

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.tokenizer.engine.mmseg.MmsegEngine`

```java
public class cn.hutool.extra.tokenizer.engine.mmseg.MmsegEngine implements cn.hutool.extra.tokenizer.TokenizerEngine {
  public cn.hutool.extra.tokenizer.engine.mmseg.MmsegEngine();
  public cn.hutool.extra.tokenizer.engine.mmseg.MmsegEngine(com.chenlb.mmseg4j.MMSeg);
  public cn.hutool.extra.tokenizer.Result parse(java.lang.CharSequence);
}
```

## `cn.hutool.extra.tokenizer.engine.mmseg.MmsegResult`

```java
public class cn.hutool.extra.tokenizer.engine.mmseg.MmsegResult extends cn.hutool.extra.tokenizer.AbstractResult {
  public cn.hutool.extra.tokenizer.engine.mmseg.MmsegResult(com.chenlb.mmseg4j.MMSeg);
}
```

## `cn.hutool.extra.tokenizer.engine.mmseg.MmsegWord`

```java
public class cn.hutool.extra.tokenizer.engine.mmseg.MmsegWord implements cn.hutool.extra.tokenizer.Word {
  public cn.hutool.extra.tokenizer.engine.mmseg.MmsegWord(com.chenlb.mmseg4j.Word);
  public java.lang.String getText();
  public int getStartOffset();
  public int getEndOffset();
  public java.lang.String toString();
}
```
