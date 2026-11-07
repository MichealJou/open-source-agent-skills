# com.feilong.net.bot.wxwork

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.net.bot.wxwork.DefaultWxworkBot`

```java
public class com.feilong.net.bot.wxwork.DefaultWxworkBot extends com.feilong.net.bot.AbstractBot implements com.feilong.net.bot.wxwork.WxworkBot {
  public com.feilong.net.bot.wxwork.DefaultWxworkBot();
  public com.feilong.net.bot.wxwork.DefaultWxworkBot(java.lang.String);
  public com.feilong.net.bot.wxwork.message.WxworkResponse sendNewsMessage(com.feilong.net.bot.wxwork.message.news.Article...);
  public void setKey(java.lang.String);
  public java.lang.String getKey();
}
```

## `com.feilong.net.bot.wxwork.WxworkBot`

```java
public interface com.feilong.net.bot.wxwork.WxworkBot extends com.feilong.net.bot.Bot {
  public abstract com.feilong.net.bot.wxwork.message.WxworkResponse sendNewsMessage(com.feilong.net.bot.wxwork.message.news.Article...);
}
```

## `com.feilong.net.bot.wxwork.WxworkPushUtil`

```java
public class com.feilong.net.bot.wxwork.WxworkPushUtil {
  public com.feilong.net.bot.wxwork.WxworkPushUtil();
  public static <T extends com.feilong.net.bot.message.BotMessage> com.feilong.net.bot.wxwork.message.WxworkResponse pushMessage(T, java.lang.String);
}
```
