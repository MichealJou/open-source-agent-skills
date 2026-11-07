# cn.hutool.ai

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.ai.AIServiceFactory` | `AIService getAIService(final AIConfig config)` | 获取AI服务 |
| `cn.hutool.ai.AIServiceFactory` | `T getAIService(final AIConfig config,final Class<T> clazz)` | 获取AI服务 |
| `cn.hutool.ai.AIUtil` | `AIService getAIService(final AIConfig config)` | 获取AI模型服务 |
| `cn.hutool.ai.AIUtil` | `DeepSeekService getDeepSeekService(final AIConfig config)` | 获取DeepSeek模型服务 |
| `cn.hutool.ai.AIUtil` | `DoubaoService getDoubaoService(final AIConfig config)` | 获取Doubao模型服务 |
| `cn.hutool.ai.AIUtil` | `GeminiService getGeminiService(final AIConfig config)` | 获取Gemini模型服务 |
| `cn.hutool.ai.AIUtil` | `GrokService getGrokService(final AIConfig config)` | 获取Grok模型服务 |
| `cn.hutool.ai.AIUtil` | `HutoolService getHutoolService(final AIConfig config)` | 获取Hutool-AI服务 |
| `cn.hutool.ai.AIUtil` | `OpenaiService getOpenAIService(final AIConfig config)` | 获取Openai模型服务 |
| `cn.hutool.ai.AIUtil` | `String chat(final AIConfig config,final List<Message> messages)` | AI大模型对话功能 |
| `cn.hutool.ai.AIUtil` | `String chat(final AIConfig config,final String prompt)` | AI大模型对话功能 |
| `cn.hutool.ai.AIUtil` | `T getAIService(final AIConfig config,final Class<T> clazz)` | 获取AI模型服务，每个大模型提供的功能会不一样，可以调用此方法指定不同AI服务类，调用不同的功能 |
| `cn.hutool.ai.ModelName` | `String getValue()` | 获取值 |
| `cn.hutool.ai.Models$DeepSeek` | `String getModel()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.Models$Doubao` | `String getModel()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.Models$Gemini` | `String getModel()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.Models$Grok` | `String getModel()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.Models$Hutool` | `String getModel()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.Models$Ollama` | `String getModel()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.Models$Openai` | `String getModel()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
