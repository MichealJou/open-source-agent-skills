# cn.hutool.ai.model.grok

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.ai.model.grok.GrokCommon$GrokVision` | `String getDetail()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.grok.GrokConfig` | `String getModelName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.grok.GrokProvider` | `GrokService create(final AIConfig config)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.grok.GrokProvider` | `String getServiceName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.grok.GrokService` | `String chatVision(String prompt,final List<String> images)` | 图像理解：模型会依据传入的图片信息以及问题，给出回复。 |
| `cn.hutool.ai.model.grok.GrokService` | `String chatVision(String prompt,final List<String> images,String detail)` | 图像理解：模型会依据传入的图片信息以及问题，给出回复。 |
| `cn.hutool.ai.model.grok.GrokService` | `String deferredCompletion(String requestId)` | 从延迟对话中获取结果 |
| `cn.hutool.ai.model.grok.GrokService` | `String getLanguageModel(String modelId)` | 获取语言模型信息 |
| `cn.hutool.ai.model.grok.GrokService` | `String getModel(String modelId)` | 获取模型信息 |
| `cn.hutool.ai.model.grok.GrokService` | `String imagesGenerations(String prompt)` | 文生图 请设置config中model为支持图片功能的模型，目前支持GROK_2_IMAGE |
| `cn.hutool.ai.model.grok.GrokService` | `String languageModels()` | 列出所有语言model |
| `cn.hutool.ai.model.grok.GrokService` | `String message(List<Message> messages,int maxToken)` | 创建消息回复 |
| `cn.hutool.ai.model.grok.GrokService` | `String message(String prompt,int maxToken)` | 创建消息回复 |
| `cn.hutool.ai.model.grok.GrokService` | `String models()` | 列出所有model列表 |
| `cn.hutool.ai.model.grok.GrokService` | `String tokenizeText(String text)` | 分词：可以将文本转换为模型可理解的 token 信息 |
| `cn.hutool.ai.model.grok.GrokService` | `void chatVision(String prompt,final List<String> images,String detail,final Consumer<String> callback)` | 图像理解-SSE流式输出 |
| `cn.hutool.ai.model.grok.GrokService` | `void chatVision(String prompt,final List<String> images,final Consumer<String> callback)` | 图像理解：模型会依据传入的图片信息以及问题，给出回复。 |
| `cn.hutool.ai.model.grok.GrokService` | `void message(List<Message> messages,int maxToken,final Consumer<String> callback)` | 创建消息回复-SSE流式输出 |
| `cn.hutool.ai.model.grok.GrokService` | `void message(String prompt,int maxToken,final Consumer<String> callback)` | 创建消息回复-SSE流式输出 |
| `cn.hutool.ai.model.grok.GrokServiceImpl` | `String chat(final List<Message> messages)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.grok.GrokServiceImpl` | `String chatVision(String prompt,final List<String> images,String detail)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.grok.GrokServiceImpl` | `String deferredCompletion(String requestId)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.grok.GrokServiceImpl` | `String getLanguageModel(String modelId)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.grok.GrokServiceImpl` | `String getModel(String modelId)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.grok.GrokServiceImpl` | `String imagesGenerations(String prompt)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.grok.GrokServiceImpl` | `String languageModels()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.grok.GrokServiceImpl` | `String message(final List<Message> messages,int maxToken)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.grok.GrokServiceImpl` | `String models()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.grok.GrokServiceImpl` | `String tokenizeText(String text)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.grok.GrokServiceImpl` | `void chat(List<Message> messages,Consumer<String> callback)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.grok.GrokServiceImpl` | `void chatVision(String prompt,List<String> images,String detail,Consumer<String> callback)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.grok.GrokServiceImpl` | `void message(List<Message> messages,int maxToken,final Consumer<String> callback)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
