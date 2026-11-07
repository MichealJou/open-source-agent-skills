# cn.hutool.ai.model.hutool

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.ai.model.hutool.HutoolCommon`

```java
public class cn.hutool.ai.model.hutool.HutoolCommon {
  public cn.hutool.ai.model.hutool.HutoolCommon();
}
```

## `cn.hutool.ai.model.hutool.HutoolCommon$HutoolSpeech`

```java
public final class cn.hutool.ai.model.hutool.HutoolCommon$HutoolSpeech extends java.lang.Enum<cn.hutool.ai.model.hutool.HutoolCommon$HutoolSpeech> {
  public static cn.hutool.ai.model.hutool.HutoolCommon$HutoolSpeech[] values();
  public static cn.hutool.ai.model.hutool.HutoolCommon$HutoolSpeech valueOf(java.lang.String);
  public java.lang.String getVoice();
}
```

## `cn.hutool.ai.model.hutool.HutoolCommon$HutoolVideo`

```java
public final class cn.hutool.ai.model.hutool.HutoolCommon$HutoolVideo extends java.lang.Enum<cn.hutool.ai.model.hutool.HutoolCommon$HutoolVideo> {
  public static cn.hutool.ai.model.hutool.HutoolCommon$HutoolVideo[] values();
  public static cn.hutool.ai.model.hutool.HutoolCommon$HutoolVideo valueOf(java.lang.String);
  public java.lang.String getType();
  public java.lang.Object getValue();
}
```

## `cn.hutool.ai.model.hutool.HutoolCommon$HutoolVision`

```java
public final class cn.hutool.ai.model.hutool.HutoolCommon$HutoolVision extends java.lang.Enum<cn.hutool.ai.model.hutool.HutoolCommon$HutoolVision> {
  public static cn.hutool.ai.model.hutool.HutoolCommon$HutoolVision[] values();
  public static cn.hutool.ai.model.hutool.HutoolCommon$HutoolVision valueOf(java.lang.String);
  public java.lang.String getDetail();
}
```

## `cn.hutool.ai.model.hutool.HutoolConfig`

```java
public class cn.hutool.ai.model.hutool.HutoolConfig extends cn.hutool.ai.core.BaseConfig {
  public cn.hutool.ai.model.hutool.HutoolConfig();
  public cn.hutool.ai.model.hutool.HutoolConfig(java.lang.String);
  public java.lang.String getModelName();
}
```

## `cn.hutool.ai.model.hutool.HutoolProvider`

```java
public class cn.hutool.ai.model.hutool.HutoolProvider implements cn.hutool.ai.core.AIServiceProvider {
  public cn.hutool.ai.model.hutool.HutoolProvider();
  public java.lang.String getServiceName();
  public cn.hutool.ai.model.hutool.HutoolService create(cn.hutool.ai.core.AIConfig);
  public cn.hutool.ai.core.AIService create(cn.hutool.ai.core.AIConfig);
}
```

## `cn.hutool.ai.model.hutool.HutoolService`

```java
public interface cn.hutool.ai.model.hutool.HutoolService extends cn.hutool.ai.core.AIService {
  public abstract java.lang.String chatVision(java.lang.String, java.util.List<java.lang.String>, java.lang.String);
  public abstract void chatVision(java.lang.String, java.util.List<java.lang.String>, java.lang.String, java.util.function.Consumer<java.lang.String>);
  public default java.lang.String chatVision(java.lang.String, java.util.List<java.lang.String>);
  public default void chatVision(java.lang.String, java.util.List<java.lang.String>, java.util.function.Consumer<java.lang.String>);
  public abstract java.lang.String tokenizeText(java.lang.String);
  public abstract java.lang.String imagesGenerations(java.lang.String);
  public abstract java.lang.String embeddingVision(java.lang.String, java.lang.String);
  public abstract java.io.InputStream tts(java.lang.String, cn.hutool.ai.model.hutool.HutoolCommon$HutoolSpeech);
  public default java.io.InputStream tts(java.lang.String);
  public abstract java.lang.String stt(java.io.File);
  public abstract java.lang.String videoTasks(java.lang.String, java.lang.String, java.util.List<cn.hutool.ai.model.hutool.HutoolCommon$HutoolVideo>);
  public default java.lang.String videoTasks(java.lang.String, java.lang.String);
  public abstract java.lang.String getVideoTasksInfo(java.lang.String);
}
```

## `cn.hutool.ai.model.hutool.HutoolServiceImpl`

```java
public class cn.hutool.ai.model.hutool.HutoolServiceImpl extends cn.hutool.ai.core.BaseAIService implements cn.hutool.ai.model.hutool.HutoolService {
  public cn.hutool.ai.model.hutool.HutoolServiceImpl(cn.hutool.ai.core.AIConfig);
  public java.lang.String chat(java.util.List<cn.hutool.ai.core.Message>);
  public void chat(java.util.List<cn.hutool.ai.core.Message>, java.util.function.Consumer<java.lang.String>);
  public java.lang.String chatVision(java.lang.String, java.util.List<java.lang.String>, java.lang.String);
  public void chatVision(java.lang.String, java.util.List<java.lang.String>, java.lang.String, java.util.function.Consumer<java.lang.String>);
  public java.lang.String tokenizeText(java.lang.String);
  public java.lang.String imagesGenerations(java.lang.String);
  public java.lang.String embeddingVision(java.lang.String, java.lang.String);
  public java.io.InputStream tts(java.lang.String, cn.hutool.ai.model.hutool.HutoolCommon$HutoolSpeech);
  public java.lang.String stt(java.io.File);
  public java.lang.String videoTasks(java.lang.String, java.lang.String, java.util.List<cn.hutool.ai.model.hutool.HutoolCommon$HutoolVideo>);
  public java.lang.String getVideoTasksInfo(java.lang.String);
}
```
