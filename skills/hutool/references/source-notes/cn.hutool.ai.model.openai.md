# cn.hutool.ai.model.openai

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.ai.model.openai.OpenaiCommon$OpenaiReasoning` | `String getEffort()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.openai.OpenaiCommon$OpenaiSpeech` | `String getVoice()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.openai.OpenaiCommon$OpenaiVision` | `String getDetail()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.openai.OpenaiConfig` | `String getModelName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.openai.OpenaiProvider` | `OpenaiService create(final AIConfig config)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.openai.OpenaiProvider` | `String getServiceName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.openai.OpenaiService` | `InputStream textToSpeech(String input)` | TTS文本转语音 请设置config中model为支持TTS功能的模型 TTS系列 |
| `cn.hutool.ai.model.openai.OpenaiService` | `InputStream textToSpeech(String input,final OpenaiCommon.OpenaiSpeech voice)` | TTS文本转语音 请设置config中model为支持TTS功能的模型 TTS系列 |
| `cn.hutool.ai.model.openai.OpenaiService` | `String chatReasoning(String prompt)` | 推理chat 支持o3-mini和o1 |
| `cn.hutool.ai.model.openai.OpenaiService` | `String chatReasoning(String prompt,String reasoningEffort)` | 推理chat 支持o3-mini和o1 |
| `cn.hutool.ai.model.openai.OpenaiService` | `String chatReasoning(final List<Message> messages)` | 推理chat 支持o3-mini和o1 |
| `cn.hutool.ai.model.openai.OpenaiService` | `String chatReasoning(final List<Message> messages,String reasoningEffort)` | 推理chat 支持o3-mini和o1 |
| `cn.hutool.ai.model.openai.OpenaiService` | `String chatVision(String prompt,final List<String> images)` | 图像理解：模型会依据传入的图片信息以及问题，给出回复。 |
| `cn.hutool.ai.model.openai.OpenaiService` | `String chatVision(String prompt,final List<String> images,String detail)` | 图像理解：模型会依据传入的图片信息以及问题，给出回复。 |
| `cn.hutool.ai.model.openai.OpenaiService` | `String embeddingText(String input)` | 文本向量化 请设置config中model为支持文本向量化功能的模型 text-embedding系列 |
| `cn.hutool.ai.model.openai.OpenaiService` | `String imagesEdits(String prompt,final File image)` | 图片编辑 该方法仅支持 DALL·E 2 model |
| `cn.hutool.ai.model.openai.OpenaiService` | `String imagesEdits(String prompt,final File image,final File mask)` | 图片编辑 该方法仅支持 DALL·E 2 model |
| `cn.hutool.ai.model.openai.OpenaiService` | `String imagesGenerations(String prompt)` | 文生图 请设置config中model为支持图片功能的模型 DALL·E系列 |
| `cn.hutool.ai.model.openai.OpenaiService` | `String imagesVariations(final File image)` | 图片变形 该方法仅支持 DALL·E 2 model |
| `cn.hutool.ai.model.openai.OpenaiService` | `String moderations(String text)` | 检查文本是否具有潜在的危害性 仅支持omni-moderation-latest和text-moderation-latest模型 |
| `cn.hutool.ai.model.openai.OpenaiService` | `String moderations(String text,String imgUrl)` | 检查文本或图像是否具有潜在的危害性 仅支持omni-moderation-latest和text-moderation-latest模型 |
| `cn.hutool.ai.model.openai.OpenaiService` | `String speechToText(final File file)` | STT音频转文本 请设置config中model为支持STT功能的模型 whisper |
| `cn.hutool.ai.model.openai.OpenaiService` | `void chatReasoning(String prompt,String reasoningEffort,final Consumer<String> callback)` | 推理chat-SSE流式输出 支持o3-mini和o1 |
| `cn.hutool.ai.model.openai.OpenaiService` | `void chatReasoning(String prompt,final Consumer<String> callback)` | 推理chat-SSE流式输出 支持o3-mini和o1 |
| `cn.hutool.ai.model.openai.OpenaiService` | `void chatReasoning(final List<Message> messages,String reasoningEffort,final Consumer<String> callback)` | 推理chat-SSE流式输出 支持o3-mini和o1 |
| `cn.hutool.ai.model.openai.OpenaiService` | `void chatReasoning(final List<Message> messages,final Consumer<String> callback)` | 推理chat-SSE流式输出 支持o3-mini和o1 |
| `cn.hutool.ai.model.openai.OpenaiService` | `void chatVision(String prompt,final List<String> images,String detail,final Consumer<String> callback)` | 图像理解-SSE流式输出 |
| `cn.hutool.ai.model.openai.OpenaiService` | `void chatVision(String prompt,final List<String> images,final Consumer<String> callback)` | 图像理解-SSE流式输出 |
| `cn.hutool.ai.model.openai.OpenaiServiceImpl` | `InputStream textToSpeech(String input,final OpenaiCommon.OpenaiSpeech voice)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.openai.OpenaiServiceImpl` | `String chat(final List<Message> messages)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.openai.OpenaiServiceImpl` | `String chatReasoning(final List<Message> messages,String reasoningEffort)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.openai.OpenaiServiceImpl` | `String chatVision(String prompt,final List<String> images,String detail)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.openai.OpenaiServiceImpl` | `String embeddingText(String input)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.openai.OpenaiServiceImpl` | `String imagesEdits(String prompt,final File image,final File mask)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.openai.OpenaiServiceImpl` | `String imagesGenerations(String prompt)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.openai.OpenaiServiceImpl` | `String imagesVariations(final File image)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.openai.OpenaiServiceImpl` | `String moderations(String text,String imgUrl)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.openai.OpenaiServiceImpl` | `String speechToText(final File file)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.openai.OpenaiServiceImpl` | `void chat(List<Message> messages,Consumer<String> callback)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.openai.OpenaiServiceImpl` | `void chatReasoning(List<Message> messages,String reasoningEffort,Consumer<String> callback)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.openai.OpenaiServiceImpl` | `void chatVision(String prompt,List<String> images,String detail,Consumer<String> callback)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
