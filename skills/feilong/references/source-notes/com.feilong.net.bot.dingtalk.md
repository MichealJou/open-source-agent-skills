# com.feilong.net.bot.dingtalk

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.net.bot.dingtalk.DefaultDingTalkBot` | `String getKey()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.net.bot.dingtalk.DefaultDingTalkBot` | `boolean sendMessage(String title,String content,String... atMobiles)` | 【原文待译】Send message. |
| `com.feilong.net.bot.dingtalk.DefaultDingTalkBot` | `void setAccessToken(String accessToken)` | 【原文待译】Sets the key. |
| `com.feilong.net.bot.dingtalk.DefaultDingTalkBot` | `void setDefaultTitle(String defaultTitle)` | 设置 markdown默认title. |
| `com.feilong.net.bot.dingtalk.DefaultDingTalkBot` | `void setSecret(String secret)` | 自定义加签可选秘钥. 如果设置了, 将使用 钉钉加签规则: 把timestamp+"\n"+密钥当做签名字符串，使用HmacSHA256算法计算签名，然后进行Base64 encode，最后再把签名参数再进行urlEncode，得到最终的签名（需要使用UTF-8字符集） |
| `com.feilong.net.bot.dingtalk.DingTalkBot` | `boolean sendMessage(String title,String content,String... atMobiles)` | 消息, 支持markdown格式,也支持纯文本. |
| `com.feilong.net.bot.dingtalk.DingTalkBotBuilder` | `DingTalkBot newAsyncCatchExceptionDingTalkBot(String accessToken,String secret,String defaultTitle)` | 【原文待译】Builds the async catch exception. |
| `com.feilong.net.bot.dingtalk.DingTalkPushUtil` | `Boolean pushMessage(T botMessage,String accessToken,String secret)` | 发起POST请求时，必须将字符集编码设置成UTF-8 每个机器人每分钟最多发送20条。 消息发送太频繁会严重影响群成员的使用体验， 大量发消息的场景 (譬如系统监控报警) 可以将这些信息进行整合，通过markdown消息以摘要的形式发送到群里。 当前自定义机器人支持文本 (text)、 链接 (link)、 markdown(markdown)、 ActionCard、 FeedCard消息类型， 请根据自己的使用场景选择合适的消息类型，达到最好的展示样式。 详情参考：消息类型及数据格式。 自定义机器人发送消息时，可以通过手机号码指定“被@人列表”。 在“被@人列表”里面的人员收到该消息时，会… |
| `com.feilong.net.bot.dingtalk.DingtalkResponse` | `String getErrcode()` | 【原文待译】Gets the errcode. |
| `com.feilong.net.bot.dingtalk.DingtalkResponse` | `String getErrmsg()` | 【原文待译】Gets the errmsg. |
| `com.feilong.net.bot.dingtalk.DingtalkResponse` | `boolean getIsSuccess()` | 【原文待译】Gets the checks if is success. |
| `com.feilong.net.bot.dingtalk.DingtalkResponse` | `void setErrcode(String errcode)` | 【原文待译】Sets the errcode. |
| `com.feilong.net.bot.dingtalk.DingtalkResponse` | `void setErrmsg(String errmsg)` | 【原文待译】Sets the errmsg. |
