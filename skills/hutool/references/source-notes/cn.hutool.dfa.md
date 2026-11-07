# cn.hutool.dfa

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.dfa.FoundWord` | `String getFoundWord()` | 获取单词匹配到的内容，即文中的单词 |
| `cn.hutool.dfa.FoundWord` | `String getWord()` | 获取生效的单词，即单词树中的词 |
| `cn.hutool.dfa.FoundWord` | `String toString()` | 默认的，只输出匹配到的关键字 |
| `cn.hutool.dfa.SensitiveProcessor` | `String process(FoundWord foundWord)` | 敏感词过滤处理 |
| `cn.hutool.dfa.SensitiveUtil` | `FoundWord getFoundFirstSensitive(Object obj)` | 查找敏感词，返回找到的第一个敏感词 |
| `cn.hutool.dfa.SensitiveUtil` | `FoundWord getFoundFirstSensitive(String text)` | 查找敏感词，返回找到的第一个敏感词 |
| `cn.hutool.dfa.SensitiveUtil` | `List<FoundWord> getFoundAllSensitive(Object bean)` | 查找敏感词，返回找到的所有敏感词 |
| `cn.hutool.dfa.SensitiveUtil` | `List<FoundWord> getFoundAllSensitive(Object bean,boolean isDensityMatch,boolean isGreedMatch)` | 查找敏感词，返回找到的所有敏感词 密集匹配原则：假如关键词有 ab,b，文本是abab，将匹配 [ab,b,ab] 贪婪匹配（最长匹配）原则：假如关键字a,ab，最长匹配将匹配[a, ab] |
| `cn.hutool.dfa.SensitiveUtil` | `List<FoundWord> getFoundAllSensitive(String text)` | 查找敏感词，返回找到的所有敏感词 |
| `cn.hutool.dfa.SensitiveUtil` | `List<FoundWord> getFoundAllSensitive(String text,boolean isDensityMatch,boolean isGreedMatch)` | 查找敏感词，返回找到的所有敏感词 密集匹配原则：假如关键词有 ab,b，文本是abab，将匹配 [ab,b,ab] 贪婪匹配（最长匹配）原则：假如关键字a,ab，最长匹配将匹配[a, ab] |
| `cn.hutool.dfa.SensitiveUtil` | `String sensitiveFilter(String text)` | 处理过滤文本中的敏感词，默认替换成* |
| `cn.hutool.dfa.SensitiveUtil` | `String sensitiveFilter(String text,boolean isGreedMatch,SensitiveProcessor sensitiveProcessor)` | 处理过滤文本中的敏感词，默认替换成* |
| `cn.hutool.dfa.SensitiveUtil` | `T sensitiveFilter(T bean,boolean isGreedMatch,SensitiveProcessor sensitiveProcessor)` | 敏感词过滤 |
| `cn.hutool.dfa.SensitiveUtil` | `boolean containsSensitive(Object obj)` | 是否包含敏感词 |
| `cn.hutool.dfa.SensitiveUtil` | `boolean containsSensitive(String text)` | 是否包含敏感词 |
| `cn.hutool.dfa.SensitiveUtil` | `boolean isInited()` | @return 是否已经被初始化 |
| `cn.hutool.dfa.SensitiveUtil` | `void init(Collection<String> sensitiveWords)` | 初始化敏感词树 |
| `cn.hutool.dfa.SensitiveUtil` | `void init(String sensitiveWords,boolean isAsync)` | 初始化敏感词树，使用逗号分隔每个单词 |
| `cn.hutool.dfa.SensitiveUtil` | `void init(String sensitiveWords,char separator,boolean isAsync)` | 初始化敏感词树 |
| `cn.hutool.dfa.SensitiveUtil` | `void init(final Collection<String> sensitiveWords,boolean isAsync)` | 初始化敏感词树 |
| `cn.hutool.dfa.SensitiveUtil` | `void setCharFilter(Filter<Character> charFilter)` | 设置字符过滤规则，通过定义字符串过滤规则，过滤不需要的字符 当accept为false时，此字符不参与匹配 |
| `cn.hutool.dfa.StopChar` | `boolean isNotStopChar(char ch)` | 是否为合法字符（待处理字符） |
| `cn.hutool.dfa.StopChar` | `boolean isStopChar(char ch)` | 判断指定的词是否是不处理的词。 如果参数为空，则返回true，因为空也属于不处理的字符。 |
| `cn.hutool.dfa.WordTree` | `FoundWord matchWord(String text)` | 获得第一个匹配的关键字 |
| `cn.hutool.dfa.WordTree` | `List<FoundWord> matchAllWords(String text)` | 找出所有匹配的关键字 |
| `cn.hutool.dfa.WordTree` | `List<FoundWord> matchAllWords(String text,int limit)` | 找出所有匹配的关键字 |
| `cn.hutool.dfa.WordTree` | `List<FoundWord> matchAllWords(String text,int limit,boolean isDensityMatch,boolean isGreedMatch)` | 找出所有匹配的关键字 密集匹配原则：假如关键词有 ab,b，文本是abab，将匹配 [ab,b,ab] 贪婪匹配（最长匹配）原则：假如关键字a,ab，最长匹配将匹配[a, ab] |
| `cn.hutool.dfa.WordTree` | `List<String> matchAll(String text)` | 找出所有匹配的关键字 |
| `cn.hutool.dfa.WordTree` | `List<String> matchAll(String text,int limit)` | 找出所有匹配的关键字 |
| `cn.hutool.dfa.WordTree` | `List<String> matchAll(String text,int limit,boolean isDensityMatch,boolean isGreedMatch)` | 找出所有匹配的关键字 密集匹配原则：假如关键词有 ab,b，文本是abab，将匹配 [ab,b,ab] 贪婪匹配（最长匹配）原则：假如关键字a,ab，最长匹配将匹配[a, ab] |
| `cn.hutool.dfa.WordTree` | `String match(String text)` | 获得第一个匹配的关键字 |
| `cn.hutool.dfa.WordTree` | `WordTree addWord(String word)` | 添加单词，使用默认类型 |
| `cn.hutool.dfa.WordTree` | `WordTree addWords(Collection<String> words)` | 增加一组单词 |
| `cn.hutool.dfa.WordTree` | `WordTree addWords(String... words)` | 增加一组单词 |
| `cn.hutool.dfa.WordTree` | `WordTree setCharFilter(Filter<Character> charFilter)` | 设置字符过滤规则，通过定义字符串过滤规则，过滤不需要的字符 当accept为false时，此字符不参与匹配 |
| `cn.hutool.dfa.WordTree` | `boolean isMatch(String text)` | 指定文本是否包含树中的词 |
| `cn.hutool.dfa.WordTree` | `void clear()` | 清除所有的词, 此方法调用后, wordTree 将被清空 endCharacterSet 也将清空 |
