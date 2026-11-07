# cn.hutool.ai.model.ollama

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.ai.model.ollama.OllamaCommon$OllamaFormat` | `String getFormat()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.ollama.OllamaConfig` | `String getModelName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.ollama.OllamaProvider` | `OllamaService create(final AIConfig config)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.ollama.OllamaProvider` | `String getServiceName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.ollama.OllamaService` | `String chat(String prompt)` | 简化的对话方法 |
| `cn.hutool.ai.model.ollama.OllamaService` | `String copyModel(String source,String destination)` | 复制模型 |
| `cn.hutool.ai.model.ollama.OllamaService` | `String deleteModel(String modelName)` | 删除模型 |
| `cn.hutool.ai.model.ollama.OllamaService` | `String embeddings(String prompt)` | 生成文本嵌入向量 |
| `cn.hutool.ai.model.ollama.OllamaService` | `String generate(String prompt)` | 生成文本补全 |
| `cn.hutool.ai.model.ollama.OllamaService` | `String generate(String prompt,String format)` | 生成文本补全（带选项） |
| `cn.hutool.ai.model.ollama.OllamaService` | `String listModels()` | 列出本地可用的模型 |
| `cn.hutool.ai.model.ollama.OllamaService` | `String pullModel(String modelName)` | 拉取模型 |
| `cn.hutool.ai.model.ollama.OllamaService` | `String showModel(String modelName)` | 显示模型信息 |
| `cn.hutool.ai.model.ollama.OllamaService` | `void chat(String prompt,Consumer<String> callback)` | 简化的对话方法-SSE流式输出 |
| `cn.hutool.ai.model.ollama.OllamaService` | `void generate(String prompt,Consumer<String> callback)` | 生成文本补全-SSE流式输出 |
| `cn.hutool.ai.model.ollama.OllamaService` | `void generate(String prompt,String format,Consumer<String> callback)` | 生成文本补全（带选项）-SSE流式输出 |
| `cn.hutool.ai.model.ollama.OllamaServiceImpl` | `String chat(final List<Message> messages)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.ollama.OllamaServiceImpl` | `String copyModel(String source,String destination)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.ollama.OllamaServiceImpl` | `String deleteModel(String modelName)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.ollama.OllamaServiceImpl` | `String embeddings(String prompt)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.ollama.OllamaServiceImpl` | `String generate(String prompt)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.ollama.OllamaServiceImpl` | `String generate(String prompt,String format)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.ollama.OllamaServiceImpl` | `String listModels()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.ollama.OllamaServiceImpl` | `String pullModel(String modelName)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.ollama.OllamaServiceImpl` | `String showModel(String modelName)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.ollama.OllamaServiceImpl` | `void chat(final List<Message> messages,final Consumer<String> callback)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.ollama.OllamaServiceImpl` | `void generate(String prompt,Consumer<String> callback)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.ai.model.ollama.OllamaServiceImpl` | `void generate(String prompt,String format,Consumer<String> callback)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
