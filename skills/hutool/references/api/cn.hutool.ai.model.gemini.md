# cn.hutool.ai.model.gemini

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.ai.model.gemini.GeminiCommon`

```java
public class cn.hutool.ai.model.gemini.GeminiCommon {
  public cn.hutool.ai.model.gemini.GeminiCommon();
}
```

## `cn.hutool.ai.model.gemini.GeminiCommon$GeminiAspectRatio`

```java
public final class cn.hutool.ai.model.gemini.GeminiCommon$GeminiAspectRatio extends java.lang.Enum<cn.hutool.ai.model.gemini.GeminiCommon$GeminiAspectRatio> {
  public static cn.hutool.ai.model.gemini.GeminiCommon$GeminiAspectRatio[] values();
  public static cn.hutool.ai.model.gemini.GeminiCommon$GeminiAspectRatio valueOf(java.lang.String);
  public java.lang.String getRatio();
}
```

## `cn.hutool.ai.model.gemini.GeminiCommon$GeminiDurationSeconds`

```java
public final class cn.hutool.ai.model.gemini.GeminiCommon$GeminiDurationSeconds extends java.lang.Enum<cn.hutool.ai.model.gemini.GeminiCommon$GeminiDurationSeconds> {
  public static cn.hutool.ai.model.gemini.GeminiCommon$GeminiDurationSeconds[] values();
  public static cn.hutool.ai.model.gemini.GeminiCommon$GeminiDurationSeconds valueOf(java.lang.String);
  public java.lang.Integer getValue();
}
```

## `cn.hutool.ai.model.gemini.GeminiCommon$GeminiImageCount`

```java
public final class cn.hutool.ai.model.gemini.GeminiCommon$GeminiImageCount extends java.lang.Enum<cn.hutool.ai.model.gemini.GeminiCommon$GeminiImageCount> {
  public static cn.hutool.ai.model.gemini.GeminiCommon$GeminiImageCount[] values();
  public static cn.hutool.ai.model.gemini.GeminiCommon$GeminiImageCount valueOf(java.lang.String);
  public int getCount();
}
```

## `cn.hutool.ai.model.gemini.GeminiCommon$GeminiImageSize`

```java
public final class cn.hutool.ai.model.gemini.GeminiCommon$GeminiImageSize extends java.lang.Enum<cn.hutool.ai.model.gemini.GeminiCommon$GeminiImageSize> {
  public static cn.hutool.ai.model.gemini.GeminiCommon$GeminiImageSize[] values();
  public static cn.hutool.ai.model.gemini.GeminiCommon$GeminiImageSize valueOf(java.lang.String);
  public java.lang.String getValue();
}
```

## `cn.hutool.ai.model.gemini.GeminiCommon$GeminiPersonGeneration`

```java
public final class cn.hutool.ai.model.gemini.GeminiCommon$GeminiPersonGeneration extends java.lang.Enum<cn.hutool.ai.model.gemini.GeminiCommon$GeminiPersonGeneration> {
  public static cn.hutool.ai.model.gemini.GeminiCommon$GeminiPersonGeneration[] values();
  public static cn.hutool.ai.model.gemini.GeminiCommon$GeminiPersonGeneration valueOf(java.lang.String);
  public java.lang.String getValue();
}
```

## `cn.hutool.ai.model.gemini.GeminiCommon$GeminiVoice`

```java
public final class cn.hutool.ai.model.gemini.GeminiCommon$GeminiVoice extends java.lang.Enum<cn.hutool.ai.model.gemini.GeminiCommon$GeminiVoice> {
  public static cn.hutool.ai.model.gemini.GeminiCommon$GeminiVoice[] values();
  public static cn.hutool.ai.model.gemini.GeminiCommon$GeminiVoice valueOf(java.lang.String);
  public java.lang.String getValue();
}
```

## `cn.hutool.ai.model.gemini.GeminiConfig`

```java
public class cn.hutool.ai.model.gemini.GeminiConfig extends cn.hutool.ai.core.BaseConfig {
  public cn.hutool.ai.model.gemini.GeminiConfig();
  public cn.hutool.ai.model.gemini.GeminiConfig(java.lang.String);
  public java.lang.String getModelName();
}
```

## `cn.hutool.ai.model.gemini.GeminiProvider`

```java
public class cn.hutool.ai.model.gemini.GeminiProvider implements cn.hutool.ai.core.AIServiceProvider {
  public cn.hutool.ai.model.gemini.GeminiProvider();
  public java.lang.String getServiceName();
  public cn.hutool.ai.model.gemini.GeminiService create(cn.hutool.ai.core.AIConfig);
  public cn.hutool.ai.core.AIService create(cn.hutool.ai.core.AIConfig);
}
```

## `cn.hutool.ai.model.gemini.GeminiService`

```java
public interface cn.hutool.ai.model.gemini.GeminiService extends cn.hutool.ai.core.AIService {
  public abstract java.lang.String chatMultimodal(java.lang.String, java.util.List<java.lang.String>);
  public abstract void chatMultimodal(java.lang.String, java.util.List<java.lang.String>, java.util.function.Consumer<java.lang.String>);
  public abstract java.lang.String chatJson(java.util.List<cn.hutool.ai.core.Message>);
  public abstract java.lang.String predictImage(java.lang.String);
  public abstract java.lang.String predictVideo(java.lang.String);
  public abstract java.lang.String getVideoOperation(java.lang.String);
  public abstract void downLoadVideo(java.lang.String, java.lang.String);
  public abstract java.lang.String textToSpeech(java.lang.String);
  public abstract java.lang.String textToSpeech(java.lang.String, java.lang.String);
  public abstract java.lang.String uploadFile(java.io.File);
  public abstract byte[] addWavHeader(byte[]);
}
```

## `cn.hutool.ai.model.gemini.GeminiServiceImpl`

```java
public class cn.hutool.ai.model.gemini.GeminiServiceImpl extends cn.hutool.ai.core.BaseAIService implements cn.hutool.ai.model.gemini.GeminiService {
  public cn.hutool.ai.model.gemini.GeminiServiceImpl(cn.hutool.ai.core.AIConfig);
  public java.lang.String chat(java.util.List<cn.hutool.ai.core.Message>);
  public void chat(java.util.List<cn.hutool.ai.core.Message>, java.util.function.Consumer<java.lang.String>);
  public java.lang.String chatMultimodal(java.lang.String, java.util.List<java.lang.String>);
  public void chatMultimodal(java.lang.String, java.util.List<java.lang.String>, java.util.function.Consumer<java.lang.String>);
  public java.lang.String chatJson(java.util.List<cn.hutool.ai.core.Message>);
  public java.lang.String predictImage(java.lang.String);
  public java.lang.String predictVideo(java.lang.String);
  public java.lang.String getVideoOperation(java.lang.String);
  public void downLoadVideo(java.lang.String, java.lang.String);
  public java.lang.String textToSpeech(java.lang.String);
  public java.lang.String textToSpeech(java.lang.String, java.lang.String);
  public java.lang.String uploadFile(java.io.File);
  public byte[] addWavHeader(byte[]);
}
```
