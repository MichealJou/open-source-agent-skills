# cn.hutool.extra.tokenizer.engine.ikanalyzer

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.tokenizer.engine.ikanalyzer.IKAnalyzerEngine`

```java
public class cn.hutool.extra.tokenizer.engine.ikanalyzer.IKAnalyzerEngine implements cn.hutool.extra.tokenizer.TokenizerEngine {
  public cn.hutool.extra.tokenizer.engine.ikanalyzer.IKAnalyzerEngine();
  public cn.hutool.extra.tokenizer.engine.ikanalyzer.IKAnalyzerEngine(org.wltea.analyzer.core.IKSegmenter);
  public cn.hutool.extra.tokenizer.Result parse(java.lang.CharSequence);
}
```

## `cn.hutool.extra.tokenizer.engine.ikanalyzer.IKAnalyzerResult`

```java
public class cn.hutool.extra.tokenizer.engine.ikanalyzer.IKAnalyzerResult extends cn.hutool.extra.tokenizer.AbstractResult {
  public cn.hutool.extra.tokenizer.engine.ikanalyzer.IKAnalyzerResult(org.wltea.analyzer.core.IKSegmenter);
}
```

## `cn.hutool.extra.tokenizer.engine.ikanalyzer.IKAnalyzerWord`

```java
public class cn.hutool.extra.tokenizer.engine.ikanalyzer.IKAnalyzerWord implements cn.hutool.extra.tokenizer.Word {
  public cn.hutool.extra.tokenizer.engine.ikanalyzer.IKAnalyzerWord(org.wltea.analyzer.core.Lexeme);
  public java.lang.String getText();
  public int getStartOffset();
  public int getEndOffset();
  public java.lang.String toString();
}
```
