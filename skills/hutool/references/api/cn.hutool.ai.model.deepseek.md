# cn.hutool.ai.model.deepseek

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.ai.model.deepseek.DeepSeekCommon`

```java
public class cn.hutool.ai.model.deepseek.DeepSeekCommon {
  public cn.hutool.ai.model.deepseek.DeepSeekCommon();
}
```

## `cn.hutool.ai.model.deepseek.DeepSeekConfig`

```java
public class cn.hutool.ai.model.deepseek.DeepSeekConfig extends cn.hutool.ai.core.BaseConfig {
  public cn.hutool.ai.model.deepseek.DeepSeekConfig();
  public cn.hutool.ai.model.deepseek.DeepSeekConfig(java.lang.String);
  public java.lang.String getModelName();
}
```

## `cn.hutool.ai.model.deepseek.DeepSeekProvider`

```java
public class cn.hutool.ai.model.deepseek.DeepSeekProvider implements cn.hutool.ai.core.AIServiceProvider {
  public cn.hutool.ai.model.deepseek.DeepSeekProvider();
  public java.lang.String getServiceName();
  public cn.hutool.ai.model.deepseek.DeepSeekService create(cn.hutool.ai.core.AIConfig);
  public cn.hutool.ai.core.AIService create(cn.hutool.ai.core.AIConfig);
}
```

## `cn.hutool.ai.model.deepseek.DeepSeekService`

```java
public interface cn.hutool.ai.model.deepseek.DeepSeekService extends cn.hutool.ai.core.AIService {
  public abstract java.lang.String beta(java.lang.String);
  public abstract void beta(java.lang.String, java.util.function.Consumer<java.lang.String>);
  public abstract java.lang.String models();
  public abstract java.lang.String balance();
}
```

## `cn.hutool.ai.model.deepseek.DeepSeekServiceImpl`

```java
public class cn.hutool.ai.model.deepseek.DeepSeekServiceImpl extends cn.hutool.ai.core.BaseAIService implements cn.hutool.ai.model.deepseek.DeepSeekService {
  public cn.hutool.ai.model.deepseek.DeepSeekServiceImpl(cn.hutool.ai.core.AIConfig);
  public java.lang.String chat(java.util.List<cn.hutool.ai.core.Message>);
  public void chat(java.util.List<cn.hutool.ai.core.Message>, java.util.function.Consumer<java.lang.String>);
  public java.lang.String beta(java.lang.String);
  public void beta(java.lang.String, java.util.function.Consumer<java.lang.String>);
  public java.lang.String models();
  public java.lang.String balance();
}
```
