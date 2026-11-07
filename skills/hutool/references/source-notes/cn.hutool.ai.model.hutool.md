# cn.hutool.ai.model.hutool

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.ai.model.hutool.HutoolCommon$HutoolSpeech` | `String getVoice()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.hutool.HutoolCommon$HutoolVideo` | `Object getValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.hutool.HutoolCommon$HutoolVideo` | `String getType()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.hutool.HutoolCommon$HutoolVision` | `String getDetail()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.hutool.HutoolConfig` | `String getModelName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.hutool.HutoolProvider` | `HutoolService create(final AIConfig config)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.hutool.HutoolProvider` | `String getServiceName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.hutool.HutoolService` | `InputStream tts(String input)` | TTS文本转语音 |
| `cn.hutool.ai.model.hutool.HutoolService` | `InputStream tts(String input,final HutoolCommon.HutoolSpeech voice)` | TTS文本转语音 |
| `cn.hutool.ai.model.hutool.HutoolService` | `String chatVision(String prompt,final List<String> images)` | 图像理解：模型会依据传入的图片信息以及问题，给出回复。 |
| `cn.hutool.ai.model.hutool.HutoolService` | `String chatVision(String prompt,final List<String> images,String detail)` | 图像理解：模型会依据传入的图片信息以及问题，给出回复。 |
| `cn.hutool.ai.model.hutool.HutoolService` | `String embeddingVision(String text,String image)` | 图文向量化：仅支持单一文本、单张图片或文本与图片的组合输入（即一段文本 + 一张图片），暂不支持批量文本 / 图片的同时处理 |
| `cn.hutool.ai.model.hutool.HutoolService` | `String getVideoTasksInfo(String taskId)` | 查询视频生成任务信息 |
| `cn.hutool.ai.model.hutool.HutoolService` | `String imagesGenerations(String prompt)` | 文生图 |
| `cn.hutool.ai.model.hutool.HutoolService` | `String stt(final File file)` | STT音频转文本 |
| `cn.hutool.ai.model.hutool.HutoolService` | `String tokenizeText(String text)` | 分词：可以将文本转换为模型可理解的 token 信息 |
| `cn.hutool.ai.model.hutool.HutoolService` | `String videoTasks(String text,String image)` | 创建视频生成任务 |
| `cn.hutool.ai.model.hutool.HutoolService` | `String videoTasks(String text,String image,final List<HutoolCommon.HutoolVideo> videoParams)` | 创建视频生成任务 |
| `cn.hutool.ai.model.hutool.HutoolService` | `void chatVision(String prompt,final List<String> images,String detail,final Consumer<String> callback)` | 图像理解-SSE流式输出 |
| `cn.hutool.ai.model.hutool.HutoolService` | `void chatVision(String prompt,final List<String> images,final Consumer<String> callback)` | 图像理解：模型会依据传入的图片信息以及问题，给出回复。 |
| `cn.hutool.ai.model.hutool.HutoolServiceImpl` | `InputStream tts(String input,final HutoolCommon.HutoolSpeech voice)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.hutool.HutoolServiceImpl` | `String chat(final List<Message> messages)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.hutool.HutoolServiceImpl` | `String chatVision(String prompt,final List<String> images,String detail)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.hutool.HutoolServiceImpl` | `String embeddingVision(String text,String image)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.hutool.HutoolServiceImpl` | `String getVideoTasksInfo(String taskId)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.hutool.HutoolServiceImpl` | `String imagesGenerations(String prompt)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.hutool.HutoolServiceImpl` | `String stt(final File file)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.hutool.HutoolServiceImpl` | `String tokenizeText(String text)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.hutool.HutoolServiceImpl` | `String videoTasks(String text,String image,final List<HutoolCommon.HutoolVideo> videoParams)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.hutool.HutoolServiceImpl` | `void chat(List<Message> messages,Consumer<String> callback)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.hutool.HutoolServiceImpl` | `void chatVision(String prompt,List<String> images,String detail,Consumer<String> callback)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
