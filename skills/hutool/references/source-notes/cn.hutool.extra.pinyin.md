# cn.hutool.extra.pinyin

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.extra.pinyin.PinyinEngine` | `String getFirstLetter(String str,String separator)` | 将输入字符串转为拼音首字母，其它字符原样返回 |
| `cn.hutool.extra.pinyin.PinyinEngine` | `String getPinyin(String str,String separator)` | 获取字符串对应的完整拼音，非中文返回原字符 |
| `cn.hutool.extra.pinyin.PinyinEngine` | `String getPinyin(String str,String separator,boolean tone)` | 获取字符串对应的完整拼音，非中文返回原字符 |
| `cn.hutool.extra.pinyin.PinyinEngine` | `String getPinyin(char c)` | 如果c为汉字，则返回大写拼音；如果c不是汉字，则返回String.valueOf(c) |
| `cn.hutool.extra.pinyin.PinyinEngine` | `String getPinyin(char c,boolean tone)` | 如果c为汉字，则返回大写拼音；如果c不是汉字，则返回String.valueOf(c) |
| `cn.hutool.extra.pinyin.PinyinEngine` | `char getFirstLetter(char c)` | 将输入字符串转为拼音首字母，其它字符原样返回 |
| `cn.hutool.extra.pinyin.PinyinUtil` | `PinyinEngine getEngine()` | 获得全局单例的拼音引擎 |
| `cn.hutool.extra.pinyin.PinyinUtil` | `String getFirstLetter(String str,String separator)` | 将输入字符串转为拼音首字母，其它字符原样返回 |
| `cn.hutool.extra.pinyin.PinyinUtil` | `String getPinyin(String str)` | 将输入字符串转为拼音，每个字之间的拼音使用空格分隔 |
| `cn.hutool.extra.pinyin.PinyinUtil` | `String getPinyin(String str,String separator)` | 将输入字符串转为拼音，以字符为单位插入分隔符 |
| `cn.hutool.extra.pinyin.PinyinUtil` | `String getPinyin(char c)` | 如果c为汉字，则返回大写拼音；如果c不是汉字，则返回String.valueOf(c) |
| `cn.hutool.extra.pinyin.PinyinUtil` | `String getPinyin(final String str,boolean tone)` | 将输入字符串转为拼音，每个字之间的拼音使用空格分隔 |
| `cn.hutool.extra.pinyin.PinyinUtil` | `String getPinyin(final String str,final String separator,boolean tone)` | 将输入字符串转为拼音，以字符为单位插入分隔符 |
| `cn.hutool.extra.pinyin.PinyinUtil` | `String getPinyin(final char c,boolean tone)` | 如果c为汉字，则返回大写拼音；如果c不是汉字，则返回String.valueOf(c) |
| `cn.hutool.extra.pinyin.PinyinUtil` | `boolean isChinese(char c)` | 是否为中文字符 |
| `cn.hutool.extra.pinyin.PinyinUtil` | `char getFirstLetter(char c)` | 将输入字符串转为拼音首字母，其它字符原样返回 |
