# com.google.common.escape

版本 33.4.8-jre。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.google.common.escape.ArrayBasedCharEscaper` | `String escape(String s)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.escape.ArrayBasedEscaperMap` | `ArrayBasedEscaperMap create(Map<Character, String> replacements)` | 【原文待译】Returns a new ArrayBasedEscaperMap for creating ArrayBasedCharEscaper or ArrayBasedUnicodeEscaper instances. |
| `com.google.common.escape.ArrayBasedUnicodeEscaper` | `String escape(String s)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.escape.CharEscaper` | `String escape(String string)` | 【原文待译】Returns the escaped form of a given literal string. |
| `com.google.common.escape.CharEscaperBuilder` | `CharEscaperBuilder addEscape(char c,String r)` | 【原文待译】Add a new mapping from an index to an object to the escaping. |
| `com.google.common.escape.CharEscaperBuilder` | `CharEscaperBuilder addEscapes(char[] cs,String r)` | 【原文待译】Add multiple mappings at once for a particular index. |
| `com.google.common.escape.CharEscaperBuilder` | `Escaper toEscaper()` | 【原文待译】Convert this builder into a char escaper which is just a decorator around the underlying array of replacement char[]s. |
| `com.google.common.escape.CharEscaperBuilder` | `char[] @Nullable [] toArray()` | 【原文待译】Convert this builder into an array of char[]s where the maximum index is the value of the highest character that has been seen. The array will be sparse in the sense that any unseen index will default to null. |
| `com.google.common.escape.Escaper` | `Function<String, String> asFunction()` | 【原文待译】Returns a Function that invokes #escape(String) on this escaper. |
| `com.google.common.escape.Escaper` | `String escape(String string)` | 【原文待译】Returns the escaped form of a given literal string. Note that this method may treat input characters differently depending on the specific escaper implementation. UnicodeEscaper handles UTF-16 correctly, including surrogate character pairs. If the input is badly formed the escaper should throw Illeg… |
| `com.google.common.escape.Escapers` | `Builder builder()` | 【原文待译】Returns a builder for creating simple, fast escapers. A builder instance can be reused and each escaper that is created will be a snapshot of the current builder state. Builders are not thread safe. The initial state of the builder is such that: There are no replacement mappings safeMin == Character… |
| `com.google.common.escape.Escapers` | `Escaper nullEscaper()` | 【原文待译】Returns an Escaper that does no escaping, passing all character data through unchanged. |
| `com.google.common.escape.Escapers` | `String computeReplacement(CharEscaper escaper,char c)` | 【原文待译】Returns a string that would replace the given character in the specified escaper, or null if no replacement should be made. This method is intended for use in tests through the EscaperAsserts class; production users of CharEscaper should limit themselves to its public interface. |
| `com.google.common.escape.Escapers` | `String computeReplacement(UnicodeEscaper escaper,int cp)` | 【原文待译】Returns a string that would replace the given character in the specified escaper, or null if no replacement should be made. This method is intended for use in tests through the EscaperAsserts class; production users of UnicodeEscaper should limit themselves to its public interface. |
| `com.google.common.escape.Escapers$Builder` | `Builder addEscape(char c,String replacement)` | 【原文待译】Adds a replacement string for the given input character. The specified character will be replaced by the given string whenever it occurs in the input, irrespective of whether it lies inside or outside the 'safe' range. |
| `com.google.common.escape.Escapers$Builder` | `Builder setSafeRange(char safeMin,char safeMax)` | 【原文待译】Sets the safe range of characters for the escaper. Characters in this range that have no explicit replacement are considered 'safe' and remain unescaped in the output. If safeMax < safeMin then the safe range is empty. |
| `com.google.common.escape.Escapers$Builder` | `Builder setUnsafeReplacement(@Nullable
String unsafeReplacement)` | 【原文待译】Sets the replacement string for any characters outside the 'safe' range that have no explicit replacement. If unsafeReplacement is null then no replacement will occur, if it is "" then the unsafe characters are removed from the output. |
| `com.google.common.escape.Escapers$Builder` | `Escaper build()` | 【原文待译】Returns a new escaper based on the current state of the builder. |
| `com.google.common.escape.UnicodeEscaper` | `String escape(String string)` | 【原文待译】Returns the escaped form of a given literal string. If you are escaping input in arbitrary successive chunks, then it is not generally safe to use this method. If an input string ends with an unmatched high surrogate character, then this method will throw IllegalArgumentException. You should ensure … |
