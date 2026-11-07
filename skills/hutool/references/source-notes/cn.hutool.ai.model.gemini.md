# cn.hutool.ai.model.gemini

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.ai.model.gemini.GeminiCommon$GeminiAspectRatio` | `String getRatio()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.gemini.GeminiCommon$GeminiDurationSeconds` | `Integer getValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.gemini.GeminiCommon$GeminiImageCount` | `int getCount()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.gemini.GeminiCommon$GeminiImageSize` | `String getValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.gemini.GeminiCommon$GeminiPersonGeneration` | `String getValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.gemini.GeminiCommon$GeminiVoice` | `String getValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.gemini.GeminiConfig` | `String getModelName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.gemini.GeminiProvider` | `GeminiService create(final AIConfig config)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.gemini.GeminiProvider` | `String getServiceName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.gemini.GeminiService` | `String chatJson(final List<Message> messages)` | 结构化输出：强制要求模型返回 JSON 格式 |
| `cn.hutool.ai.model.gemini.GeminiService` | `String chatMultimodal(String prompt,final List<String> mediaList)` | 全模态理解（图像/视频/音频/PDF）：模型会依据传入的媒体资源给出回复。 |
| `cn.hutool.ai.model.gemini.GeminiService` | `String getVideoOperation(String operationName)` | 获取视频生成状态：用于轮询视频生成进度 |
| `cn.hutool.ai.model.gemini.GeminiService` | `String predictImage(String prompt)` | 生成图像 (Imagen 模型集成) |
| `cn.hutool.ai.model.gemini.GeminiService` | `String predictVideo(String prompt)` | 生成视频:根据文本提示语生成视频 |
| `cn.hutool.ai.model.gemini.GeminiService` | `String textToSpeech(String prompt)` | 文本转语音 (TTS) |
| `cn.hutool.ai.model.gemini.GeminiService` | `String textToSpeech(String prompt,String voice)` | 文本转语音 (TTS) - 指定音色 |
| `cn.hutool.ai.model.gemini.GeminiService` | `String uploadFile(final File file)` | 上传大文件到Gemini File API |
| `cn.hutool.ai.model.gemini.GeminiService` | `byte[] addWavHeader(final byte[] rawPcm)` | 为原始 PCM 音频数据添加 WAV 头 |
| `cn.hutool.ai.model.gemini.GeminiService` | `void chatMultimodal(String prompt,final List<String> mediaList,final Consumer<String> callback)` | 全模态理解-SSE流式输出 |
| `cn.hutool.ai.model.gemini.GeminiService` | `void downLoadVideo(String videoUri,String filePath)` | 下载生成的视频文件 |
| `cn.hutool.ai.model.gemini.GeminiServiceImpl` | `String chat(final List<Message> messages)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.gemini.GeminiServiceImpl` | `String chatJson(final List<Message> messages)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.gemini.GeminiServiceImpl` | `String chatMultimodal(String prompt,final List<String> mediaList)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.gemini.GeminiServiceImpl` | `String getVideoOperation(String operationName)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.gemini.GeminiServiceImpl` | `String predictImage(String prompt)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.gemini.GeminiServiceImpl` | `String predictVideo(String prompt)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.gemini.GeminiServiceImpl` | `String textToSpeech(String prompt)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.gemini.GeminiServiceImpl` | `String textToSpeech(String prompt,String voice)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.gemini.GeminiServiceImpl` | `String uploadFile(final File file)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.gemini.GeminiServiceImpl` | `byte[] addWavHeader(final byte[] pcmData)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.gemini.GeminiServiceImpl` | `void chat(final List<Message> messages,final Consumer<String> callback)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.gemini.GeminiServiceImpl` | `void chatMultimodal(String prompt,final List<String> mediaList,final Consumer<String> callback)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.gemini.GeminiServiceImpl` | `void downLoadVideo(String videoUri,String filePath)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
