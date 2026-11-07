# com.feilong.net.bot.dingtalk.message

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.net.bot.dingtalk.message.At` | `List<String> getAtUserIds()` | 获得 被@人的用户userid . 发送消息是基于userid，这个userid跟钉钉账号还不一样，是钉钉开发者平台的userid。 可以通过钉钉账号的信息来获取，这里使用的是get_userid用手机号获取方式； |
| `com.feilong.net.bot.dingtalk.message.At` | `String[] getAtMobiles()` | 获得 被@人的手机号。 注意在text内容里要有@人的手机号. |
| `com.feilong.net.bot.dingtalk.message.At` | `boolean getIsAtAll()` | 获得 是否@所有人. |
| `com.feilong.net.bot.dingtalk.message.At` | `void setAtMobiles(String... atMobiles)` | 设置 被@人的手机号。 注意在text内容里要有@人的手机号. |
| `com.feilong.net.bot.dingtalk.message.At` | `void setAtUserIds(List<String> atUserIds)` | 设置 被@人的用户userid . 发送消息是基于userid，这个userid跟钉钉账号还不一样，是钉钉开发者平台的userid。 可以通过钉钉账号的信息来获取，这里使用的是get_userid用手机号获取方式； |
| `com.feilong.net.bot.dingtalk.message.At` | `void setIsAtAll(boolean isAtAll)` | 设置 是否@所有人. |
