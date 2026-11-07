# cn.hutool.extra.emoji

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.emoji.EmojiUtil`

```java
public class cn.hutool.extra.emoji.EmojiUtil {
  public cn.hutool.extra.emoji.EmojiUtil();
  public static boolean isEmoji(java.lang.String);
  public static boolean containsEmoji(java.lang.String);
  public static java.util.Set<com.vdurmont.emoji.Emoji> getByTag(java.lang.String);
  public static com.vdurmont.emoji.Emoji get(java.lang.String);
  public static java.lang.String toUnicode(java.lang.String);
  public static java.lang.String toAlias(java.lang.String);
  public static java.lang.String toAlias(java.lang.String, com.vdurmont.emoji.EmojiParser$FitzpatrickAction);
  public static java.lang.String toHtmlHex(java.lang.String);
  public static java.lang.String toHtml(java.lang.String);
  public static java.lang.String toHtml(java.lang.String, boolean);
  public static java.lang.String removeAllEmojis(java.lang.String);
  public static java.util.List<java.lang.String> extractEmojis(java.lang.String);
}
```
