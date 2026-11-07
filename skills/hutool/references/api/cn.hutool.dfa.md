# cn.hutool.dfa

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.dfa.FoundWord`

```java
public class cn.hutool.dfa.FoundWord extends cn.hutool.core.lang.DefaultSegment<java.lang.Integer> {
  public cn.hutool.dfa.FoundWord(java.lang.String, java.lang.String, int, int);
  public java.lang.String getWord();
  public java.lang.String getFoundWord();
  public java.lang.String toString();
}
```

## `cn.hutool.dfa.SensitiveProcessor`

```java
public interface cn.hutool.dfa.SensitiveProcessor {
  public default java.lang.String process(cn.hutool.dfa.FoundWord);
}
```

## `cn.hutool.dfa.SensitiveUtil`

```java
public final class cn.hutool.dfa.SensitiveUtil {
  public cn.hutool.dfa.SensitiveUtil();
  public static boolean isInited();
  public static void init(java.util.Collection<java.lang.String>, boolean);
  public static void init(java.util.Collection<java.lang.String>);
  public static void init(java.lang.String, char, boolean);
  public static void init(java.lang.String, boolean);
  public static void setCharFilter(cn.hutool.core.lang.Filter<java.lang.Character>);
  public static boolean containsSensitive(java.lang.String);
  public static boolean containsSensitive(java.lang.Object);
  public static cn.hutool.dfa.FoundWord getFoundFirstSensitive(java.lang.String);
  public static cn.hutool.dfa.FoundWord getFoundFirstSensitive(java.lang.Object);
  public static java.util.List<cn.hutool.dfa.FoundWord> getFoundAllSensitive(java.lang.String);
  public static java.util.List<cn.hutool.dfa.FoundWord> getFoundAllSensitive(java.lang.String, boolean, boolean);
  public static java.util.List<cn.hutool.dfa.FoundWord> getFoundAllSensitive(java.lang.Object);
  public static java.util.List<cn.hutool.dfa.FoundWord> getFoundAllSensitive(java.lang.Object, boolean, boolean);
  public static <T> T sensitiveFilter(T, boolean, cn.hutool.dfa.SensitiveProcessor);
  public static java.lang.String sensitiveFilter(java.lang.String);
  public static java.lang.String sensitiveFilter(java.lang.String, boolean, cn.hutool.dfa.SensitiveProcessor);
}
```

## `cn.hutool.dfa.StopChar`

```java
public class cn.hutool.dfa.StopChar {
  public cn.hutool.dfa.StopChar();
  public static boolean isStopChar(char);
  public static boolean isNotStopChar(char);
}
```

## `cn.hutool.dfa.WordTree`

```java
public class cn.hutool.dfa.WordTree extends java.util.HashMap<java.lang.Character, cn.hutool.dfa.WordTree> {
  public cn.hutool.dfa.WordTree();
  public cn.hutool.dfa.WordTree setCharFilter(cn.hutool.core.lang.Filter<java.lang.Character>);
  public cn.hutool.dfa.WordTree addWords(java.util.Collection<java.lang.String>);
  public cn.hutool.dfa.WordTree addWords(java.lang.String...);
  public cn.hutool.dfa.WordTree addWord(java.lang.String);
  public boolean isMatch(java.lang.String);
  public java.lang.String match(java.lang.String);
  public cn.hutool.dfa.FoundWord matchWord(java.lang.String);
  public java.util.List<java.lang.String> matchAll(java.lang.String);
  public java.util.List<cn.hutool.dfa.FoundWord> matchAllWords(java.lang.String);
  public java.util.List<java.lang.String> matchAll(java.lang.String, int);
  public java.util.List<cn.hutool.dfa.FoundWord> matchAllWords(java.lang.String, int);
  public java.util.List<java.lang.String> matchAll(java.lang.String, int, boolean, boolean);
  public java.util.List<cn.hutool.dfa.FoundWord> matchAllWords(java.lang.String, int, boolean, boolean);
  public void clear();
}
```
