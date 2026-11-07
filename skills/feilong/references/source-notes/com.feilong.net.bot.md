# com.feilong.net.bot

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.net.bot.AbstractBot` | `boolean getIsAsync()` | 获得 是否异步,默认false,表示是同步. |
| `com.feilong.net.bot.AbstractBot` | `boolean getIsCatchException()` | 获得 是否捕获异常,默认false,表示不捕获异常. |
| `com.feilong.net.bot.AbstractBot` | `boolean getIsThrowException()` | 当出现异常, 是否抛出异常. 默认false,表示不抛出exception; 如果是true 那么会抛出异常,需要自定捕获异常处理. |
| `com.feilong.net.bot.AbstractBot` | `boolean sendMessage(String content)` | 【原文待译】Send message. |
| `com.feilong.net.bot.AbstractBot` | `boolean sendMessage(String content,MessageParams inputMessageParams)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.net.bot.AbstractBot` | `void setIsAsync(boolean isAsync)` | 设置 是否异步,默认false,表示是同步. |
| `com.feilong.net.bot.AbstractBot` | `void setIsCatchException(boolean isCatchException)` | 设置 是否捕获异常,默认false,表示不捕获异常. |
| `com.feilong.net.bot.AbstractBot` | `void setIsThrowException(boolean isThrowException)` | 当出现异常, 是否抛出异常. 默认false,表示不抛出exception; 如果是true 那么会抛出异常,需要自定捕获异常处理. |
| `com.feilong.net.bot.Bot` | `String getKey()` | 获取该机器人的key(微信机器人是key属性, 钉钉是accessToken属性). |
| `com.feilong.net.bot.Bot` | `boolean sendMessage(String content)` | 消息, 支持markdown格式,也支持纯文本. |
| `com.feilong.net.bot.Bot` | `boolean sendMessage(String content,MessageParams messageParams)` | 发消息. |
| `com.feilong.net.bot.CombinationConfig` | `Bot getBot()` | 获得 使用的bot. |
| `com.feilong.net.bot.CombinationConfig` | `Logger getLogger()` | 获得 使用的logger. |
| `com.feilong.net.bot.CombinationConfig` | `String getSignName()` | 获得 签名. |
| `com.feilong.net.bot.CombinationConfig` | `boolean getIsPrintLog()` | 获得 是否输出日志, 默认是true , 如果是false 那么不输出日志. |
| `com.feilong.net.bot.CombinationConfig` | `boolean getIsSendBotMessage()` | 获得 是否发送机器人消息, 默认是true , 如果是false 那么不发送消息. |
| `com.feilong.net.bot.CombinationConfig` | `void setBot(Bot bot)` | 设置 使用的bot. |
| `com.feilong.net.bot.CombinationConfig` | `void setIsPrintLog(boolean isPrintLog)` | 设置 是否输出日志, 默认是true , 如果是false 那么不输出日志. |
| `com.feilong.net.bot.CombinationConfig` | `void setIsSendBotMessage(boolean isSendBotMessage)` | 设置 是否发送机器人消息, 默认是true , 如果是false 那么不发送消息. |
| `com.feilong.net.bot.CombinationConfig` | `void setLogger(Logger logger)` | 设置 使用的logger. |
| `com.feilong.net.bot.CombinationConfig` | `void setSignName(String signName)` | 设置 签名. |
| `com.feilong.net.bot.LogAndBotCombination` | `void debug(CombinationConfig combinationConfig,String pattern,Object... arguments)` | Debug级别输出日志以及发送机器人. |
| `com.feilong.net.bot.LogAndBotCombination` | `void debug(Logger logger,Bot bot,String pattern,Object... arguments)` | Debug级别输出日志以及发送机器人. |
| `com.feilong.net.bot.LogAndBotCombination` | `void debugWithSignName(Logger logger,Bot bot,String signName,String pattern,Object... arguments)` | Debug级别输出日志以及发送机器人. |
| `com.feilong.net.bot.LogAndBotCombination` | `void error(CombinationConfig combinationConfig,String pattern,Object... arguments)` | Error级别输出日志以及发送机器人. |
| `com.feilong.net.bot.LogAndBotCombination` | `void error(Logger logger,Bot bot,String pattern,Object... arguments)` | Error级别输出日志以及发送机器人. |
| `com.feilong.net.bot.LogAndBotCombination` | `void errorWithSignName(Logger logger,Bot bot,String signName,String pattern,Object... arguments)` | Error级别输出日志以及发送机器人. |
| `com.feilong.net.bot.LogAndBotCombination` | `void info(CombinationConfig combinationConfig,String pattern,Object... arguments)` | Info级别输出日志以及发送机器人. |
| `com.feilong.net.bot.LogAndBotCombination` | `void info(Logger logger,Bot bot,String pattern,Object... arguments)` | Info级别输出日志以及发送机器人. |
| `com.feilong.net.bot.LogAndBotCombination` | `void infoWithSignName(Logger logger,Bot bot,String signName,String pattern,Object... arguments)` | Info级别输出日志以及发送机器人. |
| `com.feilong.net.bot.LogAndBotCombination` | `void warn(CombinationConfig combinationConfig,String pattern,Object... arguments)` | Warn级别输出日志以及发送机器人. |
| `com.feilong.net.bot.LogAndBotCombination` | `void warn(Logger logger,Bot bot,String pattern,Object... arguments)` | Warn级别输出日志以及发送机器人. |
| `com.feilong.net.bot.LogAndBotCombination` | `void warnWithSignName(Logger logger,Bot bot,String signName,String pattern,Object... arguments)` | Warn级别输出日志以及发送机器人. |
| `com.feilong.net.bot.MarkdownHelper` | `String b(String text)` | 加粗. |
| `com.feilong.net.bot.MarkdownHelper` | `String font(String text,String color)` | 用font标签包裹. 使用 标签设置颜色，但该标签不在钉钉Markdown格式消息的官方支持范围内，为了业务稳定性不建议使用 |
| `com.feilong.net.bot.MarkdownHelper` | `String link(String text,String url)` | 生成标签. |
| `com.feilong.net.bot.MarkdownHelper` | `String newLine()` | 一个\n有时无法成功换行，建议使用两个\n\n确保换行效果。 |
| `com.feilong.net.bot.MarkdownStringCreator` | `String createListString(String title,Map<String, String> itemMap)` | 生成 类似于的markdown string. |
