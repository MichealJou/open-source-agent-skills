# cn.hutool.extra.tokenizer.engine.analysis

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.tokenizer.engine.analysis.AnalysisEngine`

```java
public class cn.hutool.extra.tokenizer.engine.analysis.AnalysisEngine implements cn.hutool.extra.tokenizer.TokenizerEngine {
  public cn.hutool.extra.tokenizer.engine.analysis.AnalysisEngine(org.apache.lucene.analysis.Analyzer);
  public cn.hutool.extra.tokenizer.Result parse(java.lang.CharSequence);
}
```

## `cn.hutool.extra.tokenizer.engine.analysis.AnalysisResult`

```java
public class cn.hutool.extra.tokenizer.engine.analysis.AnalysisResult extends cn.hutool.extra.tokenizer.AbstractResult {
  public cn.hutool.extra.tokenizer.engine.analysis.AnalysisResult(org.apache.lucene.analysis.TokenStream);
}
```

## `cn.hutool.extra.tokenizer.engine.analysis.AnalysisWord`

```java
public class cn.hutool.extra.tokenizer.engine.analysis.AnalysisWord implements cn.hutool.extra.tokenizer.Word {
  public cn.hutool.extra.tokenizer.engine.analysis.AnalysisWord(org.apache.lucene.analysis.tokenattributes.CharTermAttribute);
  public java.lang.String getText();
  public int getStartOffset();
  public int getEndOffset();
  public java.lang.String toString();
}
```

## `cn.hutool.extra.tokenizer.engine.analysis.SmartcnEngine`

```java
public class cn.hutool.extra.tokenizer.engine.analysis.SmartcnEngine extends cn.hutool.extra.tokenizer.engine.analysis.AnalysisEngine {
  public cn.hutool.extra.tokenizer.engine.analysis.SmartcnEngine();
}
```
