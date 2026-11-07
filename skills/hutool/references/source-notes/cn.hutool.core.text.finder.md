# cn.hutool.core.text.finder

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.text.finder.CharFinder` | `int end(int start)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.finder.CharFinder` | `int start(int from)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.finder.CharMatcherFinder` | `int end(int start)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.finder.CharMatcherFinder` | `int start(int from)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.finder.Finder` | `Finder reset()` | 复位查找器，用于重用对象 |
| `cn.hutool.core.text.finder.Finder` | `int end(int start)` | 返回结束位置，即最后一个字符后的位置（不包含） |
| `cn.hutool.core.text.finder.Finder` | `int start(int from)` | 返回开始位置，即起始字符位置（包含），未找到返回-1 |
| `cn.hutool.core.text.finder.LengthFinder` | `int end(int start)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.finder.LengthFinder` | `int start(int from)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.finder.PatternFinder` | `PatternFinder reset()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.finder.PatternFinder` | `TextFinder setNegative(boolean negative)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.finder.PatternFinder` | `TextFinder setText(CharSequence text)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.finder.PatternFinder` | `int end(int start)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.finder.PatternFinder` | `int start(int from)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.finder.StrFinder` | `int end(int start)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.finder.StrFinder` | `int start(int from)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.finder.TextFinder` | `TextFinder setEndIndex(int endIndex)` | 设置查找的结束位置 如果从前向后查找，结束位置最大为text.length() 如果从后向前，结束位置为-1 |
| `cn.hutool.core.text.finder.TextFinder` | `TextFinder setNegative(boolean negative)` | 设置是否反向查找，true表示从后向前查找 |
| `cn.hutool.core.text.finder.TextFinder` | `TextFinder setText(CharSequence text)` | 设置被查找的文本 |
