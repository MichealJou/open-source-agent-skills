# cn.hutool.extra.tokenizer.engine.mynlp

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.tokenizer.engine.mynlp.MynlpEngine`

```java
public class cn.hutool.extra.tokenizer.engine.mynlp.MynlpEngine implements cn.hutool.extra.tokenizer.TokenizerEngine {
  public cn.hutool.extra.tokenizer.engine.mynlp.MynlpEngine();
  public cn.hutool.extra.tokenizer.engine.mynlp.MynlpEngine(com.mayabot.nlp.segment.Lexer);
  public cn.hutool.extra.tokenizer.Result parse(java.lang.CharSequence);
}
```

## `cn.hutool.extra.tokenizer.engine.mynlp.MynlpResult`

```java
public class cn.hutool.extra.tokenizer.engine.mynlp.MynlpResult implements cn.hutool.extra.tokenizer.Result {
  public cn.hutool.extra.tokenizer.engine.mynlp.MynlpResult(com.mayabot.nlp.segment.Sentence);
  public boolean hasNext();
  public cn.hutool.extra.tokenizer.Word next();
  public void remove();
  public java.lang.Object next();
}
```

## `cn.hutool.extra.tokenizer.engine.mynlp.MynlpWord`

```java
public class cn.hutool.extra.tokenizer.engine.mynlp.MynlpWord implements cn.hutool.extra.tokenizer.Word {
  public cn.hutool.extra.tokenizer.engine.mynlp.MynlpWord(com.mayabot.nlp.segment.WordTerm);
  public java.lang.String getText();
  public int getStartOffset();
  public int getEndOffset();
  public java.lang.String toString();
}
```
