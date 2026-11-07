# com.feilong.net.bot.wxwork.message.news

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.net.bot.wxwork.message.news.Article`

```java
public class com.feilong.net.bot.wxwork.message.news.Article {
  public com.feilong.net.bot.wxwork.message.news.Article();
  public com.feilong.net.bot.wxwork.message.news.Article(java.lang.String, java.lang.String);
  public com.feilong.net.bot.wxwork.message.news.Article(java.lang.String, java.lang.String, java.lang.String, java.lang.String);
  public java.lang.String getTitle();
  public void setTitle(java.lang.String);
  public java.lang.String getDescription();
  public void setDescription(java.lang.String);
  public java.lang.String getUrl();
  public void setUrl(java.lang.String);
  public java.lang.String getPicurl();
  public void setPicurl(java.lang.String);
}
```

## `com.feilong.net.bot.wxwork.message.news.News`

```java
public class com.feilong.net.bot.wxwork.message.news.News {
  public com.feilong.net.bot.wxwork.message.news.News();
  public com.feilong.net.bot.wxwork.message.news.News(java.util.List<com.feilong.net.bot.wxwork.message.news.Article>);
  public java.util.List<com.feilong.net.bot.wxwork.message.news.Article> getArticles();
  public void setArticles(java.util.List<com.feilong.net.bot.wxwork.message.news.Article>);
}
```

## `com.feilong.net.bot.wxwork.message.news.WxworkNewsMessage`

```java
public class com.feilong.net.bot.wxwork.message.news.WxworkNewsMessage extends com.feilong.net.bot.message.BotMessage {
  public com.feilong.net.bot.wxwork.message.news.WxworkNewsMessage();
  public com.feilong.net.bot.wxwork.message.news.WxworkNewsMessage(com.feilong.net.bot.wxwork.message.news.News);
  public com.feilong.net.bot.wxwork.message.news.News getNews();
  public void setNews(com.feilong.net.bot.wxwork.message.news.News);
}
```
