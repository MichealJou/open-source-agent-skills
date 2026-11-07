# cn.hutool.ai.model.doubao

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.ai.model.doubao.DoubaoCommon`

```java
public class cn.hutool.ai.model.doubao.DoubaoCommon {
  public cn.hutool.ai.model.doubao.DoubaoCommon();
}
```

## `cn.hutool.ai.model.doubao.DoubaoCommon$DoubaoContext`

```java
public final class cn.hutool.ai.model.doubao.DoubaoCommon$DoubaoContext extends java.lang.Enum<cn.hutool.ai.model.doubao.DoubaoCommon$DoubaoContext> {
  public static cn.hutool.ai.model.doubao.DoubaoCommon$DoubaoContext[] values();
  public static cn.hutool.ai.model.doubao.DoubaoCommon$DoubaoContext valueOf(java.lang.String);
  public java.lang.String getMode();
}
```

## `cn.hutool.ai.model.doubao.DoubaoCommon$DoubaoVideo`

```java
public final class cn.hutool.ai.model.doubao.DoubaoCommon$DoubaoVideo extends java.lang.Enum<cn.hutool.ai.model.doubao.DoubaoCommon$DoubaoVideo> {
  public static cn.hutool.ai.model.doubao.DoubaoCommon$DoubaoVideo[] values();
  public static cn.hutool.ai.model.doubao.DoubaoCommon$DoubaoVideo valueOf(java.lang.String);
  public java.lang.String getType();
  public java.lang.Object getValue();
}
```

## `cn.hutool.ai.model.doubao.DoubaoCommon$DoubaoVision`

```java
public final class cn.hutool.ai.model.doubao.DoubaoCommon$DoubaoVision extends java.lang.Enum<cn.hutool.ai.model.doubao.DoubaoCommon$DoubaoVision> {
  public static cn.hutool.ai.model.doubao.DoubaoCommon$DoubaoVision[] values();
  public static cn.hutool.ai.model.doubao.DoubaoCommon$DoubaoVision valueOf(java.lang.String);
  public java.lang.String getDetail();
}
```

## `cn.hutool.ai.model.doubao.DoubaoConfig`

```java
public class cn.hutool.ai.model.doubao.DoubaoConfig extends cn.hutool.ai.core.BaseConfig {
  public cn.hutool.ai.model.doubao.DoubaoConfig();
  public cn.hutool.ai.model.doubao.DoubaoConfig(java.lang.String);
  public java.lang.String getModelName();
}
```

## `cn.hutool.ai.model.doubao.DoubaoProvider`

```java
public class cn.hutool.ai.model.doubao.DoubaoProvider implements cn.hutool.ai.core.AIServiceProvider {
  public cn.hutool.ai.model.doubao.DoubaoProvider();
  public java.lang.String getServiceName();
  public cn.hutool.ai.model.doubao.DoubaoService create(cn.hutool.ai.core.AIConfig);
  public cn.hutool.ai.core.AIService create(cn.hutool.ai.core.AIConfig);
}
```

## `cn.hutool.ai.model.doubao.DoubaoService`

```java
public interface cn.hutool.ai.model.doubao.DoubaoService extends cn.hutool.ai.core.AIService {
  public default java.lang.String chatVision(java.lang.String, java.util.List<java.lang.String>);
  public default void chatVision(java.lang.String, java.util.List<java.lang.String>, java.util.function.Consumer<java.lang.String>);
  public abstract java.lang.String chatVision(java.lang.String, java.util.List<java.lang.String>, java.lang.String);
  public abstract void chatVision(java.lang.String, java.util.List<java.lang.String>, java.lang.String, java.util.function.Consumer<java.lang.String>);
  public abstract java.lang.String videoTasks(java.lang.String, java.lang.String, java.util.List<cn.hutool.ai.model.doubao.DoubaoCommon$DoubaoVideo>);
  public default java.lang.String videoTasks(java.lang.String, java.lang.String);
  public abstract java.lang.String getVideoTasksInfo(java.lang.String);
  public abstract java.lang.String embeddingText(java.lang.String[]);
  public abstract java.lang.String embeddingVision(java.lang.String, java.lang.String);
  public abstract java.lang.String botsChat(java.util.List<cn.hutool.ai.core.Message>);
  public abstract void botsChat(java.util.List<cn.hutool.ai.core.Message>, java.util.function.Consumer<java.lang.String>);
  public abstract java.lang.String tokenization(java.lang.String[]);
  public default java.lang.String batchChat(java.lang.String);
  public abstract java.lang.String batchChat(java.util.List<cn.hutool.ai.core.Message>);
  public abstract java.lang.String createContext(java.util.List<cn.hutool.ai.core.Message>, java.lang.String);
  public default java.lang.String createContext(java.util.List<cn.hutool.ai.core.Message>);
  public default java.lang.String chatContext(java.lang.String, java.lang.String);
  public default void chatContext(java.lang.String, java.lang.String, java.util.function.Consumer<java.lang.String>);
  public abstract java.lang.String chatContext(java.util.List<cn.hutool.ai.core.Message>, java.lang.String);
  public abstract void chatContext(java.util.List<cn.hutool.ai.core.Message>, java.lang.String, java.util.function.Consumer<java.lang.String>);
  public abstract java.lang.String imagesGenerations(java.lang.String);
}
```

## `cn.hutool.ai.model.doubao.DoubaoServiceImpl`

```java
public class cn.hutool.ai.model.doubao.DoubaoServiceImpl extends cn.hutool.ai.core.BaseAIService implements cn.hutool.ai.model.doubao.DoubaoService {
  public cn.hutool.ai.model.doubao.DoubaoServiceImpl(cn.hutool.ai.core.AIConfig);
  public java.lang.String chat(java.util.List<cn.hutool.ai.core.Message>);
  public void chat(java.util.List<cn.hutool.ai.core.Message>, java.util.function.Consumer<java.lang.String>);
  public java.lang.String chatVision(java.lang.String, java.util.List<java.lang.String>, java.lang.String);
  public void chatVision(java.lang.String, java.util.List<java.lang.String>, java.lang.String, java.util.function.Consumer<java.lang.String>);
  public java.lang.String videoTasks(java.lang.String, java.lang.String, java.util.List<cn.hutool.ai.model.doubao.DoubaoCommon$DoubaoVideo>);
  public java.lang.String getVideoTasksInfo(java.lang.String);
  public java.lang.String embeddingText(java.lang.String[]);
  public java.lang.String embeddingVision(java.lang.String, java.lang.String);
  public java.lang.String botsChat(java.util.List<cn.hutool.ai.core.Message>);
  public void botsChat(java.util.List<cn.hutool.ai.core.Message>, java.util.function.Consumer<java.lang.String>);
  public java.lang.String tokenization(java.lang.String[]);
  public java.lang.String batchChat(java.util.List<cn.hutool.ai.core.Message>);
  public java.lang.String createContext(java.util.List<cn.hutool.ai.core.Message>, java.lang.String);
  public java.lang.String chatContext(java.util.List<cn.hutool.ai.core.Message>, java.lang.String);
  public void chatContext(java.util.List<cn.hutool.ai.core.Message>, java.lang.String, java.util.function.Consumer<java.lang.String>);
  public java.lang.String imagesGenerations(java.lang.String);
}
```
