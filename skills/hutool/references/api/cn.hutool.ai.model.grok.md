# cn.hutool.ai.model.grok

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.ai.model.grok.GrokCommon`

```java
public class cn.hutool.ai.model.grok.GrokCommon {
  public cn.hutool.ai.model.grok.GrokCommon();
}
```

## `cn.hutool.ai.model.grok.GrokCommon$GrokVision`

```java
public final class cn.hutool.ai.model.grok.GrokCommon$GrokVision extends java.lang.Enum<cn.hutool.ai.model.grok.GrokCommon$GrokVision> {
  public static cn.hutool.ai.model.grok.GrokCommon$GrokVision[] values();
  public static cn.hutool.ai.model.grok.GrokCommon$GrokVision valueOf(java.lang.String);
  public java.lang.String getDetail();
}
```

## `cn.hutool.ai.model.grok.GrokConfig`

```java
public class cn.hutool.ai.model.grok.GrokConfig extends cn.hutool.ai.core.BaseConfig {
  public cn.hutool.ai.model.grok.GrokConfig();
  public cn.hutool.ai.model.grok.GrokConfig(java.lang.String);
  public java.lang.String getModelName();
}
```

## `cn.hutool.ai.model.grok.GrokProvider`

```java
public class cn.hutool.ai.model.grok.GrokProvider implements cn.hutool.ai.core.AIServiceProvider {
  public cn.hutool.ai.model.grok.GrokProvider();
  public java.lang.String getServiceName();
  public cn.hutool.ai.model.grok.GrokService create(cn.hutool.ai.core.AIConfig);
  public cn.hutool.ai.core.AIService create(cn.hutool.ai.core.AIConfig);
}
```

## `cn.hutool.ai.model.grok.GrokService`

```java
public interface cn.hutool.ai.model.grok.GrokService extends cn.hutool.ai.core.AIService {
  public default java.lang.String message(java.lang.String, int);
  public default void message(java.lang.String, int, java.util.function.Consumer<java.lang.String>);
  public abstract java.lang.String message(java.util.List<cn.hutool.ai.core.Message>, int);
  public abstract void message(java.util.List<cn.hutool.ai.core.Message>, int, java.util.function.Consumer<java.lang.String>);
  public abstract java.lang.String chatVision(java.lang.String, java.util.List<java.lang.String>, java.lang.String);
  public abstract void chatVision(java.lang.String, java.util.List<java.lang.String>, java.lang.String, java.util.function.Consumer<java.lang.String>);
  public default java.lang.String chatVision(java.lang.String, java.util.List<java.lang.String>);
  public default void chatVision(java.lang.String, java.util.List<java.lang.String>, java.util.function.Consumer<java.lang.String>);
  public abstract java.lang.String models();
  public abstract java.lang.String getModel(java.lang.String);
  public abstract java.lang.String languageModels();
  public abstract java.lang.String getLanguageModel(java.lang.String);
  public abstract java.lang.String tokenizeText(java.lang.String);
  public abstract java.lang.String deferredCompletion(java.lang.String);
  public abstract java.lang.String imagesGenerations(java.lang.String);
}
```

## `cn.hutool.ai.model.grok.GrokServiceImpl`

```java
public class cn.hutool.ai.model.grok.GrokServiceImpl extends cn.hutool.ai.core.BaseAIService implements cn.hutool.ai.model.grok.GrokService {
  public cn.hutool.ai.model.grok.GrokServiceImpl(cn.hutool.ai.core.AIConfig);
  public java.lang.String chat(java.util.List<cn.hutool.ai.core.Message>);
  public void chat(java.util.List<cn.hutool.ai.core.Message>, java.util.function.Consumer<java.lang.String>);
  public java.lang.String message(java.util.List<cn.hutool.ai.core.Message>, int);
  public void message(java.util.List<cn.hutool.ai.core.Message>, int, java.util.function.Consumer<java.lang.String>);
  public java.lang.String chatVision(java.lang.String, java.util.List<java.lang.String>, java.lang.String);
  public void chatVision(java.lang.String, java.util.List<java.lang.String>, java.lang.String, java.util.function.Consumer<java.lang.String>);
  public java.lang.String models();
  public java.lang.String getModel(java.lang.String);
  public java.lang.String languageModels();
  public java.lang.String getLanguageModel(java.lang.String);
  public java.lang.String tokenizeText(java.lang.String);
  public java.lang.String deferredCompletion(java.lang.String);
  public java.lang.String imagesGenerations(java.lang.String);
}
```
