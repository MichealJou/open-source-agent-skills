# com.feilong.net.bot.wxwork.message.news

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.net.bot.wxwork.message.news.Article` | `String getDescription()` | 获得 否 描述，不超过512个字节，超过会自动截断. |
| `com.feilong.net.bot.wxwork.message.news.Article` | `String getPicurl()` | 获得 否 图文消息的图片链接，支持JPG、PNG格式，较好的效果为大图 1068*455，小图150*150。. |
| `com.feilong.net.bot.wxwork.message.news.Article` | `String getTitle()` | 获得 是 标题，不超过128个字节，超过会自动截断. |
| `com.feilong.net.bot.wxwork.message.news.Article` | `String getUrl()` | 获得 是 点击后跳转的链接。. |
| `com.feilong.net.bot.wxwork.message.news.Article` | `void setDescription(String description)` | 设置 否 描述，不超过512个字节，超过会自动截断. |
| `com.feilong.net.bot.wxwork.message.news.Article` | `void setPicurl(String picurl)` | 设置 否 图文消息的图片链接，支持JPG、PNG格式，较好的效果为大图 1068*455，小图150*150。. |
| `com.feilong.net.bot.wxwork.message.news.Article` | `void setTitle(String title)` | 设置 是 标题，不超过128个字节，超过会自动截断. |
| `com.feilong.net.bot.wxwork.message.news.Article` | `void setUrl(String url)` | 设置 是 点击后跳转的链接。. |
| `com.feilong.net.bot.wxwork.message.news.News` | `List<Article> getArticles()` | 【原文待译】Gets the articles. |
| `com.feilong.net.bot.wxwork.message.news.News` | `void setArticles(List<Article> articles)` | 【原文待译】Sets the articles. |
| `com.feilong.net.bot.wxwork.message.news.WxworkNewsMessage` | `News getNews()` | 【原文待译】Gets the news. |
| `com.feilong.net.bot.wxwork.message.news.WxworkNewsMessage` | `void setNews(News news)` | 【原文待译】Sets the news. |
