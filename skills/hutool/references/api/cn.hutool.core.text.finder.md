# cn.hutool.core.text.finder

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.text.finder.CharFinder`

```java
public class cn.hutool.core.text.finder.CharFinder extends cn.hutool.core.text.finder.TextFinder {
  public cn.hutool.core.text.finder.CharFinder(char);
  public cn.hutool.core.text.finder.CharFinder(char, boolean);
  public int start(int);
  public int end(int);
}
```

## `cn.hutool.core.text.finder.CharMatcherFinder`

```java
public class cn.hutool.core.text.finder.CharMatcherFinder extends cn.hutool.core.text.finder.TextFinder {
  public cn.hutool.core.text.finder.CharMatcherFinder(cn.hutool.core.lang.Matcher<java.lang.Character>);
  public int start(int);
  public int end(int);
}
```

## `cn.hutool.core.text.finder.Finder`

```java
public interface cn.hutool.core.text.finder.Finder {
  public abstract int start(int);
  public abstract int end(int);
  public default cn.hutool.core.text.finder.Finder reset();
}
```

## `cn.hutool.core.text.finder.LengthFinder`

```java
public class cn.hutool.core.text.finder.LengthFinder extends cn.hutool.core.text.finder.TextFinder {
  public cn.hutool.core.text.finder.LengthFinder(int);
  public int start(int);
  public int end(int);
}
```

## `cn.hutool.core.text.finder.PatternFinder`

```java
public class cn.hutool.core.text.finder.PatternFinder extends cn.hutool.core.text.finder.TextFinder {
  public cn.hutool.core.text.finder.PatternFinder(java.lang.String, boolean);
  public cn.hutool.core.text.finder.PatternFinder(java.util.regex.Pattern);
  public cn.hutool.core.text.finder.TextFinder setText(java.lang.CharSequence);
  public cn.hutool.core.text.finder.TextFinder setNegative(boolean);
  public int start(int);
  public int end(int);
  public cn.hutool.core.text.finder.PatternFinder reset();
  public cn.hutool.core.text.finder.Finder reset();
}
```

## `cn.hutool.core.text.finder.StrFinder`

```java
public class cn.hutool.core.text.finder.StrFinder extends cn.hutool.core.text.finder.TextFinder {
  public cn.hutool.core.text.finder.StrFinder(java.lang.CharSequence, boolean);
  public int start(int);
  public int end(int);
}
```

## `cn.hutool.core.text.finder.TextFinder`

```java
public abstract class cn.hutool.core.text.finder.TextFinder implements cn.hutool.core.text.finder.Finder,java.io.Serializable {
  public cn.hutool.core.text.finder.TextFinder();
  public cn.hutool.core.text.finder.TextFinder setText(java.lang.CharSequence);
  public cn.hutool.core.text.finder.TextFinder setEndIndex(int);
  public cn.hutool.core.text.finder.TextFinder setNegative(boolean);
}
```
