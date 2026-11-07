# com.feilong.lib.lang3.text

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.lang3.text.StrBuilder`

```java
public class com.feilong.lib.lang3.text.StrBuilder implements java.lang.CharSequence,java.lang.Appendable,java.io.Serializable {
  public com.feilong.lib.lang3.text.StrBuilder();
  public com.feilong.lib.lang3.text.StrBuilder(int);
  public com.feilong.lib.lang3.text.StrBuilder(java.lang.String);
  public java.lang.String getNewLineText();
  public com.feilong.lib.lang3.text.StrBuilder setNewLineText(java.lang.String);
  public java.lang.String getNullText();
  public com.feilong.lib.lang3.text.StrBuilder setNullText(java.lang.String);
  public int length();
  public com.feilong.lib.lang3.text.StrBuilder setLength(int);
  public int capacity();
  public com.feilong.lib.lang3.text.StrBuilder ensureCapacity(int);
  public com.feilong.lib.lang3.text.StrBuilder minimizeCapacity();
  public int size();
  public boolean isEmpty();
  public com.feilong.lib.lang3.text.StrBuilder clear();
  public char charAt(int);
  public com.feilong.lib.lang3.text.StrBuilder setCharAt(int, char);
  public com.feilong.lib.lang3.text.StrBuilder deleteCharAt(int);
  public char[] toCharArray();
  public char[] toCharArray(int, int);
  public char[] getChars(char[]);
  public void getChars(int, int, char[], int);
  public int readFrom(java.lang.Readable) throws java.io.IOException;
  public com.feilong.lib.lang3.text.StrBuilder appendNewLine();
  public com.feilong.lib.lang3.text.StrBuilder appendNull();
  public com.feilong.lib.lang3.text.StrBuilder append(java.lang.Object);
  public com.feilong.lib.lang3.text.StrBuilder append(java.lang.CharSequence);
  public com.feilong.lib.lang3.text.StrBuilder append(java.lang.CharSequence, int, int);
  public com.feilong.lib.lang3.text.StrBuilder append(java.lang.String);
  public com.feilong.lib.lang3.text.StrBuilder append(java.lang.String, int, int);
  public com.feilong.lib.lang3.text.StrBuilder append(java.lang.String, java.lang.Object...);
  public com.feilong.lib.lang3.text.StrBuilder append(java.nio.CharBuffer);
  public com.feilong.lib.lang3.text.StrBuilder append(java.nio.CharBuffer, int, int);
  public com.feilong.lib.lang3.text.StrBuilder append(java.lang.StringBuffer);
  public com.feilong.lib.lang3.text.StrBuilder append(java.lang.StringBuffer, int, int);
  public com.feilong.lib.lang3.text.StrBuilder append(java.lang.StringBuilder);
  public com.feilong.lib.lang3.text.StrBuilder append(java.lang.StringBuilder, int, int);
  public com.feilong.lib.lang3.text.StrBuilder append(com.feilong.lib.lang3.text.StrBuilder);
  public com.feilong.lib.lang3.text.StrBuilder append(com.feilong.lib.lang3.text.StrBuilder, int, int);
  public com.feilong.lib.lang3.text.StrBuilder append(char[]);
  public com.feilong.lib.lang3.text.StrBuilder append(char[], int, int);
  public com.feilong.lib.lang3.text.StrBuilder append(boolean);
  public com.feilong.lib.lang3.text.StrBuilder append(char);
  public com.feilong.lib.lang3.text.StrBuilder append(int);
  public com.feilong.lib.lang3.text.StrBuilder append(long);
  public com.feilong.lib.lang3.text.StrBuilder append(float);
  public com.feilong.lib.lang3.text.StrBuilder append(double);
  public com.feilong.lib.lang3.text.StrBuilder appendln(java.lang.Object);
  public com.feilong.lib.lang3.text.StrBuilder appendln(java.lang.String);
  public com.feilong.lib.lang3.text.StrBuilder appendln(java.lang.String, int, int);
  public com.feilong.lib.lang3.text.StrBuilder appendln(java.lang.String, java.lang.Object...);
  public com.feilong.lib.lang3.text.StrBuilder appendln(java.lang.StringBuffer);
  public com.feilong.lib.lang3.text.StrBuilder appendln(java.lang.StringBuilder);
  public com.feilong.lib.lang3.text.StrBuilder appendln(java.lang.StringBuilder, int, int);
  public com.feilong.lib.lang3.text.StrBuilder appendln(java.lang.StringBuffer, int, int);
  public com.feilong.lib.lang3.text.StrBuilder appendln(com.feilong.lib.lang3.text.StrBuilder);
  public com.feilong.lib.lang3.text.StrBuilder appendln(com.feilong.lib.lang3.text.StrBuilder, int, int);
  public com.feilong.lib.lang3.text.StrBuilder appendln(char[]);
  public com.feilong.lib.lang3.text.StrBuilder appendln(char[], int, int);
  public com.feilong.lib.lang3.text.StrBuilder appendln(boolean);
  public com.feilong.lib.lang3.text.StrBuilder appendln(char);
  public com.feilong.lib.lang3.text.StrBuilder appendln(int);
  public com.feilong.lib.lang3.text.StrBuilder appendln(long);
  public com.feilong.lib.lang3.text.StrBuilder appendln(float);
  public com.feilong.lib.lang3.text.StrBuilder appendln(double);
  public <T> com.feilong.lib.lang3.text.StrBuilder appendAll(T...);
  public com.feilong.lib.lang3.text.StrBuilder appendAll(java.lang.Iterable<?>);
  public com.feilong.lib.lang3.text.StrBuilder appendAll(java.util.Iterator<?>);
  public com.feilong.lib.lang3.text.StrBuilder appendWithSeparators(java.lang.Object[], java.lang.String);
  public com.feilong.lib.lang3.text.StrBuilder appendWithSeparators(java.lang.Iterable<?>, java.lang.String);
  public com.feilong.lib.lang3.text.StrBuilder appendWithSeparators(java.util.Iterator<?>, java.lang.String);
  public com.feilong.lib.lang3.text.StrBuilder appendSeparator(java.lang.String);
  public com.feilong.lib.lang3.text.StrBuilder appendSeparator(java.lang.String, java.lang.String);
  public com.feilong.lib.lang3.text.StrBuilder appendSeparator(char);
  public com.feilong.lib.lang3.text.StrBuilder appendSeparator(char, char);
  public com.feilong.lib.lang3.text.StrBuilder appendSeparator(java.lang.String, int);
  public com.feilong.lib.lang3.text.StrBuilder appendSeparator(char, int);
  public com.feilong.lib.lang3.text.StrBuilder appendPadding(int, char);
  public com.feilong.lib.lang3.text.StrBuilder appendFixedWidthPadLeft(java.lang.Object, int, char);
  public com.feilong.lib.lang3.text.StrBuilder appendFixedWidthPadLeft(int, int, char);
  public com.feilong.lib.lang3.text.StrBuilder appendFixedWidthPadRight(java.lang.Object, int, char);
  public com.feilong.lib.lang3.text.StrBuilder appendFixedWidthPadRight(int, int, char);
  public com.feilong.lib.lang3.text.StrBuilder insert(int, java.lang.Object);
  public com.feilong.lib.lang3.text.StrBuilder insert(int, java.lang.String);
  public com.feilong.lib.lang3.text.StrBuilder insert(int, char[]);
  public com.feilong.lib.lang3.text.StrBuilder insert(int, char[], int, int);
  public com.feilong.lib.lang3.text.StrBuilder insert(int, boolean);
  public com.feilong.lib.lang3.text.StrBuilder insert(int, char);
  public com.feilong.lib.lang3.text.StrBuilder insert(int, int);
  public com.feilong.lib.lang3.text.StrBuilder insert(int, long);
  public com.feilong.lib.lang3.text.StrBuilder insert(int, float);
  public com.feilong.lib.lang3.text.StrBuilder insert(int, double);
  public com.feilong.lib.lang3.text.StrBuilder delete(int, int);
  public com.feilong.lib.lang3.text.StrBuilder deleteAll(char);
  public com.feilong.lib.lang3.text.StrBuilder deleteFirst(char);
  public com.feilong.lib.lang3.text.StrBuilder deleteAll(java.lang.String);
  public com.feilong.lib.lang3.text.StrBuilder deleteFirst(java.lang.String);
  public com.feilong.lib.lang3.text.StrBuilder deleteAll(com.feilong.lib.lang3.text.StrMatcher);
  public com.feilong.lib.lang3.text.StrBuilder deleteFirst(com.feilong.lib.lang3.text.StrMatcher);
  public com.feilong.lib.lang3.text.StrBuilder replace(int, int, java.lang.String);
  public com.feilong.lib.lang3.text.StrBuilder replaceAll(char, char);
  public com.feilong.lib.lang3.text.StrBuilder replaceFirst(char, char);
  public com.feilong.lib.lang3.text.StrBuilder replaceAll(java.lang.String, java.lang.String);
  public com.feilong.lib.lang3.text.StrBuilder replaceFirst(java.lang.String, java.lang.String);
  public com.feilong.lib.lang3.text.StrBuilder replaceAll(com.feilong.lib.lang3.text.StrMatcher, java.lang.String);
  public com.feilong.lib.lang3.text.StrBuilder replaceFirst(com.feilong.lib.lang3.text.StrMatcher, java.lang.String);
  public com.feilong.lib.lang3.text.StrBuilder replace(com.feilong.lib.lang3.text.StrMatcher, java.lang.String, int, int, int);
  public com.feilong.lib.lang3.text.StrBuilder reverse();
  public com.feilong.lib.lang3.text.StrBuilder trim();
  public boolean startsWith(java.lang.String);
  public boolean endsWith(java.lang.String);
  public java.lang.CharSequence subSequence(int, int);
  public java.lang.String substring(int);
  public java.lang.String substring(int, int);
  public java.lang.String leftString(int);
  public java.lang.String rightString(int);
  public java.lang.String midString(int, int);
  public boolean contains(char);
  public boolean contains(java.lang.String);
  public boolean contains(com.feilong.lib.lang3.text.StrMatcher);
  public int indexOf(char);
  public int indexOf(char, int);
  public int indexOf(java.lang.String);
  public int indexOf(java.lang.String, int);
  public int indexOf(com.feilong.lib.lang3.text.StrMatcher);
  public int indexOf(com.feilong.lib.lang3.text.StrMatcher, int);
  public int lastIndexOf(char);
  public int lastIndexOf(char, int);
  public int lastIndexOf(java.lang.String);
  public int lastIndexOf(java.lang.String, int);
  public int lastIndexOf(com.feilong.lib.lang3.text.StrMatcher);
  public int lastIndexOf(com.feilong.lib.lang3.text.StrMatcher, int);
  public java.io.Reader asReader();
  public java.io.Writer asWriter();
  public void appendTo(java.lang.Appendable) throws java.io.IOException;
  public boolean equalsIgnoreCase(com.feilong.lib.lang3.text.StrBuilder);
  public boolean equals(com.feilong.lib.lang3.text.StrBuilder);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
  public java.lang.StringBuffer toStringBuffer();
  public java.lang.StringBuilder toStringBuilder();
  public java.lang.Appendable append(char) throws java.io.IOException;
  public java.lang.Appendable append(java.lang.CharSequence, int, int) throws java.io.IOException;
  public java.lang.Appendable append(java.lang.CharSequence) throws java.io.IOException;
}
```

## `com.feilong.lib.lang3.text.StrLookup`

```java
public abstract class com.feilong.lib.lang3.text.StrLookup<V> {
  public static <V> com.feilong.lib.lang3.text.StrLookup<V> mapLookup(java.util.Map<java.lang.String, V>);
  public abstract java.lang.String lookup(java.lang.String);
}
```

## `com.feilong.lib.lang3.text.StrMatcher`

```java
public abstract class com.feilong.lib.lang3.text.StrMatcher {
  public static com.feilong.lib.lang3.text.StrMatcher commaMatcher();
  public static com.feilong.lib.lang3.text.StrMatcher tabMatcher();
  public static com.feilong.lib.lang3.text.StrMatcher spaceMatcher();
  public static com.feilong.lib.lang3.text.StrMatcher splitMatcher();
  public static com.feilong.lib.lang3.text.StrMatcher trimMatcher();
  public static com.feilong.lib.lang3.text.StrMatcher singleQuoteMatcher();
  public static com.feilong.lib.lang3.text.StrMatcher doubleQuoteMatcher();
  public static com.feilong.lib.lang3.text.StrMatcher quoteMatcher();
  public static com.feilong.lib.lang3.text.StrMatcher noneMatcher();
  public static com.feilong.lib.lang3.text.StrMatcher charMatcher(char);
  public static com.feilong.lib.lang3.text.StrMatcher charSetMatcher(char...);
  public static com.feilong.lib.lang3.text.StrMatcher charSetMatcher(java.lang.String);
  public static com.feilong.lib.lang3.text.StrMatcher stringMatcher(java.lang.String);
  public abstract int isMatch(char[], int, int, int);
  public int isMatch(char[], int);
}
```

## `com.feilong.lib.lang3.text.StrSubstitutor`

```java
public class com.feilong.lib.lang3.text.StrSubstitutor {
  public static <V> java.lang.String replace(java.lang.Object, java.util.Map<java.lang.String, V>);
  public static <V> java.lang.String replace(java.lang.Object, java.util.Map<java.lang.String, V>, java.lang.String, java.lang.String);
  public static java.lang.String replace(java.lang.Object, java.util.Properties);
  public com.feilong.lib.lang3.text.StrSubstitutor();
  public <V> com.feilong.lib.lang3.text.StrSubstitutor(java.util.Map<java.lang.String, V>);
  public <V> com.feilong.lib.lang3.text.StrSubstitutor(java.util.Map<java.lang.String, V>, java.lang.String, java.lang.String);
  public <V> com.feilong.lib.lang3.text.StrSubstitutor(java.util.Map<java.lang.String, V>, java.lang.String, java.lang.String, char);
  public <V> com.feilong.lib.lang3.text.StrSubstitutor(java.util.Map<java.lang.String, V>, java.lang.String, java.lang.String, char, java.lang.String);
  public com.feilong.lib.lang3.text.StrSubstitutor(com.feilong.lib.lang3.text.StrLookup<?>);
  public com.feilong.lib.lang3.text.StrSubstitutor(com.feilong.lib.lang3.text.StrLookup<?>, java.lang.String, java.lang.String, char);
  public com.feilong.lib.lang3.text.StrSubstitutor(com.feilong.lib.lang3.text.StrLookup<?>, java.lang.String, java.lang.String, char, java.lang.String);
  public com.feilong.lib.lang3.text.StrSubstitutor(com.feilong.lib.lang3.text.StrLookup<?>, com.feilong.lib.lang3.text.StrMatcher, com.feilong.lib.lang3.text.StrMatcher, char);
  public com.feilong.lib.lang3.text.StrSubstitutor(com.feilong.lib.lang3.text.StrLookup<?>, com.feilong.lib.lang3.text.StrMatcher, com.feilong.lib.lang3.text.StrMatcher, char, com.feilong.lib.lang3.text.StrMatcher);
  public java.lang.String replace(java.lang.String);
  public java.lang.String replace(java.lang.String, int, int);
  public java.lang.String replace(char[]);
  public java.lang.String replace(char[], int, int);
  public java.lang.String replace(java.lang.StringBuffer);
  public java.lang.String replace(java.lang.StringBuffer, int, int);
  public java.lang.String replace(java.lang.CharSequence);
  public java.lang.String replace(java.lang.CharSequence, int, int);
  public java.lang.String replace(com.feilong.lib.lang3.text.StrBuilder);
  public java.lang.String replace(com.feilong.lib.lang3.text.StrBuilder, int, int);
  public java.lang.String replace(java.lang.Object);
  public boolean replaceIn(java.lang.StringBuffer);
  public boolean replaceIn(java.lang.StringBuffer, int, int);
  public boolean replaceIn(java.lang.StringBuilder);
  public boolean replaceIn(java.lang.StringBuilder, int, int);
  public boolean replaceIn(com.feilong.lib.lang3.text.StrBuilder);
  public boolean replaceIn(com.feilong.lib.lang3.text.StrBuilder, int, int);
  public char getEscapeChar();
  public void setEscapeChar(char);
  public com.feilong.lib.lang3.text.StrMatcher getVariablePrefixMatcher();
  public com.feilong.lib.lang3.text.StrSubstitutor setVariablePrefixMatcher(com.feilong.lib.lang3.text.StrMatcher);
  public com.feilong.lib.lang3.text.StrSubstitutor setVariablePrefix(char);
  public com.feilong.lib.lang3.text.StrSubstitutor setVariablePrefix(java.lang.String);
  public com.feilong.lib.lang3.text.StrMatcher getVariableSuffixMatcher();
  public com.feilong.lib.lang3.text.StrSubstitutor setVariableSuffixMatcher(com.feilong.lib.lang3.text.StrMatcher);
  public com.feilong.lib.lang3.text.StrSubstitutor setVariableSuffix(char);
  public com.feilong.lib.lang3.text.StrSubstitutor setVariableSuffix(java.lang.String);
  public com.feilong.lib.lang3.text.StrMatcher getValueDelimiterMatcher();
  public com.feilong.lib.lang3.text.StrSubstitutor setValueDelimiterMatcher(com.feilong.lib.lang3.text.StrMatcher);
  public com.feilong.lib.lang3.text.StrSubstitutor setValueDelimiter(char);
  public com.feilong.lib.lang3.text.StrSubstitutor setValueDelimiter(java.lang.String);
  public com.feilong.lib.lang3.text.StrLookup<?> getVariableResolver();
  public void setVariableResolver(com.feilong.lib.lang3.text.StrLookup<?>);
  public boolean isEnableSubstitutionInVariables();
  public void setEnableSubstitutionInVariables(boolean);
  public boolean isPreserveEscapes();
  public void setPreserveEscapes(boolean);
}
```
