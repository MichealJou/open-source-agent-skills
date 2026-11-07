# cn.hutool.ai.model.doubao

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.ai.model.doubao.DoubaoCommon$DoubaoContext` | `String getMode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.doubao.DoubaoCommon$DoubaoVideo` | `Object getValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.doubao.DoubaoCommon$DoubaoVideo` | `String getType()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.doubao.DoubaoCommon$DoubaoVision` | `String getDetail()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.doubao.DoubaoConfig` | `String getModelName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.doubao.DoubaoProvider` | `DoubaoService create(final AIConfig config)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.doubao.DoubaoProvider` | `String getServiceName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.doubao.DoubaoService` | `String batchChat(String prompt)` | 批量推理 Chat 注意：调用该方法时，配置config中的model为您创建的批量推理接入点（Endpoint）ID。详细参考官方文档 该方法不支持流式 |
| `cn.hutool.ai.model.doubao.DoubaoService` | `String batchChat(final List<Message> messages)` | 批量推理 Chat 注意：调用该方法时，配置config中的model为您创建的批量推理接入点（Endpoint）ID。详细参考官方文档 该方法不支持流式 |
| `cn.hutool.ai.model.doubao.DoubaoService` | `String botsChat(final List<Message> messages)` | 应用(Bot) config中model设置为您创建的应用ID |
| `cn.hutool.ai.model.doubao.DoubaoService` | `String chatContext(String prompt,String contextId)` | 上下文缓存对话： 向大模型发起带上下文缓存的请求 注意：配置config中的model可以为您创建的推理接入点（Endpoint）ID，也可以是支持chat的model |
| `cn.hutool.ai.model.doubao.DoubaoService` | `String chatContext(final List<Message> messages,String contextId)` | 上下文缓存对话： 向大模型发起带上下文缓存的请求 注意：配置config中的model可以为您创建的推理接入点（Endpoint）ID，也可以是支持chat的model |
| `cn.hutool.ai.model.doubao.DoubaoService` | `String chatVision(String prompt,final List<String> images)` | 图像理解：模型会依据传入的图片信息以及问题，给出回复。 |
| `cn.hutool.ai.model.doubao.DoubaoService` | `String chatVision(String prompt,final List<String> images,String detail)` | 图像理解：模型会依据传入的图片信息以及问题，给出回复。 |
| `cn.hutool.ai.model.doubao.DoubaoService` | `String createContext(final List<Message> messages)` | 创建上下文缓存： 创建上下文缓存，获得缓存 id字段后，在上下文缓存对话 API中使用。 注意：调用该方法时，配置config中的model为您创建的推理接入点（Endpoint）ID, 推理接入点中使用的模型需要在模型管理中开启缓存功能。详细参考官方文档 |
| `cn.hutool.ai.model.doubao.DoubaoService` | `String createContext(final List<Message> messages,String mode)` | 创建上下文缓存： 创建上下文缓存，获得缓存 id字段后，在上下文缓存对话 API中使用。 注意：调用该方法时，配置config中的model为您创建的推理接入点（Endpoint）ID, 推理接入点中使用的模型需要在模型管理中开启缓存功能。详细参考官方文档 |
| `cn.hutool.ai.model.doubao.DoubaoService` | `String embeddingText(String[] input)` | 文本向量化 |
| `cn.hutool.ai.model.doubao.DoubaoService` | `String embeddingVision(String text,String image)` | 图文向量化：仅支持单一文本、单张图片或文本与图片的组合输入（即一段文本 + 一张图片），暂不支持批量文本 / 图片的同时处理 |
| `cn.hutool.ai.model.doubao.DoubaoService` | `String getVideoTasksInfo(String taskId)` | 查询视频生成任务信息 |
| `cn.hutool.ai.model.doubao.DoubaoService` | `String imagesGenerations(String prompt)` | 文生图 请设置config中model为支持图片功能的模型，目前支持Doubao-Seedream-3.0-t2i |
| `cn.hutool.ai.model.doubao.DoubaoService` | `String tokenization(String[] text)` | 分词：可以将文本转换为模型可理解的 token id，并返回文本的 tokens 数量、token id、 token 在原始文本中的偏移量等信息 |
| `cn.hutool.ai.model.doubao.DoubaoService` | `String videoTasks(String text,String image)` | 创建视频生成任务 注意：调用该方法时，配置config中的model为生成视频的模型或者您创建的推理接入点（Endpoint）ID。详细参考官方文档 |
| `cn.hutool.ai.model.doubao.DoubaoService` | `String videoTasks(String text,String image,final List<DoubaoCommon.DoubaoVideo> videoParams)` | 创建视频生成任务 注意：调用该方法时，配置config中的model为您创建的推理接入点（Endpoint）ID。详细参考官方文档 |
| `cn.hutool.ai.model.doubao.DoubaoService` | `void botsChat(final List<Message> messages,final Consumer<String> callback)` | 应用(Bot)-SSE流式输出 config中model设置为您创建的应用ID |
| `cn.hutool.ai.model.doubao.DoubaoService` | `void chatContext(String prompt,String contextId,final Consumer<String> callback)` | 上下文缓存对话-SSE流式输出 注意：配置config中的model可以为您创建的推理接入点（Endpoint）ID，也可以是支持chat的model |
| `cn.hutool.ai.model.doubao.DoubaoService` | `void chatContext(final List<Message> messages,String contextId,final Consumer<String> callback)` | 上下文缓存对话-SSE流式输出 注意：配置config中的model可以为您创建的推理接入点（Endpoint）ID，也可以是支持chat的model |
| `cn.hutool.ai.model.doubao.DoubaoService` | `void chatVision(String prompt,final List<String> images,String detail,final Consumer<String> callback)` | 图像理解-SSE流式输出 |
| `cn.hutool.ai.model.doubao.DoubaoService` | `void chatVision(String prompt,final List<String> images,final Consumer<String> callback)` | 图像理解-SSE流式输出 |
| `cn.hutool.ai.model.doubao.DoubaoServiceImpl` | `String batchChat(final List<Message> messages)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.doubao.DoubaoServiceImpl` | `String botsChat(final List<Message> messages)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.doubao.DoubaoServiceImpl` | `String chat(final List<Message> messages)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.doubao.DoubaoServiceImpl` | `String chatContext(final List<Message> messages,String contextId)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.doubao.DoubaoServiceImpl` | `String chatVision(String prompt,final List<String> images,String detail)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.doubao.DoubaoServiceImpl` | `String createContext(final List<Message> messages,String mode)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.doubao.DoubaoServiceImpl` | `String embeddingText(String[] input)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.doubao.DoubaoServiceImpl` | `String embeddingVision(String text,String image)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.doubao.DoubaoServiceImpl` | `String getVideoTasksInfo(String taskId)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.doubao.DoubaoServiceImpl` | `String imagesGenerations(String prompt)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.doubao.DoubaoServiceImpl` | `String tokenization(String[] text)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.doubao.DoubaoServiceImpl` | `String videoTasks(String text,String image,final List<DoubaoCommon.DoubaoVideo> videoParams)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.doubao.DoubaoServiceImpl` | `void botsChat(List<Message> messages,Consumer<String> callback)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.doubao.DoubaoServiceImpl` | `void chat(final List<Message> messages,final Consumer<String> callback)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.doubao.DoubaoServiceImpl` | `void chatContext(final List<Message> messages,String contextId,final Consumer<String> callback)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.doubao.DoubaoServiceImpl` | `void chatVision(String prompt,List<String> images,String detail,Consumer<String> callback)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
