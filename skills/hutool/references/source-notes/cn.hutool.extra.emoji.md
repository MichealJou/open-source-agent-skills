# cn.hutool.extra.emoji

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.extra.emoji.EmojiUtil` | `Emoji get(String alias)` | 通过别名获取Emoji |
| `cn.hutool.extra.emoji.EmojiUtil` | `List<String> extractEmojis(String str)` | 提取字符串中所有的Emoji Unicode |
| `cn.hutool.extra.emoji.EmojiUtil` | `Set<Emoji> getByTag(String tag)` | 通过tag方式获取对应的所有Emoji表情 |
| `cn.hutool.extra.emoji.EmojiUtil` | `String removeAllEmojis(String str)` | 去除字符串中所有的Emoji Unicode字符 |
| `cn.hutool.extra.emoji.EmojiUtil` | `String toAlias(String str)` | 将字符串中的Unicode Emoji字符转换为别名表现形式（两个":"包围的格式） 例如： 😄 转换为 :smile: FitzpatrickAction参数被设置为FitzpatrickAction#PARSE，则别名后会增加"\|"并追加fitzpatrick类型 例如： 👦🏿 转换为 :boy\|type_6: FitzpatrickAction参数被设置为FitzpatrickAction#REMOVE，则别名后的"\|"和类型将被去除 例如： 👦🏿 转换为 :boy: FitzpatrickAction参数被设置为FitzpatrickAction#IGNORE，则别名后的类型将被忽略 … |
| `cn.hutool.extra.emoji.EmojiUtil` | `String toAlias(String str,FitzpatrickAction fitzpatrickAction)` | 将字符串中的Unicode Emoji字符转换为别名表现形式（两个":"包围的格式），别名后会增加"\|"并追加fitzpatrick类型 例如： 👦🏿 转换为 :boy\|type_6: |
| `cn.hutool.extra.emoji.EmojiUtil` | `String toHtml(String str)` | 将字符串中的Unicode Emoji字符转换为HTML表现形式（Hex方式） 例如： 👦🏿 转换为 &#128102; |
| `cn.hutool.extra.emoji.EmojiUtil` | `String toHtml(String str,boolean isHex)` | 将字符串中的Unicode Emoji字符转换为HTML表现形式，例如： |
| `cn.hutool.extra.emoji.EmojiUtil` | `String toHtmlHex(String str)` | 将字符串中的Unicode Emoji字符转换为HTML 16进制表现形式 例如： 👦🏿 转换为 &#x1f466; |
| `cn.hutool.extra.emoji.EmojiUtil` | `String toUnicode(String str)` | 将子串中的Emoji别名（两个":"包围的格式）和其HTML表示形式替换为为Unicode Emoji符号 例如： |
| `cn.hutool.extra.emoji.EmojiUtil` | `boolean containsEmoji(String str)` | 是否包含Emoji表情的Unicode符 |
| `cn.hutool.extra.emoji.EmojiUtil` | `boolean isEmoji(String str)` | 是否为Emoji表情的Unicode符 |
