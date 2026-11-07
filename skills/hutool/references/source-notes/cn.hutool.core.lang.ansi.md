# cn.hutool.core.lang.ansi

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.lang.ansi.Ansi8BitColor` | `Ansi8BitColor background(int code)` | 背景色ANSI颜色实例 |
| `cn.hutool.core.lang.ansi.Ansi8BitColor` | `Ansi8BitColor foreground(int code)` | 前景色ANSI颜色实例 |
| `cn.hutool.core.lang.ansi.Ansi8BitColor` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.ansi.Ansi8BitColor` | `boolean equals(Object obj)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.ansi.Ansi8BitColor` | `int getCode()` | 获取颜色代码(0-255) |
| `cn.hutool.core.lang.ansi.Ansi8BitColor` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.ansi.AnsiBackground` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.ansi.AnsiBackground` | `int getCode()` | 获取ANSI颜色代码 |
| `cn.hutool.core.lang.ansi.AnsiColor` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.ansi.AnsiColor` | `int getCode()` | 获取ANSI颜色代码 |
| `cn.hutool.core.lang.ansi.AnsiColorWrapper` | `AnsiElement toAnsiElement(ForeOrBack foreOrBack)` | 转换为 AnsiElement 实例 |
| `cn.hutool.core.lang.ansi.AnsiColorWrapper` | `boolean equals(Object o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.ansi.AnsiColorWrapper` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.ansi.AnsiColors` | `AnsiColorWrapper findClosest(Color color)` | 找到最接近给定 AWT Color 的 AnsiColorWrapper ANSI 颜色包装 实例。 |
| `cn.hutool.core.lang.ansi.AnsiColors$BitDepth` | `BitDepth of(int bits)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.ansi.AnsiElement` | `String toString()` | @return ANSI转义编码 |
| `cn.hutool.core.lang.ansi.AnsiElement` | `int getCode()` | 获取ANSI代码，默认返回-1 |
| `cn.hutool.core.lang.ansi.AnsiEncoder` | `String encode(Object... elements)` | 创建ANSI字符串，参数中的AnsiElement会被转换为编码形式。 |
| `cn.hutool.core.lang.ansi.AnsiStyle` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.ansi.AnsiStyle` | `int getCode()` | 获取ANSI文本样式风格代码 |
