# cn.hutool.ai.model.openai

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.ai.model.openai.OpenaiCommon`

```java
public class cn.hutool.ai.model.openai.OpenaiCommon {
  public cn.hutool.ai.model.openai.OpenaiCommon();
}
```

## `cn.hutool.ai.model.openai.OpenaiCommon$OpenaiReasoning`

```java
public final class cn.hutool.ai.model.openai.OpenaiCommon$OpenaiReasoning extends java.lang.Enum<cn.hutool.ai.model.openai.OpenaiCommon$OpenaiReasoning> {
  public static cn.hutool.ai.model.openai.OpenaiCommon$OpenaiReasoning[] values();
  public static cn.hutool.ai.model.openai.OpenaiCommon$OpenaiReasoning valueOf(java.lang.String);
  public java.lang.String getEffort();
}
```

## `cn.hutool.ai.model.openai.OpenaiCommon$OpenaiSpeech`

```java
public final class cn.hutool.ai.model.openai.OpenaiCommon$OpenaiSpeech extends java.lang.Enum<cn.hutool.ai.model.openai.OpenaiCommon$OpenaiSpeech> {
  public static cn.hutool.ai.model.openai.OpenaiCommon$OpenaiSpeech[] values();
  public static cn.hutool.ai.model.openai.OpenaiCommon$OpenaiSpeech valueOf(java.lang.String);
  public java.lang.String getVoice();
}
```

## `cn.hutool.ai.model.openai.OpenaiCommon$OpenaiVision`

```java
public final class cn.hutool.ai.model.openai.OpenaiCommon$OpenaiVision extends java.lang.Enum<cn.hutool.ai.model.openai.OpenaiCommon$OpenaiVision> {
  public static cn.hutool.ai.model.openai.OpenaiCommon$OpenaiVision[] values();
  public static cn.hutool.ai.model.openai.OpenaiCommon$OpenaiVision valueOf(java.lang.String);
  public java.lang.String getDetail();
}
```

## `cn.hutool.ai.model.openai.OpenaiConfig`

```java
public class cn.hutool.ai.model.openai.OpenaiConfig extends cn.hutool.ai.core.BaseConfig {
  public cn.hutool.ai.model.openai.OpenaiConfig();
  public cn.hutool.ai.model.openai.OpenaiConfig(java.lang.String);
  public java.lang.String getModelName();
}
```

## `cn.hutool.ai.model.openai.OpenaiProvider`

```java
public class cn.hutool.ai.model.openai.OpenaiProvider implements cn.hutool.ai.core.AIServiceProvider {
  public cn.hutool.ai.model.openai.OpenaiProvider();
  public java.lang.String getServiceName();
  public cn.hutool.ai.model.openai.OpenaiService create(cn.hutool.ai.core.AIConfig);
  public cn.hutool.ai.core.AIService create(cn.hutool.ai.core.AIConfig);
}
```

## `cn.hutool.ai.model.openai.OpenaiService`

```java
public interface cn.hutool.ai.model.openai.OpenaiService extends cn.hutool.ai.core.AIService {
  public abstract java.lang.String chatVision(java.lang.String, java.util.List<java.lang.String>, java.lang.String);
  public abstract void chatVision(java.lang.String, java.util.List<java.lang.String>, java.lang.String, java.util.function.Consumer<java.lang.String>);
  public default java.lang.String chatVision(java.lang.String, java.util.List<java.lang.String>);
  public default void chatVision(java.lang.String, java.util.List<java.lang.String>, java.util.function.Consumer<java.lang.String>);
  public abstract java.lang.String imagesGenerations(java.lang.String);
  public abstract java.lang.String imagesEdits(java.lang.String, java.io.File, java.io.File);
  public default java.lang.String imagesEdits(java.lang.String, java.io.File);
  public abstract java.lang.String imagesVariations(java.io.File);
  public abstract java.io.InputStream textToSpeech(java.lang.String, cn.hutool.ai.model.openai.OpenaiCommon$OpenaiSpeech);
  public default java.io.InputStream textToSpeech(java.lang.String);
  public abstract java.lang.String speechToText(java.io.File);
  public abstract java.lang.String embeddingText(java.lang.String);
  public abstract java.lang.String moderations(java.lang.String, java.lang.String);
  public default java.lang.String moderations(java.lang.String);
  public default java.lang.String chatReasoning(java.lang.String, java.lang.String);
  public default void chatReasoning(java.lang.String, java.lang.String, java.util.function.Consumer<java.lang.String>);
  public default java.lang.String chatReasoning(java.lang.String);
  public default void chatReasoning(java.lang.String, java.util.function.Consumer<java.lang.String>);
  public abstract java.lang.String chatReasoning(java.util.List<cn.hutool.ai.core.Message>, java.lang.String);
  public abstract void chatReasoning(java.util.List<cn.hutool.ai.core.Message>, java.lang.String, java.util.function.Consumer<java.lang.String>);
  public default java.lang.String chatReasoning(java.util.List<cn.hutool.ai.core.Message>);
  public default void chatReasoning(java.util.List<cn.hutool.ai.core.Message>, java.util.function.Consumer<java.lang.String>);
}
```

## `cn.hutool.ai.model.openai.OpenaiServiceImpl`

```java
public class cn.hutool.ai.model.openai.OpenaiServiceImpl extends cn.hutool.ai.core.BaseAIService implements cn.hutool.ai.model.openai.OpenaiService {
  public cn.hutool.ai.model.openai.OpenaiServiceImpl(cn.hutool.ai.core.AIConfig);
  public java.lang.String chat(java.util.List<cn.hutool.ai.core.Message>);
  public void chat(java.util.List<cn.hutool.ai.core.Message>, java.util.function.Consumer<java.lang.String>);
  public java.lang.String chatVision(java.lang.String, java.util.List<java.lang.String>, java.lang.String);
  public void chatVision(java.lang.String, java.util.List<java.lang.String>, java.lang.String, java.util.function.Consumer<java.lang.String>);
  public java.lang.String imagesGenerations(java.lang.String);
  public java.lang.String imagesEdits(java.lang.String, java.io.File, java.io.File);
  public java.lang.String imagesVariations(java.io.File);
  public java.io.InputStream textToSpeech(java.lang.String, cn.hutool.ai.model.openai.OpenaiCommon$OpenaiSpeech);
  public java.lang.String speechToText(java.io.File);
  public java.lang.String embeddingText(java.lang.String);
  public java.lang.String moderations(java.lang.String, java.lang.String);
  public java.lang.String chatReasoning(java.util.List<cn.hutool.ai.core.Message>, java.lang.String);
  public void chatReasoning(java.util.List<cn.hutool.ai.core.Message>, java.lang.String, java.util.function.Consumer<java.lang.String>);
}
```
