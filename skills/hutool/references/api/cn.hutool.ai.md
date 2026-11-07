# cn.hutool.ai

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.ai.AIException`

```java
public class cn.hutool.ai.AIException extends java.lang.RuntimeException {
  public cn.hutool.ai.AIException(java.lang.Throwable);
  public cn.hutool.ai.AIException(java.lang.String);
  public cn.hutool.ai.AIException(java.lang.String, java.lang.Object...);
  public cn.hutool.ai.AIException(java.lang.String, java.lang.Throwable);
  public cn.hutool.ai.AIException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.ai.AIException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.ai.AIServiceFactory`

```java
public class cn.hutool.ai.AIServiceFactory {
  public cn.hutool.ai.AIServiceFactory();
  public static cn.hutool.ai.core.AIService getAIService(cn.hutool.ai.core.AIConfig);
  public static <T extends cn.hutool.ai.core.AIService> T getAIService(cn.hutool.ai.core.AIConfig, java.lang.Class<T>);
}
```

## `cn.hutool.ai.AIUtil`

```java
public class cn.hutool.ai.AIUtil {
  public cn.hutool.ai.AIUtil();
  public static <T extends cn.hutool.ai.core.AIService> T getAIService(cn.hutool.ai.core.AIConfig, java.lang.Class<T>);
  public static cn.hutool.ai.core.AIService getAIService(cn.hutool.ai.core.AIConfig);
  public static cn.hutool.ai.model.hutool.HutoolService getHutoolService(cn.hutool.ai.core.AIConfig);
  public static cn.hutool.ai.model.deepseek.DeepSeekService getDeepSeekService(cn.hutool.ai.core.AIConfig);
  public static cn.hutool.ai.model.doubao.DoubaoService getDoubaoService(cn.hutool.ai.core.AIConfig);
  public static cn.hutool.ai.model.grok.GrokService getGrokService(cn.hutool.ai.core.AIConfig);
  public static cn.hutool.ai.model.openai.OpenaiService getOpenAIService(cn.hutool.ai.core.AIConfig);
  public static cn.hutool.ai.model.gemini.GeminiService getGeminiService(cn.hutool.ai.core.AIConfig);
  public static java.lang.String chat(cn.hutool.ai.core.AIConfig, java.lang.String);
  public static java.lang.String chat(cn.hutool.ai.core.AIConfig, java.util.List<cn.hutool.ai.core.Message>);
}
```

## `cn.hutool.ai.ModelName`

```java
public final class cn.hutool.ai.ModelName extends java.lang.Enum<cn.hutool.ai.ModelName> {
  public static cn.hutool.ai.ModelName[] values();
  public static cn.hutool.ai.ModelName valueOf(java.lang.String);
  public java.lang.String getValue();
}
```

## `cn.hutool.ai.Models`

```java
public class cn.hutool.ai.Models {
  public cn.hutool.ai.Models();
}
```

## `cn.hutool.ai.Models$DeepSeek`

```java
public final class cn.hutool.ai.Models$DeepSeek extends java.lang.Enum<cn.hutool.ai.Models$DeepSeek> {
  public static cn.hutool.ai.Models$DeepSeek[] values();
  public static cn.hutool.ai.Models$DeepSeek valueOf(java.lang.String);
  public java.lang.String getModel();
}
```

## `cn.hutool.ai.Models$Doubao`

```java
public final class cn.hutool.ai.Models$Doubao extends java.lang.Enum<cn.hutool.ai.Models$Doubao> {
  public static cn.hutool.ai.Models$Doubao[] values();
  public static cn.hutool.ai.Models$Doubao valueOf(java.lang.String);
  public java.lang.String getModel();
}
```

## `cn.hutool.ai.Models$Gemini`

```java
public final class cn.hutool.ai.Models$Gemini extends java.lang.Enum<cn.hutool.ai.Models$Gemini> {
  public static cn.hutool.ai.Models$Gemini[] values();
  public static cn.hutool.ai.Models$Gemini valueOf(java.lang.String);
  public java.lang.String getModel();
}
```

## `cn.hutool.ai.Models$Grok`

```java
public final class cn.hutool.ai.Models$Grok extends java.lang.Enum<cn.hutool.ai.Models$Grok> {
  public static cn.hutool.ai.Models$Grok[] values();
  public static cn.hutool.ai.Models$Grok valueOf(java.lang.String);
  public java.lang.String getModel();
}
```

## `cn.hutool.ai.Models$Hutool`

```java
public final class cn.hutool.ai.Models$Hutool extends java.lang.Enum<cn.hutool.ai.Models$Hutool> {
  public static cn.hutool.ai.Models$Hutool[] values();
  public static cn.hutool.ai.Models$Hutool valueOf(java.lang.String);
  public java.lang.String getModel();
}
```

## `cn.hutool.ai.Models$Ollama`

```java
public final class cn.hutool.ai.Models$Ollama extends java.lang.Enum<cn.hutool.ai.Models$Ollama> {
  public static cn.hutool.ai.Models$Ollama[] values();
  public static cn.hutool.ai.Models$Ollama valueOf(java.lang.String);
  public java.lang.String getModel();
}
```

## `cn.hutool.ai.Models$Openai`

```java
public final class cn.hutool.ai.Models$Openai extends java.lang.Enum<cn.hutool.ai.Models$Openai> {
  public static cn.hutool.ai.Models$Openai[] values();
  public static cn.hutool.ai.Models$Openai valueOf(java.lang.String);
  public java.lang.String getModel();
}
```
