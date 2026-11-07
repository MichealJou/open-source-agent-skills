# cn.hutool.extra.tokenizer

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.extra.tokenizer.TokenizerEngine` | `Result parse(CharSequence text)` | 文本分词处理接口，通过实现此接口完成分词，产生分词结果 |
| `cn.hutool.extra.tokenizer.TokenizerUtil` | `TokenizerEngine createEngine()` | 根据用户引入的分词引擎jar，自动创建对应的分词引擎对象 |
| `cn.hutool.extra.tokenizer.Word` | `String getText()` | 获取单词文本 |
| `cn.hutool.extra.tokenizer.Word` | `int getEndOffset()` | 获取本词的结束位置 |
| `cn.hutool.extra.tokenizer.Word` | `int getStartOffset()` | 获取本词的起始位置 |
