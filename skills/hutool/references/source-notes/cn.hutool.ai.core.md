# cn.hutool.ai.core

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.ai.core.AIConfig` | `Map<String, Object> getAdditionalConfigMap()` | 获取动态参数列表 |
| `cn.hutool.ai.core.AIConfig` | `Object getAdditionalConfigByKey(String key)` | 获取动态参数 |
| `cn.hutool.ai.core.AIConfig` | `Proxy getProxy()` | 获取代理配置 |
| `cn.hutool.ai.core.AIConfig` | `String getApiKey()` | 获取apiKey |
| `cn.hutool.ai.core.AIConfig` | `String getApiUrl()` | 获取apiUrl |
| `cn.hutool.ai.core.AIConfig` | `String getModel()` | 返回model |
| `cn.hutool.ai.core.AIConfig` | `String getModelName()` | 获取模型（厂商）名称 |
| `cn.hutool.ai.core.AIConfig` | `boolean getHasProxy()` | 获取是否使用代理 |
| `cn.hutool.ai.core.AIConfig` | `int getReadTimeout()` | 获取读取超时时间 |
| `cn.hutool.ai.core.AIConfig` | `int getTimeout()` | 获取连接超时时间 |
| `cn.hutool.ai.core.AIConfig` | `void putAdditionalConfigByKey(String key,Object value)` | 设置动态参数 |
| `cn.hutool.ai.core.AIConfig` | `void setApiKey(String apiKey)` | 设置apiKey |
| `cn.hutool.ai.core.AIConfig` | `void setApiUrl(String apiUrl)` | 设置apiUrl |
| `cn.hutool.ai.core.AIConfig` | `void setHasProxy(boolean hasProxy)` | 设置是否使用代理 |
| `cn.hutool.ai.core.AIConfig` | `void setModel(String model)` | 设置model |
| `cn.hutool.ai.core.AIConfig` | `void setProxy(Proxy proxy)` | 设置代理配置 |
| `cn.hutool.ai.core.AIConfig` | `void setReadTimeout(int readTimeout)` | 设置读取超时时间 |
| `cn.hutool.ai.core.AIConfig` | `void setTimeout(int timeout)` | 设置连接超时时间 |
| `cn.hutool.ai.core.AIConfigBuilder` | `AIConfig build()` | 返回config实例 |
| `cn.hutool.ai.core.AIConfigBuilder` | `AIConfigBuilder putAdditionalConfig(final String key,final Object value)` | 动态设置Request请求体中的属性字段，每个模型功能支持的字段请参照对应的官方文档 |
| `cn.hutool.ai.core.AIConfigBuilder` | `AIConfigBuilder setApiKey(final String apiKey)` | 设置apiKey |
| `cn.hutool.ai.core.AIConfigBuilder` | `AIConfigBuilder setApiUrl(final String apiUrl)` | 设置AI模型请求API接口的地址，不设置为默认值 |
| `cn.hutool.ai.core.AIConfigBuilder` | `AIConfigBuilder setModel(final String model)` | 设置具体的model，不设置为默认值 |
| `cn.hutool.ai.core.AIConfigBuilder` | `AIConfigBuilder setProxy(final Proxy proxy)` | 设置代理 |
| `cn.hutool.ai.core.AIConfigBuilder` | `AIConfigBuilder setReadTimeout(final int readTimeout)` | 设置读取超时时间，不设置为默认值 |
| `cn.hutool.ai.core.AIConfigBuilder` | `AIConfigBuilder setReadTimout(final int readTimout)` | 设置读取超时时间，不设置为默认值 |
| `cn.hutool.ai.core.AIConfigBuilder` | `AIConfigBuilder setTimeout(final int timeout)` | 设置连接超时时间，不设置为默认值 |
| `cn.hutool.ai.core.AIConfigBuilder` | `AIConfigBuilder setTimout(final int timeout)` | 设置连接超时时间，不设置为默认值 |
| `cn.hutool.ai.core.AIConfigRegistry` | `Class<? extends AIConfig> getConfigClass(final String modelName)` | 根据模型名称获取AIConfig实现类 |
| `cn.hutool.ai.core.AIService` | `String chat(String prompt)` | 对话 |
| `cn.hutool.ai.core.AIService` | `String chat(final List<Message> messages)` | 对话 |
| `cn.hutool.ai.core.AIService` | `void chat(String prompt,final Consumer<String> callback)` | 对话-SSE流式输出 |
| `cn.hutool.ai.core.AIService` | `void chat(final List<Message> messages,final Consumer<String> callback)` | 对话-SSE流式输出 |
| `cn.hutool.ai.core.AIServiceProvider` | `String getServiceName()` | 获取AI服务名称 |
| `cn.hutool.ai.core.AIServiceProvider` | `T create(final AIConfig config)` | 创建AI服务实例 |
| `cn.hutool.ai.core.BaseConfig` | `Map<String, Object> getAdditionalConfigMap()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.core.BaseConfig` | `Object getAdditionalConfigByKey(final String key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.core.BaseConfig` | `Proxy getProxy()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.core.BaseConfig` | `String getApiKey()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.core.BaseConfig` | `String getApiUrl()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.core.BaseConfig` | `String getModel()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.core.BaseConfig` | `boolean getHasProxy()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.core.BaseConfig` | `int getReadTimeout()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.core.BaseConfig` | `int getTimeout()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.core.BaseConfig` | `void putAdditionalConfigByKey(final String key,final Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.core.BaseConfig` | `void setApiKey(final String apiKey)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.core.BaseConfig` | `void setApiUrl(final String apiUrl)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.core.BaseConfig` | `void setHasProxy(boolean hasProxy)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.core.BaseConfig` | `void setModel(final String model)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.core.BaseConfig` | `void setProxy(Proxy proxy)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.core.BaseConfig` | `void setReadTimeout(final int readTimeout)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.core.BaseConfig` | `void setTimeout(final int timeout)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.core.Message` | `Object getContent()` | 获取内容 |
| `cn.hutool.ai.core.Message` | `String getRole()` | 获取角色 |
| `cn.hutool.ai.core.Message` | `void setContent(final Object content)` | 设置内容 |
| `cn.hutool.ai.core.Message` | `void setRole(final String role)` | 设置角色 |
