# cn.hutool.ai.model.ollama

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.ai.model.ollama.OllamaCommon`

```java
public class cn.hutool.ai.model.ollama.OllamaCommon {
  public cn.hutool.ai.model.ollama.OllamaCommon();
}
```

## `cn.hutool.ai.model.ollama.OllamaCommon$OllamaFormat`

```java
public final class cn.hutool.ai.model.ollama.OllamaCommon$OllamaFormat extends java.lang.Enum<cn.hutool.ai.model.ollama.OllamaCommon$OllamaFormat> {
  public static cn.hutool.ai.model.ollama.OllamaCommon$OllamaFormat[] values();
  public static cn.hutool.ai.model.ollama.OllamaCommon$OllamaFormat valueOf(java.lang.String);
  public java.lang.String getFormat();
}
```

## `cn.hutool.ai.model.ollama.OllamaCommon$Options`

```java
public class cn.hutool.ai.model.ollama.OllamaCommon$Options {
  public cn.hutool.ai.model.ollama.OllamaCommon$Options();
}
```

## `cn.hutool.ai.model.ollama.OllamaConfig`

```java
public class cn.hutool.ai.model.ollama.OllamaConfig extends cn.hutool.ai.core.BaseConfig {
  public cn.hutool.ai.model.ollama.OllamaConfig();
  public cn.hutool.ai.model.ollama.OllamaConfig(java.lang.String);
  public cn.hutool.ai.model.ollama.OllamaConfig(java.lang.String, java.lang.String);
  public java.lang.String getModelName();
}
```

## `cn.hutool.ai.model.ollama.OllamaProvider`

```java
public class cn.hutool.ai.model.ollama.OllamaProvider implements cn.hutool.ai.core.AIServiceProvider {
  public cn.hutool.ai.model.ollama.OllamaProvider();
  public java.lang.String getServiceName();
  public cn.hutool.ai.model.ollama.OllamaService create(cn.hutool.ai.core.AIConfig);
  public cn.hutool.ai.core.AIService create(cn.hutool.ai.core.AIConfig);
}
```

## `cn.hutool.ai.model.ollama.OllamaService`

```java
public interface cn.hutool.ai.model.ollama.OllamaService extends cn.hutool.ai.core.AIService {
  public abstract java.lang.String generate(java.lang.String);
  public abstract void generate(java.lang.String, java.util.function.Consumer<java.lang.String>);
  public abstract java.lang.String generate(java.lang.String, java.lang.String);
  public abstract void generate(java.lang.String, java.lang.String, java.util.function.Consumer<java.lang.String>);
  public abstract java.lang.String embeddings(java.lang.String);
  public abstract java.lang.String listModels();
  public abstract java.lang.String showModel(java.lang.String);
  public abstract java.lang.String pullModel(java.lang.String);
  public abstract java.lang.String deleteModel(java.lang.String);
  public abstract java.lang.String copyModel(java.lang.String, java.lang.String);
  public default java.lang.String chat(java.lang.String);
  public default void chat(java.lang.String, java.util.function.Consumer<java.lang.String>);
}
```

## `cn.hutool.ai.model.ollama.OllamaServiceImpl`

```java
public class cn.hutool.ai.model.ollama.OllamaServiceImpl extends cn.hutool.ai.core.BaseAIService implements cn.hutool.ai.model.ollama.OllamaService {
  public cn.hutool.ai.model.ollama.OllamaServiceImpl(cn.hutool.ai.core.AIConfig);
  public java.lang.String chat(java.util.List<cn.hutool.ai.core.Message>);
  public void chat(java.util.List<cn.hutool.ai.core.Message>, java.util.function.Consumer<java.lang.String>);
  public java.lang.String generate(java.lang.String);
  public void generate(java.lang.String, java.util.function.Consumer<java.lang.String>);
  public java.lang.String generate(java.lang.String, java.lang.String);
  public void generate(java.lang.String, java.lang.String, java.util.function.Consumer<java.lang.String>);
  public java.lang.String embeddings(java.lang.String);
  public java.lang.String listModels();
  public java.lang.String showModel(java.lang.String);
  public java.lang.String pullModel(java.lang.String);
  public java.lang.String deleteModel(java.lang.String);
  public java.lang.String copyModel(java.lang.String, java.lang.String);
}
```
