# com.feilong.net.bot.dingtalk

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.net.bot.dingtalk.DefaultDingTalkBot`

```java
public class com.feilong.net.bot.dingtalk.DefaultDingTalkBot extends com.feilong.net.bot.AbstractBot implements com.feilong.net.bot.dingtalk.DingTalkBot {
  public com.feilong.net.bot.dingtalk.DefaultDingTalkBot();
  public com.feilong.net.bot.dingtalk.DefaultDingTalkBot(java.lang.String);
  public com.feilong.net.bot.dingtalk.DefaultDingTalkBot(java.lang.String, java.lang.String);
  public boolean sendMessage(java.lang.String, java.lang.String, java.lang.String...);
  public void setAccessToken(java.lang.String);
  public void setSecret(java.lang.String);
  public void setDefaultTitle(java.lang.String);
  public java.lang.String getKey();
}
```

## `com.feilong.net.bot.dingtalk.DingTalkBot`

```java
public interface com.feilong.net.bot.dingtalk.DingTalkBot extends com.feilong.net.bot.Bot {
  public abstract boolean sendMessage(java.lang.String, java.lang.String, java.lang.String...);
}
```

## `com.feilong.net.bot.dingtalk.DingTalkBotBuilder`

```java
public class com.feilong.net.bot.dingtalk.DingTalkBotBuilder {
  public com.feilong.net.bot.dingtalk.DingTalkBotBuilder();
  public static com.feilong.net.bot.dingtalk.DingTalkBot newAsyncCatchExceptionDingTalkBot(java.lang.String, java.lang.String, java.lang.String);
}
```

## `com.feilong.net.bot.dingtalk.DingTalkPushUtil`

```java
public class com.feilong.net.bot.dingtalk.DingTalkPushUtil {
  public com.feilong.net.bot.dingtalk.DingTalkPushUtil();
  public static <T extends com.feilong.net.bot.message.BotMessage> java.lang.Boolean pushMessage(T, java.lang.String, java.lang.String);
}
```

## `com.feilong.net.bot.dingtalk.DingtalkResponse`

```java
public class com.feilong.net.bot.dingtalk.DingtalkResponse {
  public com.feilong.net.bot.dingtalk.DingtalkResponse();
  public boolean getIsSuccess();
  public java.lang.String getErrcode();
  public void setErrcode(java.lang.String);
  public java.lang.String getErrmsg();
  public void setErrmsg(java.lang.String);
}
```
