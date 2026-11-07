# cn.hutool.ai.core

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.ai.core.AIConfig`

```java
public interface cn.hutool.ai.core.AIConfig {
  public default java.lang.String getModelName();
  public abstract void setApiKey(java.lang.String);
  public abstract java.lang.String getApiKey();
  public abstract void setApiUrl(java.lang.String);
  public abstract java.lang.String getApiUrl();
  public abstract void setModel(java.lang.String);
  public abstract java.lang.String getModel();
  public abstract void putAdditionalConfigByKey(java.lang.String, java.lang.Object);
  public abstract java.lang.Object getAdditionalConfigByKey(java.lang.String);
  public abstract java.util.Map<java.lang.String, java.lang.Object> getAdditionalConfigMap();
  public abstract void setTimeout(int);
  public abstract int getTimeout();
  public abstract void setReadTimeout(int);
  public abstract int getReadTimeout();
  public abstract boolean getHasProxy();
  public abstract void setHasProxy(boolean);
  public abstract java.net.Proxy getProxy();
  public abstract void setProxy(java.net.Proxy);
}
```

## `cn.hutool.ai.core.AIConfigBuilder`

```java
public class cn.hutool.ai.core.AIConfigBuilder {
  public cn.hutool.ai.core.AIConfigBuilder(java.lang.String);
  public synchronized cn.hutool.ai.core.AIConfigBuilder setApiKey(java.lang.String);
  public synchronized cn.hutool.ai.core.AIConfigBuilder setApiUrl(java.lang.String);
  public synchronized cn.hutool.ai.core.AIConfigBuilder setModel(java.lang.String);
  public cn.hutool.ai.core.AIConfigBuilder putAdditionalConfig(java.lang.String, java.lang.Object);
  public cn.hutool.ai.core.AIConfigBuilder setTimout(int);
  public synchronized cn.hutool.ai.core.AIConfigBuilder setTimeout(int);
  public cn.hutool.ai.core.AIConfigBuilder setReadTimout(int);
  public synchronized cn.hutool.ai.core.AIConfigBuilder setReadTimeout(int);
  public synchronized cn.hutool.ai.core.AIConfigBuilder setProxy(java.net.Proxy);
  public cn.hutool.ai.core.AIConfig build();
}
```

## `cn.hutool.ai.core.AIConfigRegistry`

```java
public class cn.hutool.ai.core.AIConfigRegistry {
  public cn.hutool.ai.core.AIConfigRegistry();
  public static java.lang.Class<? extends cn.hutool.ai.core.AIConfig> getConfigClass(java.lang.String);
}
```

## `cn.hutool.ai.core.AIService`

```java
public interface cn.hutool.ai.core.AIService {
  public default java.lang.String chat(java.lang.String);
  public default void chat(java.lang.String, java.util.function.Consumer<java.lang.String>);
  public abstract java.lang.String chat(java.util.List<cn.hutool.ai.core.Message>);
  public abstract void chat(java.util.List<cn.hutool.ai.core.Message>, java.util.function.Consumer<java.lang.String>);
}
```

## `cn.hutool.ai.core.AIServiceProvider`

```java
public interface cn.hutool.ai.core.AIServiceProvider {
  public abstract java.lang.String getServiceName();
  public abstract <T extends cn.hutool.ai.core.AIService> T create(cn.hutool.ai.core.AIConfig);
}
```

## `cn.hutool.ai.core.BaseAIService`

```java
public class cn.hutool.ai.core.BaseAIService {
  public cn.hutool.ai.core.BaseAIService(cn.hutool.ai.core.AIConfig);
}
```

## `cn.hutool.ai.core.BaseConfig`

```java
public class cn.hutool.ai.core.BaseConfig implements cn.hutool.ai.core.AIConfig {
  public cn.hutool.ai.core.BaseConfig();
  public void setApiKey(java.lang.String);
  public java.lang.String getApiKey();
  public void setApiUrl(java.lang.String);
  public java.lang.String getApiUrl();
  public void setModel(java.lang.String);
  public java.lang.String getModel();
  public void putAdditionalConfigByKey(java.lang.String, java.lang.Object);
  public java.lang.Object getAdditionalConfigByKey(java.lang.String);
  public java.util.Map<java.lang.String, java.lang.Object> getAdditionalConfigMap();
  public int getTimeout();
  public void setTimeout(int);
  public int getReadTimeout();
  public void setReadTimeout(int);
  public boolean getHasProxy();
  public void setHasProxy(boolean);
  public java.net.Proxy getProxy();
  public void setProxy(java.net.Proxy);
}
```

## `cn.hutool.ai.core.Message`

```java
public class cn.hutool.ai.core.Message {
  public cn.hutool.ai.core.Message();
  public cn.hutool.ai.core.Message(java.lang.String, java.lang.Object);
  public void setRole(java.lang.String);
  public java.lang.String getRole();
  public java.lang.Object getContent();
  public void setContent(java.lang.Object);
}
```
