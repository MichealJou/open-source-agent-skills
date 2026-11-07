# cn.hutool.core.text

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.text.ASCIIStrCache`

```java
public class cn.hutool.core.text.ASCIIStrCache {
  public cn.hutool.core.text.ASCIIStrCache();
  public static java.lang.String toString(char);
}
```

## `cn.hutool.core.text.AntPathMatcher`

```java
public class cn.hutool.core.text.AntPathMatcher {
  public cn.hutool.core.text.AntPathMatcher();
  public cn.hutool.core.text.AntPathMatcher(java.lang.String);
  public cn.hutool.core.text.AntPathMatcher setPathSeparator(java.lang.String);
  public cn.hutool.core.text.AntPathMatcher setCaseSensitive(boolean);
  public cn.hutool.core.text.AntPathMatcher setTrimTokens(boolean);
  public cn.hutool.core.text.AntPathMatcher setCachePatterns(boolean);
  public boolean isPattern(java.lang.String);
  public boolean match(java.lang.String, java.lang.String);
  public boolean matchStart(java.lang.String, java.lang.String);
  public java.lang.String extractPathWithinPattern(java.lang.String, java.lang.String);
  public java.util.Map<java.lang.String, java.lang.String> extractUriTemplateVariables(java.lang.String, java.lang.String);
  public java.lang.String combine(java.lang.String, java.lang.String);
  public java.util.Comparator<java.lang.String> getPatternComparator(java.lang.String);
}
```

## `cn.hutool.core.text.AntPathMatcher$AntPathStringMatcher`

```java
public class cn.hutool.core.text.AntPathMatcher$AntPathStringMatcher {
  public cn.hutool.core.text.AntPathMatcher$AntPathStringMatcher(java.lang.String, boolean);
  public boolean matchStrings(java.lang.String, java.util.Map<java.lang.String, java.lang.String>);
}
```

## `cn.hutool.core.text.AntPathMatcher$AntPatternComparator`

```java
public class cn.hutool.core.text.AntPathMatcher$AntPatternComparator implements java.util.Comparator<java.lang.String> {
  public cn.hutool.core.text.AntPathMatcher$AntPatternComparator(java.lang.String);
  public int compare(java.lang.String, java.lang.String);
  public int compare(java.lang.Object, java.lang.Object);
}
```

## `cn.hutool.core.text.CharSequenceUtil`

```java
public class cn.hutool.core.text.CharSequenceUtil {
  public cn.hutool.core.text.CharSequenceUtil();
  public static boolean isBlank(java.lang.CharSequence);
  public static boolean isNotBlank(java.lang.CharSequence);
  public static boolean hasBlank(java.lang.CharSequence...);
  public static boolean isAllBlank(java.lang.CharSequence...);
  public static boolean isEmpty(java.lang.CharSequence);
  public static boolean isNotEmpty(java.lang.CharSequence);
  public static java.lang.String emptyIfNull(java.lang.CharSequence);
  public static java.lang.String nullToEmpty(java.lang.CharSequence);
  public static java.lang.String nullToDefault(java.lang.CharSequence, java.lang.String);
  public static java.lang.String emptyToDefault(java.lang.CharSequence, java.lang.String);
  public static java.lang.String blankToDefault(java.lang.CharSequence, java.lang.String);
  public static java.lang.String emptyToNull(java.lang.CharSequence);
  public static boolean hasEmpty(java.lang.CharSequence...);
  public static boolean isAllEmpty(java.lang.CharSequence...);
  public static boolean isAllNotEmpty(java.lang.CharSequence...);
  public static boolean isAllNotBlank(java.lang.CharSequence...);
  public static boolean isNullOrUndefined(java.lang.CharSequence);
  public static boolean isEmptyOrUndefined(java.lang.CharSequence);
  public static boolean isBlankOrUndefined(java.lang.CharSequence);
  public static java.lang.String trim(java.lang.CharSequence);
  public static java.lang.String trimToEmpty(java.lang.CharSequence);
  public static java.lang.String trimToNull(java.lang.CharSequence);
  public static java.lang.String trimStart(java.lang.CharSequence);
  public static java.lang.String trimEnd(java.lang.CharSequence);
  public static java.lang.String trim(java.lang.CharSequence, int);
  public static java.lang.String trim(java.lang.CharSequence, int, java.util.function.Predicate<java.lang.Character>);
  public static boolean startWith(java.lang.CharSequence, char);
  public static boolean startWith(java.lang.CharSequence, java.lang.CharSequence, boolean);
  public static boolean startWith(java.lang.CharSequence, java.lang.CharSequence, boolean, boolean);
  public static boolean startWith(java.lang.CharSequence, java.lang.CharSequence);
  public static boolean startWithIgnoreEquals(java.lang.CharSequence, java.lang.CharSequence);
  public static boolean startWithIgnoreCase(java.lang.CharSequence, java.lang.CharSequence);
  public static boolean startWithAny(java.lang.CharSequence, java.lang.CharSequence...);
  public static boolean startWithAnyIgnoreCase(java.lang.CharSequence, java.lang.CharSequence...);
  public static boolean endWith(java.lang.CharSequence, char);
  public static boolean endWith(java.lang.CharSequence, java.lang.CharSequence, boolean);
  public static boolean endWith(java.lang.CharSequence, java.lang.CharSequence, boolean, boolean);
  public static boolean endWith(java.lang.CharSequence, java.lang.CharSequence);
  public static boolean endWithIgnoreCase(java.lang.CharSequence, java.lang.CharSequence);
  public static boolean endWithAny(java.lang.CharSequence, java.lang.CharSequence...);
  public static boolean endWithAnyIgnoreCase(java.lang.CharSequence, java.lang.CharSequence...);
  public static boolean contains(java.lang.CharSequence, char);
  public static boolean contains(java.lang.CharSequence, java.lang.CharSequence);
  public static boolean containsAny(java.lang.CharSequence, java.lang.CharSequence...);
  public static boolean containsAny(java.lang.CharSequence, char...);
  public static boolean containsOnly(java.lang.CharSequence, char...);
  public static boolean containsAll(java.lang.CharSequence, java.lang.CharSequence...);
  public static boolean containsBlank(java.lang.CharSequence);
  public static java.lang.String getContainsStr(java.lang.CharSequence, java.lang.CharSequence...);
  public static boolean containsIgnoreCase(java.lang.CharSequence, java.lang.CharSequence);
  public static boolean containsAnyIgnoreCase(java.lang.CharSequence, java.lang.CharSequence...);
  public static java.lang.String getContainsStrIgnoreCase(java.lang.CharSequence, java.lang.CharSequence...);
  public static int indexOf(java.lang.CharSequence, char);
  public static int indexOf(java.lang.CharSequence, char, int);
  public static int indexOf(java.lang.CharSequence, char, int, int);
  public static int indexOfIgnoreCase(java.lang.CharSequence, java.lang.CharSequence);
  public static int indexOfIgnoreCase(java.lang.CharSequence, java.lang.CharSequence, int);
  public static int indexOf(java.lang.CharSequence, java.lang.CharSequence, int, boolean);
  public static int lastIndexOfIgnoreCase(java.lang.CharSequence, java.lang.CharSequence);
  public static int lastIndexOfIgnoreCase(java.lang.CharSequence, java.lang.CharSequence, int);
  public static int lastIndexOf(java.lang.CharSequence, java.lang.CharSequence, int, boolean);
  public static int ordinalIndexOf(java.lang.CharSequence, java.lang.CharSequence, int);
  public static java.lang.String removeAll(java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String removeAny(java.lang.CharSequence, java.lang.CharSequence...);
  public static java.lang.String removeAll(java.lang.CharSequence, char...);
  public static java.lang.String removeAllLineBreaks(java.lang.CharSequence);
  public static java.lang.String removePreAndLowerFirst(java.lang.CharSequence, int);
  public static java.lang.String removePreAndLowerFirst(java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String removePrefix(java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String removeAllPrefix(java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String removePrefixIgnoreCase(java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String removeSuffix(java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String removeAllSuffix(java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String removeSufAndLowerFirst(java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String removeSuffixIgnoreCase(java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String cleanBlank(java.lang.CharSequence);
  public static java.lang.String stripIgnoreCase(java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String stripIgnoreCase(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String strip(java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String strip(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String strip(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence, boolean);
  public static java.lang.String stripAll(java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String stripAll(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String addPrefixIfNot(java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String addSuffixIfNot(java.lang.CharSequence, java.lang.CharSequence);
  public static long[] splitToLong(java.lang.CharSequence, char);
  public static long[] splitToLong(java.lang.CharSequence, java.lang.CharSequence);
  public static int[] splitToInt(java.lang.CharSequence, char);
  public static int[] splitToInt(java.lang.CharSequence, java.lang.CharSequence);
  public static java.util.List<java.lang.String> split(java.lang.CharSequence, char);
  public static java.lang.String[] splitToArray(java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String[] splitToArray(java.lang.CharSequence, char);
  public static java.lang.String[] splitToArray(java.lang.CharSequence, char, int);
  public static java.util.List<java.lang.String> split(java.lang.CharSequence, char, int);
  public static java.util.List<java.lang.String> splitTrim(java.lang.CharSequence, char);
  public static java.util.List<java.lang.String> splitTrim(java.lang.CharSequence, java.lang.CharSequence);
  public static java.util.List<java.lang.String> splitTrim(java.lang.CharSequence, char, int);
  public static java.util.List<java.lang.String> splitTrim(java.lang.CharSequence, java.lang.CharSequence, int);
  public static java.util.List<java.lang.String> split(java.lang.CharSequence, char, boolean, boolean);
  public static java.util.List<java.lang.String> split(java.lang.CharSequence, char, int, boolean, boolean);
  public static <R> java.util.List<R> split(java.lang.CharSequence, char, int, boolean, java.util.function.Function<java.lang.String, R>);
  public static java.util.List<java.lang.String> split(java.lang.CharSequence, java.lang.CharSequence);
  public static java.util.List<java.lang.String> split(java.lang.CharSequence, java.lang.CharSequence, boolean, boolean);
  public static java.util.List<java.lang.String> split(java.lang.CharSequence, java.lang.CharSequence, int, boolean, boolean);
  public static java.lang.String[] split(java.lang.CharSequence, int);
  public static java.lang.String[] cut(java.lang.CharSequence, int);
  public static java.lang.String sub(java.lang.CharSequence, int, int);
  public static java.lang.String subByCodePoint(java.lang.CharSequence, int, int);
  public static java.lang.String subPreGbk(java.lang.CharSequence, int, java.lang.CharSequence);
  public static java.lang.String subPreGbk(java.lang.CharSequence, int, boolean);
  public static java.lang.String subPre(java.lang.CharSequence, int);
  public static java.lang.String subSuf(java.lang.CharSequence, int);
  public static java.lang.String subSufByLength(java.lang.CharSequence, int);
  public static java.lang.String subWithLength(java.lang.String, int, int);
  public static java.lang.String subBefore(java.lang.CharSequence, java.lang.CharSequence, boolean);
  public static java.lang.String subBefore(java.lang.CharSequence, char, boolean);
  public static java.lang.String subAfter(java.lang.CharSequence, java.lang.CharSequence, boolean);
  public static java.lang.String subAfter(java.lang.CharSequence, char, boolean);
  public static java.lang.String subBetween(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String subBetween(java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String[] subBetweenAll(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String[] subBetweenAll(java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String repeat(char, int);
  public static java.lang.String repeat(java.lang.CharSequence, int);
  public static java.lang.String repeatByLength(java.lang.CharSequence, int);
  public static java.lang.String repeatAndJoin(java.lang.CharSequence, int, java.lang.CharSequence);
  public static boolean equals(java.lang.CharSequence, java.lang.CharSequence);
  public static boolean equalsIgnoreCase(java.lang.CharSequence, java.lang.CharSequence);
  public static boolean equals(java.lang.CharSequence, java.lang.CharSequence, boolean);
  public static boolean equalsAnyIgnoreCase(java.lang.CharSequence, java.lang.CharSequence...);
  public static boolean equalsAny(java.lang.CharSequence, java.lang.CharSequence...);
  public static boolean equalsAny(java.lang.CharSequence, boolean, java.lang.CharSequence...);
  public static boolean equalsCharAt(java.lang.CharSequence, int, char);
  public static boolean isSubEquals(java.lang.CharSequence, int, java.lang.CharSequence, boolean);
  public static boolean isSubEquals(java.lang.CharSequence, int, java.lang.CharSequence, int, int, boolean);
  public static java.lang.String format(java.lang.CharSequence, java.lang.Object...);
  public static java.lang.String indexedFormat(java.lang.CharSequence, java.lang.Object...);
  public static byte[] utf8Bytes(java.lang.CharSequence);
  public static byte[] bytes(java.lang.CharSequence);
  public static byte[] bytes(java.lang.CharSequence, java.lang.String);
  public static byte[] bytes(java.lang.CharSequence, java.nio.charset.Charset);
  public static java.nio.ByteBuffer byteBuffer(java.lang.CharSequence, java.lang.String);
  public static java.lang.String wrap(java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String wrap(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String[] wrapAllWithPair(java.lang.CharSequence, java.lang.CharSequence...);
  public static java.lang.String[] wrapAll(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence...);
  public static java.lang.String wrapIfMissing(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String[] wrapAllWithPairIfMissing(java.lang.CharSequence, java.lang.CharSequence...);
  public static java.lang.String[] wrapAllIfMissing(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence...);
  public static java.lang.String unWrap(java.lang.CharSequence, java.lang.String, java.lang.String);
  public static java.lang.String unWrap(java.lang.CharSequence, char, char);
  public static java.lang.String unWrap(java.lang.CharSequence, char);
  public static boolean isWrap(java.lang.CharSequence, java.lang.String, java.lang.String);
  public static boolean isWrap(java.lang.CharSequence, java.lang.String);
  public static boolean isWrap(java.lang.CharSequence, char);
  public static boolean isWrap(java.lang.CharSequence, char, char);
  public static java.lang.String padPre(java.lang.CharSequence, int, java.lang.CharSequence);
  public static java.lang.String padPre(java.lang.CharSequence, int, char);
  public static java.lang.String padAfter(java.lang.CharSequence, int, char);
  public static java.lang.String padAfter(java.lang.CharSequence, int, java.lang.CharSequence);
  public static java.lang.String center(java.lang.CharSequence, int);
  public static java.lang.String center(java.lang.CharSequence, int, char);
  public static java.lang.String center(java.lang.CharSequence, int, java.lang.CharSequence);
  public static java.lang.String str(java.lang.CharSequence);
  public static int count(java.lang.CharSequence, java.lang.CharSequence);
  public static int count(java.lang.CharSequence, char);
  public static int compare(java.lang.CharSequence, java.lang.CharSequence, boolean);
  public static int compareIgnoreCase(java.lang.CharSequence, java.lang.CharSequence, boolean);
  public static int compareVersion(java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String appendIfMissing(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence...);
  public static java.lang.String appendIfMissingIgnoreCase(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence...);
  public static java.lang.String appendIfMissing(java.lang.CharSequence, java.lang.CharSequence, boolean, java.lang.CharSequence...);
  public static java.lang.String prependIfMissing(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence...);
  public static java.lang.String prependIfMissingIgnoreCase(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence...);
  public static java.lang.String prependIfMissing(java.lang.CharSequence, java.lang.CharSequence, boolean, java.lang.CharSequence...);
  public static java.lang.String replaceIgnoreCase(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String replace(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String replace(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence, boolean);
  public static java.lang.String replace(java.lang.CharSequence, int, java.lang.CharSequence, java.lang.CharSequence, boolean);
  public static java.lang.String replace(java.lang.CharSequence, int, int, char);
  public static java.lang.String replaceByCodePoint(java.lang.CharSequence, int, int, char);
  public static java.lang.String replace(java.lang.CharSequence, int, int, java.lang.CharSequence);
  public static java.lang.String replaceByCodePoint(java.lang.CharSequence, int, int, java.lang.CharSequence);
  public static java.lang.String replace(java.lang.CharSequence, java.util.regex.Pattern, cn.hutool.core.lang.func.Func1<java.util.regex.Matcher, java.lang.String>);
  public static java.lang.String replace(java.lang.CharSequence, java.lang.String, cn.hutool.core.lang.func.Func1<java.util.regex.Matcher, java.lang.String>);
  public static java.lang.String replaceLast(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String replaceLast(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence, boolean);
  public static java.lang.String replaceFirst(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String replaceFirst(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence, boolean);
  public static java.lang.String hide(java.lang.CharSequence, int, int);
  public static java.lang.String desensitized(java.lang.CharSequence, cn.hutool.core.util.DesensitizedUtil$DesensitizedType);
  public static java.lang.String replaceChars(java.lang.CharSequence, java.lang.String, java.lang.CharSequence);
  public static java.lang.String replaceChars(java.lang.CharSequence, char[], java.lang.CharSequence);
  public static int length(java.lang.CharSequence);
  public static int byteLength(java.lang.CharSequence, java.nio.charset.Charset);
  public static int totalLength(java.lang.CharSequence...);
  public static java.lang.String maxLength(java.lang.CharSequence, int);
  public static <T extends java.lang.CharSequence> T firstNonNull(T...);
  public static <T extends java.lang.CharSequence> T firstNonEmpty(T...);
  public static <T extends java.lang.CharSequence> T firstNonBlank(T...);
  public static java.lang.String toLoweCase(java.lang.CharSequence);
  public static java.lang.String toLowerCase(java.lang.CharSequence);
  public static java.lang.String toUpperCase(java.lang.CharSequence);
  public static java.lang.String upperFirstAndAddPre(java.lang.CharSequence, java.lang.String);
  public static java.lang.String upperFirst(java.lang.CharSequence);
  public static java.lang.String lowerFirst(java.lang.CharSequence);
  public static java.lang.String filter(java.lang.CharSequence, cn.hutool.core.lang.Filter<java.lang.Character>);
  public static boolean isUpperCase(java.lang.CharSequence);
  public static boolean isLowerCase(java.lang.CharSequence);
  public static java.lang.String swapCase(java.lang.String);
  public static java.lang.String toUnderlineCase(java.lang.CharSequence);
  public static java.lang.String toSymbolCase(java.lang.CharSequence, char);
  public static java.lang.String toCamelCase(java.lang.CharSequence);
  public static java.lang.String toCamelCase(java.lang.CharSequence, char);
  public static boolean isSurround(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence);
  public static boolean isSurround(java.lang.CharSequence, char, char);
  public static java.lang.StringBuilder builder(java.lang.CharSequence...);
  public static java.lang.StringBuilder builder(java.util.function.Function<java.lang.CharSequence, java.lang.CharSequence>, java.lang.CharSequence...);
  public static cn.hutool.core.text.StrBuilder strBuilder(java.lang.CharSequence...);
  public static java.lang.String getGeneralField(java.lang.CharSequence);
  public static java.lang.String genSetter(java.lang.CharSequence);
  public static java.lang.String genGetter(java.lang.CharSequence);
  public static java.lang.String concat(boolean, java.lang.CharSequence...);
  public static java.lang.String brief(java.lang.CharSequence, int);
  public static java.lang.String join(java.lang.CharSequence, java.lang.Object...);
  public static <T> java.lang.String join(java.lang.CharSequence, java.lang.Iterable<T>);
  public static boolean isAllCharMatch(java.lang.CharSequence, cn.hutool.core.lang.Matcher<java.lang.Character>);
  public static boolean isNumeric(java.lang.CharSequence);
  public static java.lang.String move(java.lang.CharSequence, int, int, int);
  public static boolean isCharEquals(java.lang.CharSequence);
  public static java.lang.String normalize(java.lang.CharSequence);
  public static java.lang.String fixLength(java.lang.CharSequence, char, int);
  public static boolean hasLetter(java.lang.CharSequence);
  public static java.lang.CharSequence commonPrefix(java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.CharSequence commonSuffix(java.lang.CharSequence, java.lang.CharSequence);
}
```

## `cn.hutool.core.text.NamingCase`

```java
public class cn.hutool.core.text.NamingCase {
  public cn.hutool.core.text.NamingCase();
  public static java.lang.String toUnderlineCase(java.lang.CharSequence);
  public static java.lang.String toKebabCase(java.lang.CharSequence);
  public static java.lang.String toSymbolCase(java.lang.CharSequence, char);
  public static java.lang.String toPascalCase(java.lang.CharSequence);
  public static java.lang.String toCamelCase(java.lang.CharSequence);
  public static java.lang.String toCamelCase(java.lang.CharSequence, char);
  public static java.lang.String toCamelCase(java.lang.CharSequence, char, boolean);
}
```

## `cn.hutool.core.text.PasswdStrength`

```java
public class cn.hutool.core.text.PasswdStrength {
  public cn.hutool.core.text.PasswdStrength();
  public static int check(java.lang.String);
  public static cn.hutool.core.text.PasswdStrength$PASSWD_LEVEL getLevel(java.lang.String);
}
```

## `cn.hutool.core.text.PasswdStrength$CHAR_TYPE`

```java
public final class cn.hutool.core.text.PasswdStrength$CHAR_TYPE extends java.lang.Enum<cn.hutool.core.text.PasswdStrength$CHAR_TYPE> {
  public static cn.hutool.core.text.PasswdStrength$CHAR_TYPE[] values();
  public static cn.hutool.core.text.PasswdStrength$CHAR_TYPE valueOf(java.lang.String);
}
```

## `cn.hutool.core.text.PasswdStrength$PASSWD_LEVEL`

```java
public final class cn.hutool.core.text.PasswdStrength$PASSWD_LEVEL extends java.lang.Enum<cn.hutool.core.text.PasswdStrength$PASSWD_LEVEL> {
  public static cn.hutool.core.text.PasswdStrength$PASSWD_LEVEL[] values();
  public static cn.hutool.core.text.PasswdStrength$PASSWD_LEVEL valueOf(java.lang.String);
}
```

## `cn.hutool.core.text.Simhash`

```java
public class cn.hutool.core.text.Simhash {
  public cn.hutool.core.text.Simhash();
  public cn.hutool.core.text.Simhash(int, int);
  public long hash(java.util.Collection<? extends java.lang.CharSequence>);
  public boolean equals(java.util.Collection<? extends java.lang.CharSequence>);
  public void store(java.lang.Long);
}
```

## `cn.hutool.core.text.StrBuilder`

```java
public class cn.hutool.core.text.StrBuilder implements java.lang.CharSequence,java.lang.Appendable,java.io.Serializable {
  public static cn.hutool.core.text.StrBuilder create();
  public static cn.hutool.core.text.StrBuilder create(int);
  public static cn.hutool.core.text.StrBuilder create(java.lang.CharSequence...);
  public cn.hutool.core.text.StrBuilder();
  public cn.hutool.core.text.StrBuilder(int);
  public cn.hutool.core.text.StrBuilder(java.lang.CharSequence...);
  public cn.hutool.core.text.StrBuilder append(java.lang.Object);
  public cn.hutool.core.text.StrBuilder append(char);
  public cn.hutool.core.text.StrBuilder append(char[]);
  public cn.hutool.core.text.StrBuilder append(char[], int, int);
  public cn.hutool.core.text.StrBuilder append(java.lang.CharSequence);
  public cn.hutool.core.text.StrBuilder append(java.lang.CharSequence, int, int);
  public cn.hutool.core.text.StrBuilder insert(int, java.lang.Object);
  public cn.hutool.core.text.StrBuilder insert(int, char);
  public cn.hutool.core.text.StrBuilder insert(int, char[]);
  public cn.hutool.core.text.StrBuilder insert(int, char[], int, int);
  public cn.hutool.core.text.StrBuilder insert(int, java.lang.CharSequence);
  public cn.hutool.core.text.StrBuilder insert(int, java.lang.CharSequence, int, int);
  public cn.hutool.core.text.StrBuilder getChars(int, int, char[], int);
  public boolean hasContent();
  public boolean isEmpty();
  public cn.hutool.core.text.StrBuilder clear();
  public cn.hutool.core.text.StrBuilder reset();
  public cn.hutool.core.text.StrBuilder delTo(int);
  public cn.hutool.core.text.StrBuilder del(int, int) throws java.lang.StringIndexOutOfBoundsException;
  public java.lang.String toString(boolean);
  public java.lang.String toStringAndReset();
  public java.lang.String toString();
  public int length();
  public char charAt(int);
  public java.lang.CharSequence subSequence(int, int);
  public java.lang.String subString(int);
  public java.lang.String subString(int, int);
  public java.lang.Appendable append(char) throws java.io.IOException;
  public java.lang.Appendable append(java.lang.CharSequence, int, int) throws java.io.IOException;
  public java.lang.Appendable append(java.lang.CharSequence) throws java.io.IOException;
}
```

## `cn.hutool.core.text.StrFormatter`

```java
public class cn.hutool.core.text.StrFormatter {
  public cn.hutool.core.text.StrFormatter();
  public static java.lang.String format(java.lang.String, java.lang.Object...);
  public static java.lang.String formatWith(java.lang.String, java.lang.String, java.lang.Object...);
  public static java.lang.String format(java.lang.CharSequence, java.util.Map<?, ?>, boolean);
}
```

## `cn.hutool.core.text.StrJoiner`

```java
public class cn.hutool.core.text.StrJoiner implements java.lang.Appendable,java.io.Serializable {
  public static cn.hutool.core.text.StrJoiner of(cn.hutool.core.text.StrJoiner);
  public static cn.hutool.core.text.StrJoiner of(java.lang.CharSequence);
  public static cn.hutool.core.text.StrJoiner of(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence);
  public cn.hutool.core.text.StrJoiner(java.lang.CharSequence);
  public cn.hutool.core.text.StrJoiner(java.lang.Appendable, java.lang.CharSequence);
  public cn.hutool.core.text.StrJoiner(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence);
  public cn.hutool.core.text.StrJoiner(java.lang.Appendable, java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence);
  public cn.hutool.core.text.StrJoiner setDelimiter(java.lang.CharSequence);
  public cn.hutool.core.text.StrJoiner setPrefix(java.lang.CharSequence);
  public cn.hutool.core.text.StrJoiner setSuffix(java.lang.CharSequence);
  public cn.hutool.core.text.StrJoiner setWrapElement(boolean);
  public cn.hutool.core.text.StrJoiner setNullMode(cn.hutool.core.text.StrJoiner$NullMode);
  public cn.hutool.core.text.StrJoiner setEmptyResult(java.lang.String);
  public cn.hutool.core.text.StrJoiner append(java.lang.Object);
  public <T> cn.hutool.core.text.StrJoiner append(T[]);
  public <T> cn.hutool.core.text.StrJoiner append(java.util.Iterator<T>);
  public <T> cn.hutool.core.text.StrJoiner append(T[], java.util.function.Function<T, ? extends java.lang.CharSequence>);
  public <E> cn.hutool.core.text.StrJoiner append(java.lang.Iterable<E>, java.util.function.Function<? super E, ? extends java.lang.CharSequence>);
  public <E> cn.hutool.core.text.StrJoiner append(java.util.Iterator<E>, java.util.function.Function<? super E, ? extends java.lang.CharSequence>);
  public cn.hutool.core.text.StrJoiner append(java.lang.CharSequence);
  public cn.hutool.core.text.StrJoiner append(java.lang.CharSequence, int, int);
  public cn.hutool.core.text.StrJoiner append(char);
  public cn.hutool.core.text.StrJoiner merge(cn.hutool.core.text.StrJoiner);
  public int length();
  public java.lang.String toString();
  public java.lang.Appendable append(char) throws java.io.IOException;
  public java.lang.Appendable append(java.lang.CharSequence, int, int) throws java.io.IOException;
  public java.lang.Appendable append(java.lang.CharSequence) throws java.io.IOException;
}
```

## `cn.hutool.core.text.StrJoiner$NullMode`

```java
public final class cn.hutool.core.text.StrJoiner$NullMode extends java.lang.Enum<cn.hutool.core.text.StrJoiner$NullMode> {
  public static cn.hutool.core.text.StrJoiner$NullMode[] values();
  public static cn.hutool.core.text.StrJoiner$NullMode valueOf(java.lang.String);
}
```

## `cn.hutool.core.text.StrMatcher`

```java
public class cn.hutool.core.text.StrMatcher {
  public cn.hutool.core.text.StrMatcher(java.lang.String);
  public java.util.Map<java.lang.String, java.lang.String> match(java.lang.String);
}
```

## `cn.hutool.core.text.StrSplitter`

```java
public class cn.hutool.core.text.StrSplitter {
  public cn.hutool.core.text.StrSplitter();
  public static java.util.List<java.lang.String> splitPath(java.lang.CharSequence);
  public static java.lang.String[] splitPathToArray(java.lang.CharSequence);
  public static java.util.List<java.lang.String> splitPath(java.lang.CharSequence, int);
  public static java.lang.String[] splitPathToArray(java.lang.CharSequence, int);
  public static java.util.List<java.lang.String> splitTrim(java.lang.CharSequence, char, boolean);
  public static java.util.List<java.lang.String> split(java.lang.CharSequence, char, boolean, boolean);
  public static java.util.List<java.lang.String> splitTrim(java.lang.CharSequence, char, int, boolean);
  public static java.util.List<java.lang.String> split(java.lang.CharSequence, char, int, boolean, boolean);
  public static <R> java.util.List<R> split(java.lang.CharSequence, char, int, boolean, java.util.function.Function<java.lang.String, R>);
  public static java.util.List<java.lang.String> splitIgnoreCase(java.lang.CharSequence, char, int, boolean, boolean);
  public static java.util.List<java.lang.String> split(java.lang.CharSequence, char, int, boolean, boolean, boolean);
  public static <R> java.util.List<R> split(java.lang.CharSequence, char, int, boolean, boolean, java.util.function.Function<java.lang.String, R>);
  public static java.lang.String[] splitToArray(java.lang.CharSequence, char, int, boolean, boolean);
  public static java.util.List<java.lang.String> split(java.lang.CharSequence, java.lang.String, boolean, boolean);
  public static java.util.List<java.lang.String> splitTrim(java.lang.CharSequence, java.lang.String, boolean);
  public static java.util.List<java.lang.String> split(java.lang.CharSequence, java.lang.String, int, boolean, boolean);
  public static java.util.List<java.lang.String> splitTrim(java.lang.CharSequence, java.lang.String, int, boolean);
  public static java.util.List<java.lang.String> splitIgnoreCase(java.lang.CharSequence, java.lang.String, int, boolean, boolean);
  public static java.util.List<java.lang.String> splitTrimIgnoreCase(java.lang.CharSequence, java.lang.String, int, boolean);
  public static java.util.List<java.lang.String> split(java.lang.CharSequence, java.lang.String, int, boolean, boolean, boolean);
  public static java.lang.String[] splitToArray(java.lang.CharSequence, java.lang.String, int, boolean, boolean);
  public static java.util.List<java.lang.String> split(java.lang.CharSequence, int);
  public static java.lang.String[] splitToArray(java.lang.String, int);
  public static java.util.List<java.lang.String> splitByRegex(java.lang.String, java.lang.String, int, boolean, boolean);
  public static java.util.List<java.lang.String> split(java.lang.String, java.util.regex.Pattern, int, boolean, boolean);
  public static java.lang.String[] splitToArray(java.lang.String, java.util.regex.Pattern, int, boolean, boolean);
  public static java.lang.String[] splitByLength(java.lang.CharSequence, int);
}
```

## `cn.hutool.core.text.TextSimilarity`

```java
public class cn.hutool.core.text.TextSimilarity {
  public cn.hutool.core.text.TextSimilarity();
  public static double similar(java.lang.String, java.lang.String);
  public static java.lang.String similar(java.lang.String, java.lang.String, int);
  public static java.lang.String longestCommonSubstring(java.lang.String, java.lang.String);
}
```

## `cn.hutool.core.text.UnicodeUtil`

```java
public class cn.hutool.core.text.UnicodeUtil {
  public cn.hutool.core.text.UnicodeUtil();
  public static java.lang.String toString(java.lang.String);
  public static java.lang.String toUnicode(char);
  public static java.lang.String toUnicode(int);
  public static java.lang.String toUnicode(java.lang.String);
  public static java.lang.String toUnicode(java.lang.String, boolean);
}
```
