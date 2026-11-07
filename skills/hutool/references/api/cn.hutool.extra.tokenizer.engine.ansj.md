# cn.hutool.extra.tokenizer.engine.ansj

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.tokenizer.engine.ansj.AnsjEngine`

```java
public class cn.hutool.extra.tokenizer.engine.ansj.AnsjEngine implements cn.hutool.extra.tokenizer.TokenizerEngine {
  public cn.hutool.extra.tokenizer.engine.ansj.AnsjEngine();
  public cn.hutool.extra.tokenizer.engine.ansj.AnsjEngine(org.ansj.splitWord.Analysis);
  public cn.hutool.extra.tokenizer.Result parse(java.lang.CharSequence);
}
```

## `cn.hutool.extra.tokenizer.engine.ansj.AnsjResult`

```java
public class cn.hutool.extra.tokenizer.engine.ansj.AnsjResult implements cn.hutool.extra.tokenizer.Result {
  public cn.hutool.extra.tokenizer.engine.ansj.AnsjResult(org.ansj.domain.Result);
  public boolean hasNext();
  public cn.hutool.extra.tokenizer.Word next();
  public void remove();
  public java.util.Iterator<cn.hutool.extra.tokenizer.Word> iterator();
  public java.lang.Object next();
}
```

## `cn.hutool.extra.tokenizer.engine.ansj.AnsjWord`

```java
public class cn.hutool.extra.tokenizer.engine.ansj.AnsjWord implements cn.hutool.extra.tokenizer.Word {
  public cn.hutool.extra.tokenizer.engine.ansj.AnsjWord(org.ansj.domain.Term);
  public java.lang.String getText();
  public int getStartOffset();
  public int getEndOffset();
  public java.lang.String toString();
}
```
