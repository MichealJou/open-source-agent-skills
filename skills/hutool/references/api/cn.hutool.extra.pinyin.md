# cn.hutool.extra.pinyin

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.pinyin.PinyinEngine`

```java
public interface cn.hutool.extra.pinyin.PinyinEngine {
  public abstract java.lang.String getPinyin(char);
  public default java.lang.String getPinyin(char, boolean);
  public abstract java.lang.String getPinyin(java.lang.String, java.lang.String);
  public default java.lang.String getPinyin(java.lang.String, java.lang.String, boolean);
  public default char getFirstLetter(char);
  public default java.lang.String getFirstLetter(java.lang.String, java.lang.String);
}
```

## `cn.hutool.extra.pinyin.PinyinException`

```java
public class cn.hutool.extra.pinyin.PinyinException extends java.lang.RuntimeException {
  public cn.hutool.extra.pinyin.PinyinException(java.lang.Throwable);
  public cn.hutool.extra.pinyin.PinyinException(java.lang.String);
  public cn.hutool.extra.pinyin.PinyinException(java.lang.String, java.lang.Object...);
  public cn.hutool.extra.pinyin.PinyinException(java.lang.String, java.lang.Throwable);
  public cn.hutool.extra.pinyin.PinyinException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.extra.pinyin.PinyinException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.extra.pinyin.PinyinUtil`

```java
public class cn.hutool.extra.pinyin.PinyinUtil {
  public cn.hutool.extra.pinyin.PinyinUtil();
  public static cn.hutool.extra.pinyin.PinyinEngine getEngine();
  public static java.lang.String getPinyin(char);
  public static java.lang.String getPinyin(char, boolean);
  public static java.lang.String getPinyin(java.lang.String);
  public static java.lang.String getPinyin(java.lang.String, boolean);
  public static java.lang.String getPinyin(java.lang.String, java.lang.String);
  public static java.lang.String getPinyin(java.lang.String, java.lang.String, boolean);
  public static char getFirstLetter(char);
  public static java.lang.String getFirstLetter(java.lang.String, java.lang.String);
  public static boolean isChinese(char);
}
```
