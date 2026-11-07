# cn.hutool.core.text

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.text.ASCIIStrCache` | `String toString(char c)` | 字符转为字符串 如果为ASCII字符，使用缓存 |
| `cn.hutool.core.text.AntPathMatcher` | `AntPathMatcher setCachePatterns(boolean cachePatterns)` | 【原文待译】Specify whether to cache parsed pattern metadata for patterns passed into this matcher's #match method. A value of true activates an unlimited pattern cache; a value of false turns the pattern cache off completely. Default is for the cache to be on, but with the variant to automatically turn it off … |
| `cn.hutool.core.text.AntPathMatcher` | `AntPathMatcher setCaseSensitive(boolean caseSensitive)` | 设置是否大小写敏感，默认为true |
| `cn.hutool.core.text.AntPathMatcher` | `AntPathMatcher setPathSeparator(String pathSeparator)` | 设置路径分隔符 |
| `cn.hutool.core.text.AntPathMatcher` | `AntPathMatcher setTrimTokens(boolean trimTokens)` | 设置是否去除路径节点两边的空白符，默认为false |
| `cn.hutool.core.text.AntPathMatcher` | `Comparator<String> getPatternComparator(String path)` | 【原文待译】Given a full path, returns a Comparator suitable for sorting patterns in order of explicitness. This Comparator will {@linkplain List#sort(Comparator) sort} a list so that more specific patterns (without URI templates or wild cards) come before generic patterns. So given a list with the following pa… |
| `cn.hutool.core.text.AntPathMatcher` | `Map<String, String> extractUriTemplateVariables(String pattern,String path)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.AntPathMatcher` | `String combine(String pattern1,String pattern2)` | 【原文待译】Combine two patterns into a new pattern. This implementation simply concatenates the two patterns, unless the first pattern contains a file extension match (e.g., *.html). In that case, the second pattern will be merged into the first. Otherwise, an IllegalArgumentException will be thrown. Examples … |
| `cn.hutool.core.text.AntPathMatcher` | `String extractPathWithinPattern(String pattern,String path)` | 【原文待译】Given a pattern and a full path, determine the pattern-mapped part. For example: '/docs/cvs/commit.html' and '/docs/cvs/commit.html → '' '/docs/*' and '/docs/cvs/commit → 'cvs/commit' '/docs/cvs/*.html' and '/docs/cvs/commit.html → 'commit.html' '/docs/**' and '/docs/cvs/commit → 'cvs/commit' '/docs… |
| `cn.hutool.core.text.AntPathMatcher` | `boolean isPattern(String path)` | 判断给定路径是否是表达式 |
| `cn.hutool.core.text.AntPathMatcher` | `boolean match(String pattern,String path)` | 给定路径是否匹配表达式 |
| `cn.hutool.core.text.AntPathMatcher` | `boolean matchStart(String pattern,String path)` | 前置部分匹配 |
| `cn.hutool.core.text.CharSequenceUtil` | `ByteBuffer byteBuffer(CharSequence str,String charset)` | 字符串转换为byteBuffer |
| `cn.hutool.core.text.CharSequenceUtil` | `CharSequence commonPrefix(CharSequence str1,CharSequence str2)` | 字符串1和字符串2的公共前缀 |
| `cn.hutool.core.text.CharSequenceUtil` | `CharSequence commonSuffix(CharSequence str1,CharSequence str2)` | 字符串1和字符串2的公共后缀 |
| `cn.hutool.core.text.CharSequenceUtil` | `List<R> split(CharSequence str,char separator,int limit,boolean ignoreEmpty,Function<String, R> mapping)` | 切分字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `List<String> split(CharSequence str,CharSequence separator)` | 切分字符串，如果分隔符不存在则返回原字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `List<String> split(CharSequence str,CharSequence separator,boolean isTrim,boolean ignoreEmpty)` | 切分字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `List<String> split(CharSequence str,CharSequence separator,int limit,boolean isTrim,boolean ignoreEmpty)` | 切分字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `List<String> split(CharSequence str,char separator)` | 切分字符串 a#b#c =》 [a,b,c] a##b#c =》 [a,"",b,c] |
| `cn.hutool.core.text.CharSequenceUtil` | `List<String> split(CharSequence str,char separator,boolean isTrim,boolean ignoreEmpty)` | 切分字符串，不限制分片数量 |
| `cn.hutool.core.text.CharSequenceUtil` | `List<String> split(CharSequence str,char separator,int limit)` | 切分字符串，不去除切分后每个元素两边的空白符，不去除空白项 |
| `cn.hutool.core.text.CharSequenceUtil` | `List<String> split(CharSequence str,char separator,int limit,boolean isTrim,boolean ignoreEmpty)` | 切分字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `List<String> splitTrim(CharSequence str,CharSequence separator)` | 切分字符串，去除切分后每个元素两边的空白符，去除空白项 |
| `cn.hutool.core.text.CharSequenceUtil` | `List<String> splitTrim(CharSequence str,CharSequence separator,int limit)` | 切分字符串，去除切分后每个元素两边的空白符，去除空白项 |
| `cn.hutool.core.text.CharSequenceUtil` | `List<String> splitTrim(CharSequence str,char separator)` | 切分字符串，去除切分后每个元素两边的空白符，去除空白项 |
| `cn.hutool.core.text.CharSequenceUtil` | `List<String> splitTrim(CharSequence str,char separator,int limit)` | 切分字符串，去除切分后每个元素两边的空白符，去除空白项 |
| `cn.hutool.core.text.CharSequenceUtil` | `StrBuilder strBuilder(CharSequence... strs)` | 创建StrBuilder对象 |
| `cn.hutool.core.text.CharSequenceUtil` | `String addPrefixIfNot(CharSequence str,CharSequence prefix)` | 如果给定字符串不是以prefix开头的，在开头补充 prefix |
| `cn.hutool.core.text.CharSequenceUtil` | `String addSuffixIfNot(CharSequence str,CharSequence suffix)` | 如果给定字符串不是以suffix结尾的，在尾部补充 suffix |
| `cn.hutool.core.text.CharSequenceUtil` | `String appendIfMissing(CharSequence str,CharSequence suffix,CharSequence... suffixes)` | 如果给定字符串不是以给定的一个或多个字符串为结尾，则在尾部添加结尾字符串 不忽略大小写 |
| `cn.hutool.core.text.CharSequenceUtil` | `String appendIfMissing(CharSequence str,CharSequence suffix,boolean ignoreCase,CharSequence... testSuffixes)` | 如果给定字符串不是以给定的一个或多个字符串为结尾，则在尾部添加结尾字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String appendIfMissingIgnoreCase(CharSequence str,CharSequence suffix,CharSequence... suffixes)` | 如果给定字符串不是以给定的一个或多个字符串为结尾，则在尾部添加结尾字符串 忽略大小写 |
| `cn.hutool.core.text.CharSequenceUtil` | `String blankToDefault(CharSequence str,String defaultStr)` | 如果字符串是null或者""或者空白，则返回指定默认字符串，否则返回字符串本身。 |
| `cn.hutool.core.text.CharSequenceUtil` | `String brief(CharSequence str,int maxLength)` | 将给定字符串，变成 "xxx...xxx" 形式的字符串 abcdefgh 9 -》 abcdefgh abcdefgh 8 -》 abcdefgh abcdefgh 7 -》 ab...gh abcdefgh 6 -》 ab...h abcdefgh 5 -》 a...h abcdefgh 4 -》 a..h abcdefgh 3 -》 a.h abcdefgh 2 -》 a. abcdefgh 1 -》 a abcdefgh 0 -》 abcdefgh abcdefgh -1 -》 abcdefgh |
| `cn.hutool.core.text.CharSequenceUtil` | `String center(CharSequence str,final int size)` | 居中字符串，两边补充空格符，如果指定长度小于字符串，则返回原字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String center(CharSequence str,final int size,CharSequence padStr)` | 居中字符串，两边补充指定字符串，如果指定长度小于字符串，则返回原字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String center(CharSequence str,final int size,char padChar)` | 居中字符串，两边补充指定字符，如果指定长度小于字符串，则返回原字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String cleanBlank(CharSequence str)` | 清理空白字符 |
| `cn.hutool.core.text.CharSequenceUtil` | `String concat(boolean isNullToEmpty,CharSequence... strs)` | 连接多个字符串为一个 |
| `cn.hutool.core.text.CharSequenceUtil` | `String desensitized(CharSequence str,DesensitizedUtil.DesensitizedType desensitizedType)` | 脱敏，使用默认的脱敏策略 |
| `cn.hutool.core.text.CharSequenceUtil` | `String emptyIfNull(CharSequence str)` | 当给定字符串为null时，转换为Empty |
| `cn.hutool.core.text.CharSequenceUtil` | `String emptyToDefault(CharSequence str,String defaultStr)` | 如果字符串是null或者""，则返回指定默认字符串，否则返回字符串本身。 |
| `cn.hutool.core.text.CharSequenceUtil` | `String emptyToNull(CharSequence str)` | 当给定字符串为空字符串时，转换为null |
| `cn.hutool.core.text.CharSequenceUtil` | `String filter(CharSequence str,final Filter<Character> filter)` | 过滤字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String fixLength(CharSequence str,char fixedChar,int length)` | 在给定字符串末尾填充指定字符，以达到给定长度 如果字符串本身的长度大于等于length，返回原字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String format(CharSequence template,Object... params)` | 格式化文本, {} 表示占位符 此方法只是简单将占位符 {} 按照顺序替换为参数 如果想输出 {} 使用 \\转义 { 即可，如果想输出 {} 之前的 \ 使用双转义符 \\\\ 即可 例： 通常使用：format("this is {} for {}", "a", "b") =》 this is a for b 转义{}： format("this is \\{} for {}", "a", "b") =》 this is {} for a 转义\： format("this is \\\\{} for {}", "a", "b") =》 this is \a for b |
| `cn.hutool.core.text.CharSequenceUtil` | `String genGetter(CharSequence fieldName)` | 生成get方法名 |
| `cn.hutool.core.text.CharSequenceUtil` | `String genSetter(CharSequence fieldName)` | 生成set方法名 例如：name 返回 setName |
| `cn.hutool.core.text.CharSequenceUtil` | `String getContainsStr(CharSequence str,CharSequence... testStrs)` | 查找指定字符串是否包含指定字符串列表中的任意一个字符串，如果包含返回找到的第一个字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String getContainsStrIgnoreCase(CharSequence str,CharSequence... testStrs)` | 查找指定字符串是否包含指定字符串列表中的任意一个字符串，如果包含返回找到的第一个字符串 忽略大小写 |
| `cn.hutool.core.text.CharSequenceUtil` | `String getGeneralField(CharSequence getOrSetMethodName)` | 获得set或get或is方法对应的标准属性名 例如：setName 返回 name |
| `cn.hutool.core.text.CharSequenceUtil` | `String hide(CharSequence str,int startInclude,int endExclude)` | 替换指定字符串的指定区间内字符为"*" 俗称：脱敏功能，后面其他功能，可以见：DesensitizedUtil(脱敏工具类) |
| `cn.hutool.core.text.CharSequenceUtil` | `String indexedFormat(CharSequence pattern,Object... arguments)` | 有序的格式化文本，使用{number}做为占位符 通常使用：format("this is {0} for {1}", "a", "b") =》 this is a for b |
| `cn.hutool.core.text.CharSequenceUtil` | `String join(CharSequence conjunction,Iterable<T> iterable)` | 以 conjunction 为分隔符将多个对象转换为字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String join(CharSequence conjunction,Object... objs)` | 以 conjunction 为分隔符将多个对象转换为字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String lowerFirst(CharSequence str)` | 小写首字母 例如：str = Name, return name |
| `cn.hutool.core.text.CharSequenceUtil` | `String maxLength(CharSequence string,int length)` | 限制字符串长度，如果超过指定长度，截取指定长度并在末尾加"..." |
| `cn.hutool.core.text.CharSequenceUtil` | `String move(CharSequence str,int startInclude,int endExclude,int moveLength)` | 循环位移指定位置的字符串为指定距离 当moveLength大于0向右位移，小于0向左位移，0不位移 当moveLength大于字符串长度时采取循环位移策略，即位移到头后从头（尾）位移，例如长度为10，位移13则表示位移3 |
| `cn.hutool.core.text.CharSequenceUtil` | `String normalize(CharSequence str)` | 对字符串归一化处理，如 "Á" 可以使用 "u00C1"或 "u0041u0301"表示，实际测试中两个字符串并不equals 因此使用此方法归一为一种表示形式，默认按照W3C通常建议的，在NFC中交换文本。 |
| `cn.hutool.core.text.CharSequenceUtil` | `String nullToDefault(CharSequence str,String defaultStr)` | 如果字符串是 null，则返回指定默认字符串，否则返回字符串本身。 |
| `cn.hutool.core.text.CharSequenceUtil` | `String nullToEmpty(CharSequence str)` | 当给定字符串为null时，转换为Empty |
| `cn.hutool.core.text.CharSequenceUtil` | `String padAfter(CharSequence str,int length,CharSequence padStr)` | 补充字符串以满足最小长度 |
| `cn.hutool.core.text.CharSequenceUtil` | `String padAfter(CharSequence str,int length,char padChar)` | 补充字符串以满足最小长度，如果提供的字符串大于指定长度，截断之 |
| `cn.hutool.core.text.CharSequenceUtil` | `String padPre(CharSequence str,int length,CharSequence padStr)` | 补充字符串以满足指定长度，如果提供的字符串大于指定长度，截断之 同：leftPad (org.apache.commons.lang3.leftPad) |
| `cn.hutool.core.text.CharSequenceUtil` | `String padPre(CharSequence str,int length,char padChar)` | 补充字符串以满足最小长度，如果提供的字符串大于指定长度，截断之 同：leftPad (org.apache.commons.lang3.leftPad) |
| `cn.hutool.core.text.CharSequenceUtil` | `String prependIfMissing(CharSequence str,CharSequence prefix,CharSequence... prefixes)` | 如果给定字符串不是以给定的一个或多个字符串为开头，则在首部添加起始字符串 不忽略大小写 |
| `cn.hutool.core.text.CharSequenceUtil` | `String prependIfMissing(CharSequence str,CharSequence prefix,boolean ignoreCase,CharSequence... prefixes)` | 如果给定字符串不是以给定的一个或多个字符串为开头，则在首部添加起始字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String prependIfMissingIgnoreCase(CharSequence str,CharSequence prefix,CharSequence... prefixes)` | 如果给定字符串不是以给定的一个或多个字符串为开头，则在首部添加起始字符串 忽略大小写 |
| `cn.hutool.core.text.CharSequenceUtil` | `String removeAll(CharSequence str,CharSequence strToRemove)` | 移除字符串中所有给定字符串 例：removeAll("aa-bb-cc-dd", "-") =》 aabbccdd |
| `cn.hutool.core.text.CharSequenceUtil` | `String removeAll(CharSequence str,char... chars)` | 去除字符串中指定的多个字符，如有多个则全部去除 |
| `cn.hutool.core.text.CharSequenceUtil` | `String removeAllLineBreaks(CharSequence str)` | 去除所有换行符，包括： |
| `cn.hutool.core.text.CharSequenceUtil` | `String removeAllPrefix(CharSequence str,CharSequence prefix)` | 去掉指定所有前缀，如： |
| `cn.hutool.core.text.CharSequenceUtil` | `String removeAllSuffix(CharSequence str,CharSequence suffix)` | 去掉指定所有后缀，如： |
| `cn.hutool.core.text.CharSequenceUtil` | `String removeAny(CharSequence str,CharSequence... strsToRemove)` | 移除字符串中所有给定字符串，当某个字符串出现多次，则全部移除 例：removeAny("aa-bb-cc-dd", "a", "b") =》 --cc-dd |
| `cn.hutool.core.text.CharSequenceUtil` | `String removePreAndLowerFirst(CharSequence str,CharSequence prefix)` | 去掉首部指定长度的字符串并将剩余字符串首字母小写 例如：str=setName, prefix=set =》 return name |
| `cn.hutool.core.text.CharSequenceUtil` | `String removePreAndLowerFirst(CharSequence str,int preLength)` | 去掉首部指定长度的字符串并将剩余字符串首字母小写 例如：str=setName, preLength=3 =》 return name |
| `cn.hutool.core.text.CharSequenceUtil` | `String removePrefix(CharSequence str,CharSequence prefix)` | 去掉指定前缀 |
| `cn.hutool.core.text.CharSequenceUtil` | `String removePrefixIgnoreCase(CharSequence str,CharSequence prefix)` | 忽略大小写去掉指定前缀 |
| `cn.hutool.core.text.CharSequenceUtil` | `String removeSufAndLowerFirst(CharSequence str,CharSequence suffix)` | 去掉指定后缀，并小写首字母 |
| `cn.hutool.core.text.CharSequenceUtil` | `String removeSuffix(CharSequence str,CharSequence suffix)` | 去掉指定后缀 |
| `cn.hutool.core.text.CharSequenceUtil` | `String removeSuffixIgnoreCase(CharSequence str,CharSequence suffix)` | 忽略大小写去掉指定后缀 |
| `cn.hutool.core.text.CharSequenceUtil` | `String repeat(CharSequence str,int count)` | 重复某个字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String repeat(char c,int count)` | 重复某个字符 |
| `cn.hutool.core.text.CharSequenceUtil` | `String repeatAndJoin(CharSequence str,int count,CharSequence delimiter)` | 重复某个字符串并通过分界符连接 |
| `cn.hutool.core.text.CharSequenceUtil` | `String repeatByLength(CharSequence str,int padLen)` | 重复某个字符串到指定长度 |
| `cn.hutool.core.text.CharSequenceUtil` | `String replace(CharSequence str,CharSequence searchStr,CharSequence replacement)` | 替换字符串中的指定字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String replace(CharSequence str,CharSequence searchStr,CharSequence replacement,boolean ignoreCase)` | 替换字符串中的指定字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String replace(CharSequence str,String regex,Func1<java.util.regex.Matcher, String> replaceFun)` | 替换所有正则匹配的文本，并使用自定义函数决定如何替换 |
| `cn.hutool.core.text.CharSequenceUtil` | `String replace(CharSequence str,int fromIndex,CharSequence searchStr,CharSequence replacement,boolean ignoreCase)` | 替换字符串中的指定字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String replace(CharSequence str,int startInclude,int endExclude,CharSequence replacedStr)` | 替换指定字符串的指定区间内字符为指定字符串，字符串只重复一次 此方法使用String#codePoints()完成拆分替换 |
| `cn.hutool.core.text.CharSequenceUtil` | `String replace(CharSequence str,int startInclude,int endExclude,char replacedChar)` | 替换指定字符串的指定区间内字符为固定字符 此方法使用String#codePoints()完成拆分替换 |
| `cn.hutool.core.text.CharSequenceUtil` | `String replace(CharSequence str,java.util.regex.Pattern pattern,Func1<java.util.regex.Matcher, String> replaceFun)` | 替换所有正则匹配的文本，并使用自定义函数决定如何替换 replaceFun可以通过Matcher提取出匹配到的内容的不同部分，然后经过重新处理、组装变成新的内容放回原位。 |
| `cn.hutool.core.text.CharSequenceUtil` | `String replaceByCodePoint(CharSequence str,int startInclude,int endExclude,CharSequence replacedStr)` | 替换指定字符串的指定区间内字符为指定字符串，字符串只重复一次 此方法使用String#codePoints()完成拆分替换 |
| `cn.hutool.core.text.CharSequenceUtil` | `String replaceByCodePoint(CharSequence str,int startInclude,int endExclude,char replacedChar)` | 替换指定字符串的指定区间内字符为固定字符 此方法使用String#codePoints()完成拆分替换 |
| `cn.hutool.core.text.CharSequenceUtil` | `String replaceChars(CharSequence str,String chars,CharSequence replacedStr)` | 替换字符字符数组中所有的字符为replacedStr 提供的chars为所有需要被替换的字符，例如："\r\n"，则"\r"和"\n"都会被替换，哪怕他们单独存在 |
| `cn.hutool.core.text.CharSequenceUtil` | `String replaceChars(CharSequence str,char[] chars,CharSequence replacedStr)` | 替换字符字符数组中所有的字符为replacedStr |
| `cn.hutool.core.text.CharSequenceUtil` | `String replaceFirst(CharSequence str,CharSequence searchStr,CharSequence replacedStr)` | 替换字符串中第一个指定字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String replaceFirst(CharSequence str,CharSequence searchStr,CharSequence replacedStr,boolean ignoreCase)` | 替换字符串中第一个指定字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String replaceIgnoreCase(CharSequence str,CharSequence searchStr,CharSequence replacement)` | 替换字符串中的指定字符串，忽略大小写 |
| `cn.hutool.core.text.CharSequenceUtil` | `String replaceLast(CharSequence str,CharSequence searchStr,CharSequence replacedStr)` | 替换字符串中最后一个指定字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String replaceLast(CharSequence str,CharSequence searchStr,CharSequence replacedStr,boolean ignoreCase)` | 替换字符串中最后一个指定字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String str(CharSequence cs)` | CharSequence 转为字符串，null安全 |
| `cn.hutool.core.text.CharSequenceUtil` | `String strip(CharSequence str,CharSequence prefix,CharSequence suffix)` | 去除两边的指定字符串 两边字符如果存在，则去除，不存在不做处理 |
| `cn.hutool.core.text.CharSequenceUtil` | `String strip(CharSequence str,CharSequence prefix,CharSequence suffix,boolean ignoreCase)` | 去除两边的指定字符串 两边字符如果存在，则去除，不存在不做处理 |
| `cn.hutool.core.text.CharSequenceUtil` | `String strip(CharSequence str,CharSequence prefixOrSuffix)` | 去除两边的指定字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String stripAll(final CharSequence str,final CharSequence prefix,final CharSequence suffix)` | 去除两边 所有 的指定字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String stripAll(final CharSequence str,final CharSequence prefixOrSuffix)` | 去除两边 所有 的指定字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String stripIgnoreCase(final CharSequence str,final CharSequence prefix,final CharSequence suffix)` | 去除两边的指定字符串，忽略大小写 |
| `cn.hutool.core.text.CharSequenceUtil` | `String stripIgnoreCase(final CharSequence str,final CharSequence prefixOrSuffix)` | 去除两边的指定字符串，忽略大小写 |
| `cn.hutool.core.text.CharSequenceUtil` | `String sub(CharSequence str,int fromIndexInclude,int toIndexExclude)` | 改进JDK subString index从0开始计算，最后一个字符为-1 如果from和to位置一样，返回 "" 如果from或to为负数，则按照length从后向前数位置，如果绝对值大于字符串长度，则from归到0，to归到length 如果经过修正的index中from大于to，则互换from和to example: abcdefgh 2 3 =》 c abcdefgh 2 -3 =》 cde |
| `cn.hutool.core.text.CharSequenceUtil` | `String subAfter(CharSequence string,CharSequence separator,boolean isLastSeparator)` | 截取分隔字符串之后的字符串，不包括分隔字符串 如果给定的字符串为空串（null或""），返回原字符串 如果分隔字符串为空串（null或""），则返回空串，如果分隔字符串未找到，返回空串，举例如下： |
| `cn.hutool.core.text.CharSequenceUtil` | `String subAfter(CharSequence string,char separator,boolean isLastSeparator)` | 截取分隔字符串之后的字符串，不包括分隔字符串 如果给定的字符串为空串（null或""），返回原字符串 如果分隔字符串为空串（null或""），则返回空串，如果分隔字符串未找到，返回空串，举例如下： |
| `cn.hutool.core.text.CharSequenceUtil` | `String subBefore(CharSequence string,CharSequence separator,boolean isLastSeparator)` | 截取分隔字符串之前的字符串，不包括分隔字符串 如果给定的字符串为空串（null或""）或者分隔字符串为null，返回原字符串 如果分隔字符串为空串""，则返回空串，如果分隔字符串未找到，返回原字符串，举例如下： |
| `cn.hutool.core.text.CharSequenceUtil` | `String subBefore(CharSequence string,char separator,boolean isLastSeparator)` | 截取分隔字符串之前的字符串，不包括分隔字符串 如果给定的字符串为空串（null或""）或者分隔字符串为null，返回原字符串 如果分隔字符串未找到，返回原字符串，举例如下： |
| `cn.hutool.core.text.CharSequenceUtil` | `String subBetween(CharSequence str,CharSequence before,CharSequence after)` | 截取指定字符串中间部分，不包括标识字符串 栗子： |
| `cn.hutool.core.text.CharSequenceUtil` | `String subBetween(CharSequence str,CharSequence beforeAndAfter)` | 截取指定字符串中间部分，不包括标识字符串 栗子： |
| `cn.hutool.core.text.CharSequenceUtil` | `String subByCodePoint(CharSequence str,int fromIndex,int toIndex)` | 通过CodePoint截取字符串，可以截断Emoji |
| `cn.hutool.core.text.CharSequenceUtil` | `String subPre(CharSequence string,int toIndexExclude)` | 切割指定位置之前部分的字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String subPreGbk(CharSequence str,int len,CharSequence suffix)` | 截取部分字符串，这里一个汉字的长度认为是2 |
| `cn.hutool.core.text.CharSequenceUtil` | `String subPreGbk(CharSequence str,int len,boolean halfUp)` | 截取部分字符串，这里一个汉字的长度认为是2 可以自定义halfUp，如len为10，如果截取后最后一个字符是半个字符，true表示保留，则长度是11，否则长度9 |
| `cn.hutool.core.text.CharSequenceUtil` | `String subSuf(CharSequence string,int fromIndex)` | 切割指定位置之后部分的字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String subSufByLength(CharSequence string,int length)` | 切割指定长度的后部分的字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String subWithLength(String input,int fromIndex,int length)` | 截取字符串,从指定位置开始,截取指定长度的字符串 如果fromIndex为正数，则向后截取指定length长度，如果为负数，则向前截取length长度。 |
| `cn.hutool.core.text.CharSequenceUtil` | `String swapCase(final String str)` | 切换给定字符串中的大小写。大写转小写，小写转大写。 |
| `cn.hutool.core.text.CharSequenceUtil` | `String toCamelCase(CharSequence name)` | 将下划线方式命名的字符串转换为驼峰式。如果转换前的下划线大写方式命名的字符串为空，则返回空字符串。 例如：hello_world=》helloWorld |
| `cn.hutool.core.text.CharSequenceUtil` | `String toCamelCase(CharSequence name,char symbol)` | 将连接符方式命名的字符串转换为驼峰式。如果转换前的下划线大写方式命名的字符串为空，则返回空字符串。 例如：hello_world=》helloWorld; hello-world=》helloWorld |
| `cn.hutool.core.text.CharSequenceUtil` | `String toLoweCase(final CharSequence str)` | 将字符串转为小写 |
| `cn.hutool.core.text.CharSequenceUtil` | `String toLowerCase(final CharSequence str)` | 将字符串转为小写 |
| `cn.hutool.core.text.CharSequenceUtil` | `String toSymbolCase(CharSequence str,char symbol)` | 将驼峰式命名的字符串转换为使用符号连接方式。如果转换前的驼峰式命名的字符串为空，则返回空字符串。 |
| `cn.hutool.core.text.CharSequenceUtil` | `String toUnderlineCase(CharSequence str)` | 将驼峰式命名的字符串转换为下划线方式。如果转换前的驼峰式命名的字符串为空，则返回空字符串。 例如： |
| `cn.hutool.core.text.CharSequenceUtil` | `String toUpperCase(final CharSequence str)` | 将字符串转为大写 |
| `cn.hutool.core.text.CharSequenceUtil` | `String trim(CharSequence str)` | 除去字符串头尾部的空白，如果字符串是null，依然返回null。 注意，和String#trim()不同，此方法使用CharUtil#isBlankChar(char) 来判定空白， 因而可以除去英文字符集之外的其它空白，如中文空格。 |
| `cn.hutool.core.text.CharSequenceUtil` | `String trim(CharSequence str,int mode)` | 除去字符串头尾部的空白符，如果字符串是null，依然返回null。 |
| `cn.hutool.core.text.CharSequenceUtil` | `String trim(CharSequence str,int mode,Predicate<Character> predicate)` | 按照断言，除去字符串头尾部的断言为真的字符，如果字符串是null，依然返回null。 |
| `cn.hutool.core.text.CharSequenceUtil` | `String trimEnd(CharSequence str)` | 除去字符串尾部的空白，如果字符串是null，则返回null。 注意，和String#trim()不同，此方法使用CharUtil#isBlankChar(char) 来判定空白， 因而可以除去英文字符集之外的其它空白，如中文空格。 |
| `cn.hutool.core.text.CharSequenceUtil` | `String trimStart(CharSequence str)` | 除去字符串头部的空白，如果字符串是null，则返回null。 注意，和String#trim()不同，此方法使用CharUtil#isBlankChar(char) 来判定空白， 因而可以除去英文字符集之外的其它空白，如中文空格。 |
| `cn.hutool.core.text.CharSequenceUtil` | `String trimToEmpty(CharSequence str)` | 除去字符串头尾部的空白，如果字符串是null，返回""。 |
| `cn.hutool.core.text.CharSequenceUtil` | `String trimToNull(CharSequence str)` | 除去字符串头尾部的空白，如果字符串是null或者""，返回null。 |
| `cn.hutool.core.text.CharSequenceUtil` | `String unWrap(CharSequence str,String prefix,String suffix)` | 去掉字符包装，如果未被包装则返回原字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String unWrap(CharSequence str,char prefix,char suffix)` | 去掉字符包装，如果未被包装则返回原字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String unWrap(CharSequence str,char prefixAndSuffix)` | 去掉字符包装，如果未被包装则返回原字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String upperFirst(CharSequence str)` | 大写首字母 例如：str = name, return Name |
| `cn.hutool.core.text.CharSequenceUtil` | `String upperFirstAndAddPre(CharSequence str,String preString)` | 原字符串首字母大写并在其首部添加指定字符串 例如：str=name, preString=get =》 return getName |
| `cn.hutool.core.text.CharSequenceUtil` | `String wrap(CharSequence str,CharSequence prefix,CharSequence suffix)` | 包装指定字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String wrap(CharSequence str,CharSequence prefixAndSuffix)` | 包装指定字符串 当前缀和后缀一致时使用此方法 |
| `cn.hutool.core.text.CharSequenceUtil` | `String wrapIfMissing(CharSequence str,CharSequence prefix,CharSequence suffix)` | 包装指定字符串，如果前缀或后缀已经包含对应的字符串，则不再包装 |
| `cn.hutool.core.text.CharSequenceUtil` | `StringBuilder builder(CharSequence... strs)` | 创建StringBuilder对象 |
| `cn.hutool.core.text.CharSequenceUtil` | `StringBuilder builder(Function<CharSequence, CharSequence> strEditor,final CharSequence... strs)` | 创建StringBuilder对象 |
| `cn.hutool.core.text.CharSequenceUtil` | `String[] cut(CharSequence str,int partLength)` | 将字符串切分为N等份 |
| `cn.hutool.core.text.CharSequenceUtil` | `String[] split(CharSequence str,int len)` | 根据给定长度，将给定字符串截取为多个部分 |
| `cn.hutool.core.text.CharSequenceUtil` | `String[] splitToArray(CharSequence str,CharSequence separator)` | 切分字符串，如果分隔符不存在则返回原字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String[] splitToArray(CharSequence str,char separator)` | 切分字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String[] splitToArray(CharSequence text,char separator,int limit)` | 切分字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String[] subBetweenAll(CharSequence str,CharSequence prefix,CharSequence suffix)` | 截取指定字符串多段中间部分，不包括标识字符串 栗子： |
| `cn.hutool.core.text.CharSequenceUtil` | `String[] subBetweenAll(CharSequence str,CharSequence prefixAndSuffix)` | 截取指定字符串多段中间部分，不包括标识字符串 栗子： |
| `cn.hutool.core.text.CharSequenceUtil` | `String[] wrapAll(CharSequence prefix,CharSequence suffix,CharSequence... strs)` | 包装多个字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String[] wrapAllIfMissing(CharSequence prefix,CharSequence suffix,CharSequence... strs)` | 包装多个字符串，如果已经包装，则不再包装 |
| `cn.hutool.core.text.CharSequenceUtil` | `String[] wrapAllWithPair(CharSequence prefixAndSuffix,CharSequence... strs)` | 使用单个字符包装多个字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `String[] wrapAllWithPairIfMissing(CharSequence prefixAndSuffix,CharSequence... strs)` | 使用成对的字符包装多个字符串，如果已经包装，则不再包装 |
| `cn.hutool.core.text.CharSequenceUtil` | `T firstNonBlank(T... strs)` | 返回第一个非blank 元素 |
| `cn.hutool.core.text.CharSequenceUtil` | `T firstNonEmpty(T... strs)` | 返回第一个非empty 元素 |
| `cn.hutool.core.text.CharSequenceUtil` | `T firstNonNull(T... strs)` | 返回第一个非null 元素 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean contains(CharSequence str,CharSequence searchStr)` | 指定字符串是否在字符串中出现过 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean contains(CharSequence str,char searchChar)` | 指定字符是否在字符串中出现过 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean containsAll(CharSequence str,CharSequence... testChars)` | 检查指定字符串中是否含给定的所有字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean containsAny(CharSequence str,CharSequence... testStrs)` | 查找指定字符串是否包含指定字符串列表中的任意一个字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean containsAny(CharSequence str,char... testChars)` | 查找指定字符串是否包含指定字符列表中的任意一个字符 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean containsAnyIgnoreCase(CharSequence str,CharSequence... testStrs)` | 查找指定字符串是否包含指定字符串列表中的任意一个字符串 忽略大小写 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean containsBlank(CharSequence str)` | 给定字符串是否包含空白符（空白符包括空格、制表符、全角空格和不间断空格） 如果给定字符串为null或者""，则返回false |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean containsIgnoreCase(CharSequence str,CharSequence testStr)` | 是否包含特定字符，忽略大小写，如果给定两个参数都为null，返回true |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean containsOnly(CharSequence str,char... testChars)` | 检查指定字符串中是否只包含给定的字符 这里的containsOnly并不是必须全部给定的testChars都需要有，而是一个子集。testChars是个限定集合，检查字符串中的字符是否在这个限定集合中。 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean endWith(CharSequence str,CharSequence suffix)` | 是否以指定字符串结尾 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean endWith(CharSequence str,CharSequence suffix,boolean ignoreCase)` | 是否以指定字符串结尾 如果给定的字符串和开头字符串都为null则返回true，否则任意一个值为null返回false |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean endWith(CharSequence str,CharSequence suffix,boolean ignoreCase,boolean ignoreEquals)` | 是否以指定字符串结尾 如果给定的字符串和开头字符串都为null则返回true，否则任意一个值为null返回false |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean endWith(CharSequence str,char c)` | 字符串是否以给定字符结尾 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean endWithAny(CharSequence str,CharSequence... suffixes)` | 给定字符串是否以任何一个字符串结尾 给定字符串和数组为空都返回false |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean endWithAnyIgnoreCase(CharSequence str,CharSequence... suffixes)` | 给定字符串是否以任何一个字符串结尾（忽略大小写） 给定字符串和数组为空都返回false |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean endWithIgnoreCase(CharSequence str,CharSequence suffix)` | 是否以指定字符串结尾，忽略大小写 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean equals(CharSequence str1,CharSequence str2)` | 比较两个字符串（大小写敏感）。 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean equals(CharSequence str1,CharSequence str2,boolean ignoreCase)` | 比较两个字符串是否相等，规则如下 str1和str2都为null 忽略大小写使用String#equalsIgnoreCase(String)判断相等 不忽略大小写使用String#contentEquals(CharSequence)判断相等 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean equalsAny(CharSequence str1,CharSequence... strs)` | 给定字符串是否与提供的中任一字符串相同，相同则返回true，没有相同的返回false 如果参与比对的字符串列表为空，返回false |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean equalsAny(CharSequence str1,boolean ignoreCase,CharSequence... strs)` | 给定字符串是否与提供的中任一字符串相同，相同则返回true，没有相同的返回false 如果参与比对的字符串列表为空，返回false |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean equalsAnyIgnoreCase(CharSequence str1,CharSequence... strs)` | 给定字符串是否与提供的中任一字符串相同（忽略大小写），相同则返回true，没有相同的返回false 如果参与比对的字符串列表为空，返回false |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean equalsCharAt(CharSequence str,int position,char c)` | 字符串指定位置的字符是否与给定字符相同 如果字符串为null，返回false 如果给定的位置大于字符串长度，返回false 如果给定的位置小于0，返回false |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean equalsIgnoreCase(CharSequence str1,CharSequence str2)` | 比较两个字符串（大小写不敏感）。 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean hasBlank(CharSequence... strs)` | 指定字符串数组中，是否包含空字符串。 如果指定的字符串数组的长度为 0，或者其中的任意一个元素是空字符串，则返回 true。 例： CharSequenceUtil.hasBlank() // true CharSequenceUtil.hasBlank("", null, " ") // true CharSequenceUtil.hasBlank("123", " ") // true CharSequenceUtil.hasBlank("123", "abc") // false 注意：该方法与 #isAllBlank(CharSequence...) 的区别在于： hasBlank(C… |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean hasEmpty(CharSequence... strs)` | 是否包含空字符串。 如果指定的字符串数组的长度为 0，或者其中的任意一个元素是空字符串，则返回 true。 例： CharSequenceUtil.hasEmpty() // true CharSequenceUtil.hasEmpty("", null) // true CharSequenceUtil.hasEmpty("123", "") // true CharSequenceUtil.hasEmpty("123", "abc") // false CharSequenceUtil.hasEmpty(" ", "\t", "\n") // false 注意：该方法与 #isAllEmp… |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean hasLetter(CharSequence str)` | 指定字符串数组中，是否包含空字符串。 如果传入参数对象不是为空,则返回false。如果字符串包含字母,不区分大小写,则返回true |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean isAllBlank(CharSequence... strs)` | 指定字符串数组中的元素，是否全部为空字符串。 如果指定的字符串数组的长度为 0，或者所有元素都是空字符串，则返回 true。 例： CharSequenceUtil.isAllBlank() // true CharSequenceUtil.isAllBlank("", null, " ") // true CharSequenceUtil.isAllBlank("123", " ") // false CharSequenceUtil.isAllBlank("123", "abc") // false 注意：该方法与 #hasBlank(CharSequence...) 的区别在于： #ha… |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean isAllCharMatch(CharSequence value,Matcher<Character> matcher)` | 字符串的每一个字符是否都与定义的匹配器匹配 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean isAllEmpty(CharSequence... strs)` | 指定字符串数组中的元素，是否全部为空字符串。 如果指定的字符串数组的长度为 0，或者所有元素都是空字符串，则返回 true。 例： CharSequenceUtil.isAllEmpty() // true CharSequenceUtil.isAllEmpty("", null) // true CharSequenceUtil.isAllEmpty("123", "") // false CharSequenceUtil.isAllEmpty("123", "abc") // false CharSequenceUtil.isAllEmpty(" ", "\t", "\n") // fal… |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean isAllNotBlank(CharSequence... args)` | 是否全都不为null或空对象或空白符的对象，通过#hasBlank(CharSequence...) 判断元素 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean isAllNotEmpty(CharSequence... args)` | 指定字符串数组中的元素，是否都不为空字符串。 如果指定的字符串数组的长度不为 0，或者所有元素都不是空字符串，则返回 true。 例： CharSequenceUtil.isAllNotEmpty() // false CharSequenceUtil.isAllNotEmpty("", null) // false CharSequenceUtil.isAllNotEmpty("123", "") // false CharSequenceUtil.isAllNotEmpty("123", "abc") // true CharSequenceUtil.isAllNotEmpty(" ", … |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean isBlank(CharSequence str)` | 字符串是否为空白，空白的定义如下： null 空字符串："" 空格、全角空格、制表符、换行符，等不可见字符 例： CharSequenceUtil.isBlank(null) // true CharSequenceUtil.isBlank("") // true CharSequenceUtil.isBlank(" \t\n") // true CharSequenceUtil.isBlank("abc") // false 注意：该方法与 #isEmpty(CharSequence) 的区别是： 该方法会校验空白字符，且性能相对于 #isEmpty(CharSequence) 略慢。 建议… |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean isBlankOrUndefined(CharSequence str)` | 检查字符串是否为null、空白串、“null”、“undefined” |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean isCharEquals(CharSequence str)` | 检查给定字符串的所有字符是否都一样 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean isEmpty(CharSequence str)` | 字符串是否为空，空的定义如下： null 空字符串："" 例： CharSequenceUtil.isEmpty(null) // true CharSequenceUtil.isEmpty("") // true CharSequenceUtil.isEmpty(" \t\n") // false CharSequenceUtil.isEmpty("abc") // false 注意：该方法与 #isBlank(CharSequence) 的区别是：该方法不校验空白字符。 建议： 该方法建议用于工具类或任何可以预期的方法参数的校验中。 需要同时校验多个字符串时，建议采用 #hasEmpty(… |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean isEmptyOrUndefined(CharSequence str)` | 检查字符串是否为null、“”、“null”、“undefined” |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean isLowerCase(CharSequence str)` | 给定字符串中的字母是否全部为小写，判断依据如下： |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean isNotBlank(CharSequence str)` | 字符串是否为非空白，非空白的定义如下： 不为 null 不为空字符串："" 不为空格、全角空格、制表符、换行符，等不可见字符 例： CharSequenceUtil.isNotBlank(null) // false CharSequenceUtil.isNotBlank("") // false CharSequenceUtil.isNotBlank(" \t\n") // false CharSequenceUtil.isNotBlank("abc") // true 注意：该方法与 #isNotEmpty(CharSequence) 的区别是： 该方法会校验空白字符，且性能相对于 #is… |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean isNotEmpty(CharSequence str)` | 字符串是否为非空白，非空白的定义如下： 不为 null 不为空字符串："" 例： CharSequenceUtil.isNotEmpty(null) // false CharSequenceUtil.isNotEmpty("") // false CharSequenceUtil.isNotEmpty(" \t\n") // true CharSequenceUtil.isNotEmpty("abc") // true 注意：该方法与 #isNotBlank(CharSequence) 的区别是：该方法不校验空白字符。 建议：该方法建议用于工具类或任何可以预期的方法参数的校验中。 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean isNullOrUndefined(CharSequence str)` | 检查字符串是否为null、“null”、“undefined” |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean isNumeric(CharSequence str)` | 检查字符串是否都为数字组成 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean isSubEquals(CharSequence str1,int start1,CharSequence str2,boolean ignoreCase)` | 截取第一个字串的部分字符，与第二个字符串比较（长度一致），判断截取的子串是否相同 任意一个字符串为null返回false |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean isSubEquals(CharSequence str1,int start1,CharSequence str2,int start2,int length,boolean ignoreCase)` | 截取两个字符串的不同部分（长度一致），判断截取的子串是否相同 任意一个字符串为null返回false |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean isSurround(CharSequence str,CharSequence prefix,CharSequence suffix)` | 给定字符串是否被字符包围 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean isSurround(CharSequence str,char prefix,char suffix)` | 给定字符串是否被字符包围 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean isUpperCase(CharSequence str)` | 给定字符串中的字母是否全部为大写，判断依据如下： |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean isWrap(CharSequence str,String prefix,String suffix)` | 指定字符串是否被包装 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean isWrap(CharSequence str,String wrapper)` | 指定字符串是否被同一字符包装（前后都有这些字符串） |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean isWrap(CharSequence str,char prefixChar,char suffixChar)` | 指定字符串是否被包装 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean isWrap(CharSequence str,char wrapper)` | 指定字符串是否被同一字符包装（前后都有这些字符串） |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean startWith(CharSequence str,CharSequence prefix)` | 是否以指定字符串开头 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean startWith(CharSequence str,CharSequence prefix,boolean ignoreCase)` | 是否以指定字符串开头 如果给定的字符串和开头字符串都为null则返回true，否则任意一个值为null返回false |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean startWith(CharSequence str,CharSequence prefix,boolean ignoreCase,boolean ignoreEquals)` | 是否以指定字符串开头 如果给定的字符串和开头字符串都为null则返回true，否则任意一个值为null返回false |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean startWith(CharSequence str,char c)` | 字符串是否以给定字符开始 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean startWithAny(CharSequence str,CharSequence... prefixes)` | 给定字符串是否以任何一个字符串开始 给定字符串和数组为空都返回false |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean startWithAnyIgnoreCase(final CharSequence str,final CharSequence... prefixes)` | 给定字符串是否以任何一个字符串开始（忽略大小写） 给定字符串和数组为空都返回false |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean startWithIgnoreCase(CharSequence str,CharSequence prefix)` | 是否以指定字符串开头，忽略大小写 |
| `cn.hutool.core.text.CharSequenceUtil` | `boolean startWithIgnoreEquals(CharSequence str,CharSequence prefix)` | 是否以指定字符串开头，忽略相等字符串的情况 |
| `cn.hutool.core.text.CharSequenceUtil` | `byte[] bytes(CharSequence str)` | 编码字符串 使用系统默认编码 |
| `cn.hutool.core.text.CharSequenceUtil` | `byte[] bytes(CharSequence str,Charset charset)` | 编码字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `byte[] bytes(CharSequence str,String charset)` | 编码字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `byte[] utf8Bytes(CharSequence str)` | 编码字符串，编码为UTF-8 |
| `cn.hutool.core.text.CharSequenceUtil` | `int byteLength(CharSequence cs,Charset charset)` | 给定字符串转为bytes后的byte数（byte长度） |
| `cn.hutool.core.text.CharSequenceUtil` | `int compare(final CharSequence str1,final CharSequence str2,final boolean nullIsLess)` | 比较两个字符串，用于排序 |
| `cn.hutool.core.text.CharSequenceUtil` | `int compareIgnoreCase(CharSequence str1,CharSequence str2,boolean nullIsLess)` | 比较两个字符串，用于排序，大小写不敏感 |
| `cn.hutool.core.text.CharSequenceUtil` | `int compareVersion(CharSequence version1,CharSequence version2)` | 比较两个版本 null版本排在最小：即： |
| `cn.hutool.core.text.CharSequenceUtil` | `int count(CharSequence content,CharSequence strForSearch)` | 统计指定内容中包含指定字符串的数量 参数为 null 或者 "" 返回 0. |
| `cn.hutool.core.text.CharSequenceUtil` | `int count(CharSequence content,char charForSearch)` | 统计指定内容中包含指定字符的数量 |
| `cn.hutool.core.text.CharSequenceUtil` | `int indexOf(CharSequence str,char searchChar)` | 指定范围内查找指定字符 |
| `cn.hutool.core.text.CharSequenceUtil` | `int indexOf(CharSequence str,char searchChar,int start)` | 指定范围内查找指定字符 |
| `cn.hutool.core.text.CharSequenceUtil` | `int indexOf(CharSequence text,CharSequence searchStr,int from,boolean ignoreCase)` | 指定范围内查找字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `int indexOf(CharSequence text,char searchChar,int start,int end)` | 指定范围内查找指定字符 |
| `cn.hutool.core.text.CharSequenceUtil` | `int indexOfIgnoreCase(final CharSequence str,final CharSequence searchStr)` | 指定范围内查找字符串，忽略大小写 |
| `cn.hutool.core.text.CharSequenceUtil` | `int indexOfIgnoreCase(final CharSequence str,final CharSequence searchStr,int fromIndex)` | 指定范围内查找字符串 |
| `cn.hutool.core.text.CharSequenceUtil` | `int lastIndexOf(CharSequence text,CharSequence searchStr,int from,boolean ignoreCase)` | 指定范围内查找字符串 fromIndex 为搜索起始位置，从后往前计数 |
| `cn.hutool.core.text.CharSequenceUtil` | `int lastIndexOfIgnoreCase(CharSequence str,CharSequence searchStr)` | 指定范围内查找字符串，忽略大小写 |
| `cn.hutool.core.text.CharSequenceUtil` | `int lastIndexOfIgnoreCase(CharSequence str,CharSequence searchStr,int fromIndex)` | 指定范围内查找字符串，忽略大小写 fromIndex 为搜索起始位置，从后往前计数 |
| `cn.hutool.core.text.CharSequenceUtil` | `int length(CharSequence cs)` | 获取字符串的长度，如果为null返回0 |
| `cn.hutool.core.text.CharSequenceUtil` | `int ordinalIndexOf(CharSequence str,CharSequence searchStr,int ordinal)` | 返回字符串 searchStr 在字符串 str 中第 ordinal 次出现的位置。 如果 str=null 或 searchStr=null 或 ordinal≤0 则返回-1 此方法来自：Apache-Commons-Lang 例子（*代表任意字符）： |
| `cn.hutool.core.text.CharSequenceUtil` | `int totalLength(CharSequence... strs)` | 给定字符串数组的总长度 null字符长度定义为0 |
| `cn.hutool.core.text.CharSequenceUtil` | `int[] splitToInt(CharSequence str,CharSequence separator)` | 切分字符串为int数组 |
| `cn.hutool.core.text.CharSequenceUtil` | `int[] splitToInt(CharSequence str,char separator)` | 切分字符串为int数组 |
| `cn.hutool.core.text.CharSequenceUtil` | `long[] splitToLong(CharSequence str,CharSequence separator)` | 切分字符串为long数组 |
| `cn.hutool.core.text.CharSequenceUtil` | `long[] splitToLong(CharSequence str,char separator)` | 切分字符串为long数组 |
| `cn.hutool.core.text.NamingCase` | `String toCamelCase(CharSequence name)` | 将下划线方式命名的字符串转换为驼峰式。如果转换前的下划线大写方式命名的字符串为空，则返回空字符串。 规则为： 单字之间不以空格或任何连接符断开 第一个单字首字母采用小写字母 后续单字的首字母亦用大写字母 例如：hello_world=》helloWorld |
| `cn.hutool.core.text.NamingCase` | `String toCamelCase(CharSequence name,char symbol)` | 将连接符方式命名的字符串转换为驼峰式。如果转换前的下划线大写方式命名的字符串为空，则返回空字符串。 |
| `cn.hutool.core.text.NamingCase` | `String toCamelCase(CharSequence name,char symbol,boolean otherCharToLower)` | 将连接符方式命名的字符串转换为驼峰式。如果转换前的下划线大写方式命名的字符串为空，则返回空字符串。 |
| `cn.hutool.core.text.NamingCase` | `String toKebabCase(CharSequence str)` | 将驼峰式命名的字符串转换为短横连接方式。 如果转换前的驼峰式命名的字符串为空，则返回空字符串。 规则为： 单字之间横线线隔开 每个单字的首字母亦用小写字母 例如： |
| `cn.hutool.core.text.NamingCase` | `String toPascalCase(CharSequence name)` | 将下划线方式命名的字符串转换为帕斯卡式。 规则为： 单字之间不以空格或任何连接符断开 第一个单字首字母采用大写字母 后续单字的首字母亦用大写字母 如果转换前的下划线大写方式命名的字符串为空，则返回空字符串。 例如：hello_world=》HelloWorld |
| `cn.hutool.core.text.NamingCase` | `String toSymbolCase(CharSequence str,char symbol)` | 将驼峰式命名的字符串转换为使用符号连接方式。如果转换前的驼峰式命名的字符串为空，则返回空字符串。 |
| `cn.hutool.core.text.NamingCase` | `String toUnderlineCase(CharSequence str)` | 将驼峰式命名的字符串转换为下划线方式，又称SnakeCase、underScoreCase。 如果转换前的驼峰式命名的字符串为空，则返回空字符串。 规则为： 单字之间以下划线隔开 每个单字的首字母亦用小写字母 例如： |
| `cn.hutool.core.text.PasswdStrength` | `PASSWD_LEVEL getLevel(String passwd)` | 获取密码强度等级, 包括 easy, medium, strong, very strong, extremely strong |
| `cn.hutool.core.text.PasswdStrength` | `int check(String passwd)` | 检查密码的健壮性 |
| `cn.hutool.core.text.Simhash` | `boolean equals(Collection<? extends CharSequence> segList)` | 判断文本是否与已存储的数据重复 |
| `cn.hutool.core.text.Simhash` | `long hash(Collection<? extends CharSequence> segList)` | 指定文本计算simhash值 |
| `cn.hutool.core.text.Simhash` | `void store(Long simhash)` | 按照(frac, 《simhash, content》)索引进行存储 |
| `cn.hutool.core.text.StrBuilder` | `CharSequence subSequence(int start,int end)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.StrBuilder` | `StrBuilder append(CharSequence csq)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.StrBuilder` | `StrBuilder append(CharSequence csq,int start,int end)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.StrBuilder` | `StrBuilder append(Object obj)` | 追加对象，对象会被转换为字符串 |
| `cn.hutool.core.text.StrBuilder` | `StrBuilder append(char c)` | 追加一个字符 |
| `cn.hutool.core.text.StrBuilder` | `StrBuilder append(char[] src)` | 追加一个字符数组 |
| `cn.hutool.core.text.StrBuilder` | `StrBuilder append(char[] src,int srcPos,int length)` | 追加一个字符数组 |
| `cn.hutool.core.text.StrBuilder` | `StrBuilder clear()` | 删除全部字符，位置归零 |
| `cn.hutool.core.text.StrBuilder` | `StrBuilder create()` | 创建字符串构建器 |
| `cn.hutool.core.text.StrBuilder` | `StrBuilder create(CharSequence... strs)` | 创建字符串构建器 |
| `cn.hutool.core.text.StrBuilder` | `StrBuilder create(int initialCapacity)` | 创建字符串构建器 |
| `cn.hutool.core.text.StrBuilder` | `StrBuilder del(int start,int end)` | 删除指定长度的字符，规则如下： |
| `cn.hutool.core.text.StrBuilder` | `StrBuilder delTo(int newPosition)` | 删除到指定位置 如果新位置小于等于0，则删除全部 |
| `cn.hutool.core.text.StrBuilder` | `StrBuilder getChars(int srcBegin,int srcEnd,char[] dst,int dstBegin)` | 将指定段的字符列表写出到目标字符数组中 |
| `cn.hutool.core.text.StrBuilder` | `StrBuilder insert(int index,CharSequence csq)` | 指定位置插入字符串的某个部分 如果插入位置为当前位置，则定义为追加 如果插入位置大于当前位置，则中间部分补充空格 |
| `cn.hutool.core.text.StrBuilder` | `StrBuilder insert(int index,CharSequence csq,int start,int end)` | 指定位置插入字符串的某个部分 如果插入位置为当前位置，则定义为追加 如果插入位置大于当前位置，则中间部分补充空格 |
| `cn.hutool.core.text.StrBuilder` | `StrBuilder insert(int index,Object obj)` | 追加对象，对象会被转换为字符串 |
| `cn.hutool.core.text.StrBuilder` | `StrBuilder insert(int index,char c)` | 插入指定字符 |
| `cn.hutool.core.text.StrBuilder` | `StrBuilder insert(int index,char[] src)` | 指定位置插入数据 如果插入位置为当前位置，则定义为追加 如果插入位置大于当前位置，则中间部分补充空格 |
| `cn.hutool.core.text.StrBuilder` | `StrBuilder insert(int index,char[] src,int srcPos,int length)` | 指定位置插入数据 如果插入位置为当前位置，则定义为追加 如果插入位置大于当前位置，则中间部分补充空格 |
| `cn.hutool.core.text.StrBuilder` | `StrBuilder reset()` | 删除全部字符，位置归零 |
| `cn.hutool.core.text.StrBuilder` | `String subString(int start)` | 返回自定段的字符串 |
| `cn.hutool.core.text.StrBuilder` | `String subString(int start,int end)` | 返回自定段的字符串 |
| `cn.hutool.core.text.StrBuilder` | `String toString()` | 生成字符串 |
| `cn.hutool.core.text.StrBuilder` | `String toString(boolean isReset)` | 生成字符串 |
| `cn.hutool.core.text.StrBuilder` | `String toStringAndReset()` | 重置并返回生成的字符串 |
| `cn.hutool.core.text.StrBuilder` | `boolean hasContent()` | 是否有内容 |
| `cn.hutool.core.text.StrBuilder` | `boolean isEmpty()` | 是否为空 |
| `cn.hutool.core.text.StrBuilder` | `char charAt(int index)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.StrBuilder` | `int length()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.StrFormatter` | `String format(CharSequence template,Map<?, ?> map,boolean ignoreNull)` | 格式化文本，使用 {varName} 占位 map = {a: "aValue", b: "bValue"} format("{a} and {b}", map) ---=》 aValue and bValue |
| `cn.hutool.core.text.StrFormatter` | `String format(String strPattern,Object... argArray)` | 格式化字符串 此方法只是简单将占位符 {} 按照顺序替换为参数 如果想输出 {} 使用 \\转义 { 即可，如果想输出 {} 之前的 \ 使用双转义符 \\\\ 即可 例： 通常使用：format("this is {} for {}", "a", "b") =》 this is a for b 转义{}： format("this is \\{} for {}", "a", "b") =》 this is \{} for a 转义\： format("this is \\\\{} for {}", "a", "b") =》 this is \a for b |
| `cn.hutool.core.text.StrFormatter` | `String formatWith(String strPattern,String placeHolder,Object... argArray)` | 格式化字符串 此方法只是简单将指定占位符 按照顺序替换为参数 如果想输出占位符使用 \\转义即可，如果想输出占位符之前的 \ 使用双转义符 \\\\ 即可 例： 通常使用：format("this is {} for {}", "{}", "a", "b") =》 this is a for b 转义{}： format("this is \\{} for {}", "{}", "a", "b") =》 this is {} for a 转义\： format("this is \\\\{} for {}", "{}", "a", "b") =》 this is \a for b |
| `cn.hutool.core.text.StrJoiner` | `StrJoiner append(CharSequence csq)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.StrJoiner` | `StrJoiner append(CharSequence csq,int startInclude,int endExclude)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.StrJoiner` | `StrJoiner append(Iterable<E> iterable,Function<? super E, ? extends CharSequence> toStrFunc)` | 追加Iterator中的元素到拼接器中 |
| `cn.hutool.core.text.StrJoiner` | `StrJoiner append(Iterator<E> iterator,Function<? super E, ? extends CharSequence> toStrFunc)` | 追加Iterator中的元素到拼接器中 |
| `cn.hutool.core.text.StrJoiner` | `StrJoiner append(Iterator<T> iterator)` | 追加Iterator中的元素到拼接器中 |
| `cn.hutool.core.text.StrJoiner` | `StrJoiner append(Object obj)` | 追加对象到拼接器中 |
| `cn.hutool.core.text.StrJoiner` | `StrJoiner append(T[] array)` | 追加数组中的元素到拼接器中 |
| `cn.hutool.core.text.StrJoiner` | `StrJoiner append(T[] array,Function<T, ? extends CharSequence> toStrFunc)` | 追加数组中的元素到拼接器中 |
| `cn.hutool.core.text.StrJoiner` | `StrJoiner append(char c)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.StrJoiner` | `StrJoiner merge(StrJoiner strJoiner)` | 合并一个StrJoiner 到当前的StrJoiner 合并规则为，在尾部直接追加，当存在#prefix时，如果#wrapElement为false，则去除之。 |
| `cn.hutool.core.text.StrJoiner` | `StrJoiner of(CharSequence delimiter)` | 使用指定分隔符创建StrJoiner |
| `cn.hutool.core.text.StrJoiner` | `StrJoiner of(CharSequence delimiter,CharSequence prefix,CharSequence suffix)` | 使用指定分隔符创建StrJoiner |
| `cn.hutool.core.text.StrJoiner` | `StrJoiner of(StrJoiner joiner)` | 根据已有StrJoiner配置新建一个新的StrJoiner |
| `cn.hutool.core.text.StrJoiner` | `StrJoiner setDelimiter(CharSequence delimiter)` | 设置分隔符 |
| `cn.hutool.core.text.StrJoiner` | `StrJoiner setEmptyResult(String emptyResult)` | 设置当没有任何元素加入时，默认返回的字符串，默认"" |
| `cn.hutool.core.text.StrJoiner` | `StrJoiner setNullMode(NullMode nullMode)` | 设置null元素处理逻辑 |
| `cn.hutool.core.text.StrJoiner` | `StrJoiner setPrefix(CharSequence prefix)` | 设置前缀 |
| `cn.hutool.core.text.StrJoiner` | `StrJoiner setSuffix(CharSequence suffix)` | 设置后缀 |
| `cn.hutool.core.text.StrJoiner` | `StrJoiner setWrapElement(boolean wrapElement)` | 设置前缀和后缀是否包装每个元素 |
| `cn.hutool.core.text.StrJoiner` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.StrJoiner` | `int length()` | 长度 长度计算方式为prefix + suffix + content 此方法结果与toString().length()一致。 |
| `cn.hutool.core.text.StrMatcher` | `Map<String, String> match(String text)` | 匹配并提取匹配到的内容 |
| `cn.hutool.core.text.StrSplitter` | `List<R> split(CharSequence str,char separator,int limit,boolean ignoreEmpty,Function<String, R> mapping)` | 切分字符串，大小写敏感 |
| `cn.hutool.core.text.StrSplitter` | `List<R> split(CharSequence text,char separator,int limit,boolean ignoreEmpty,boolean ignoreCase,Function<String, R> mapping)` | 切分字符串 如果提供的字符串为null，则返回一个空的ArrayList 如果提供的字符串为""，则当ignoreEmpty时返回空的ArrayList，否则返回只有一个""元素的ArrayList |
| `cn.hutool.core.text.StrSplitter` | `List<String> split(CharSequence str,String separator,boolean isTrim,boolean ignoreEmpty)` | 切分字符串，不忽略大小写 |
| `cn.hutool.core.text.StrSplitter` | `List<String> split(CharSequence str,String separator,int limit,boolean isTrim,boolean ignoreEmpty)` | 切分字符串，不忽略大小写 |
| `cn.hutool.core.text.StrSplitter` | `List<String> split(CharSequence str,char separator,boolean isTrim,boolean ignoreEmpty)` | 切分字符串 |
| `cn.hutool.core.text.StrSplitter` | `List<String> split(CharSequence str,char separator,int limit,boolean isTrim,boolean ignoreEmpty)` | 切分字符串，大小写敏感 |
| `cn.hutool.core.text.StrSplitter` | `List<String> split(CharSequence text,String separator,int limit,boolean isTrim,boolean ignoreEmpty,boolean ignoreCase)` | 切分字符串 如果为空字符串或者null 则返回空集合 |
| `cn.hutool.core.text.StrSplitter` | `List<String> split(CharSequence text,char separator,int limit,boolean isTrim,boolean ignoreEmpty,boolean ignoreCase)` | 切分字符串 |
| `cn.hutool.core.text.StrSplitter` | `List<String> split(CharSequence text,int limit)` | 使用空白符切分字符串 切分后的字符串两边不包含空白符，空串或空白符串并不做为元素之一 如果为空字符串或者null 则返回空集合 |
| `cn.hutool.core.text.StrSplitter` | `List<String> split(String text,Pattern separatorPattern,int limit,boolean isTrim,boolean ignoreEmpty)` | 通过正则切分字符串 如果为空字符串或者null 则返回空集合 |
| `cn.hutool.core.text.StrSplitter` | `List<String> splitByRegex(String text,String separatorRegex,int limit,boolean isTrim,boolean ignoreEmpty)` | 通过正则切分字符串 |
| `cn.hutool.core.text.StrSplitter` | `List<String> splitIgnoreCase(CharSequence str,String separator,int limit,boolean isTrim,boolean ignoreEmpty)` | 切分字符串，忽略大小写 |
| `cn.hutool.core.text.StrSplitter` | `List<String> splitIgnoreCase(CharSequence text,char separator,int limit,boolean isTrim,boolean ignoreEmpty)` | 切分字符串，忽略大小写 |
| `cn.hutool.core.text.StrSplitter` | `List<String> splitPath(CharSequence str)` | 切分字符串路径，仅支持Unix分界符：/ |
| `cn.hutool.core.text.StrSplitter` | `List<String> splitPath(CharSequence str,int limit)` | 切分字符串路径，仅支持Unix分界符：/ |
| `cn.hutool.core.text.StrSplitter` | `List<String> splitTrim(CharSequence str,String separator,boolean ignoreEmpty)` | 切分字符串，去除每个元素两边空格，忽略大小写 |
| `cn.hutool.core.text.StrSplitter` | `List<String> splitTrim(CharSequence str,String separator,int limit,boolean ignoreEmpty)` | 切分字符串，去除每个元素两边空格，忽略大小写 |
| `cn.hutool.core.text.StrSplitter` | `List<String> splitTrim(CharSequence str,char separator,boolean ignoreEmpty)` | 切分字符串 |
| `cn.hutool.core.text.StrSplitter` | `List<String> splitTrim(CharSequence str,char separator,int limit,boolean ignoreEmpty)` | 切分字符串，大小写敏感，去除每个元素两边空白符 |
| `cn.hutool.core.text.StrSplitter` | `List<String> splitTrimIgnoreCase(CharSequence str,String separator,int limit,boolean ignoreEmpty)` | 切分字符串，去除每个元素两边空格，忽略大小写 |
| `cn.hutool.core.text.StrSplitter` | `String[] splitByLength(CharSequence text,int len)` | 根据给定长度，将给定字符串截取为多个部分 |
| `cn.hutool.core.text.StrSplitter` | `String[] splitPathToArray(CharSequence str)` | 切分字符串路径，仅支持Unix分界符：/ |
| `cn.hutool.core.text.StrSplitter` | `String[] splitPathToArray(CharSequence str,int limit)` | 切分字符串路径，仅支持Unix分界符：/ |
| `cn.hutool.core.text.StrSplitter` | `String[] splitToArray(CharSequence str,String separator,int limit,boolean isTrim,boolean ignoreEmpty)` | 切分字符串为字符串数组 |
| `cn.hutool.core.text.StrSplitter` | `String[] splitToArray(CharSequence str,char separator,int limit,boolean isTrim,boolean ignoreEmpty)` | 切分字符串为字符串数组 |
| `cn.hutool.core.text.StrSplitter` | `String[] splitToArray(String str,Pattern separatorPattern,int limit,boolean isTrim,boolean ignoreEmpty)` | 通过正则切分字符串为字符串数组 |
| `cn.hutool.core.text.StrSplitter` | `String[] splitToArray(String str,int limit)` | 切分字符串为字符串数组 |
| `cn.hutool.core.text.TextSimilarity` | `String longestCommonSubstring(String strA,String strB)` | 最长公共子串，采用动态规划算法。 其不要求所求得的字符在所给的字符串中是连续的。 算法解析见：https://leetcode-cn.com/problems/longest-common-subsequence/solution/zui-chang-gong-gong-zi-xu-lie-by-leetcod-y7u0/ |
| `cn.hutool.core.text.TextSimilarity` | `String similar(String strA,String strB,int scale)` | 利用莱文斯坦距离(Levenshtein distance)算法计算相似度百分比 |
| `cn.hutool.core.text.TextSimilarity` | `double similar(String strA,String strB)` | 利用莱文斯坦距离(Levenshtein distance)算法计算相似度，两个都是空串相似度为1，被认为是相同的串 比较方法为： 只比较两个字符串字母、数字、汉字部分，其他符号去除 计算出两个字符串最大子串，除以最长的字符串，结果即为相似度 |
| `cn.hutool.core.text.UnicodeUtil` | `String toString(String unicode)` | Unicode字符串转为普通字符串 Unicode字符串的表现方式为：\\uXXXX |
| `cn.hutool.core.text.UnicodeUtil` | `String toUnicode(String str)` | 字符串编码为Unicode形式 |
| `cn.hutool.core.text.UnicodeUtil` | `String toUnicode(String str,boolean isSkipAscii)` | 字符串编码为Unicode形式 |
| `cn.hutool.core.text.UnicodeUtil` | `String toUnicode(char c)` | 字符编码为Unicode形式 |
| `cn.hutool.core.text.UnicodeUtil` | `String toUnicode(int c)` | 字符编码为Unicode形式 |
