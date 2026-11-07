# cn.hutool.core.text.replacer

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.text.replacer.LookupReplacer`

```java
public class cn.hutool.core.text.replacer.LookupReplacer extends cn.hutool.core.text.replacer.StrReplacer {
  public cn.hutool.core.text.replacer.LookupReplacer(java.lang.String[]...);
}
```

## `cn.hutool.core.text.replacer.ReplacerChain`

```java
public class cn.hutool.core.text.replacer.ReplacerChain extends cn.hutool.core.text.replacer.StrReplacer implements cn.hutool.core.lang.Chain<cn.hutool.core.text.replacer.StrReplacer, cn.hutool.core.text.replacer.ReplacerChain> {
  public cn.hutool.core.text.replacer.ReplacerChain(cn.hutool.core.text.replacer.StrReplacer...);
  public java.util.Iterator<cn.hutool.core.text.replacer.StrReplacer> iterator();
  public cn.hutool.core.text.replacer.ReplacerChain addChain(cn.hutool.core.text.replacer.StrReplacer);
  public java.lang.Object addChain(java.lang.Object);
}
```

## `cn.hutool.core.text.replacer.StrReplacer`

```java
public abstract class cn.hutool.core.text.replacer.StrReplacer implements cn.hutool.core.lang.Replacer<java.lang.CharSequence>, java.io.Serializable {
  public cn.hutool.core.text.replacer.StrReplacer();
  public java.lang.CharSequence replace(java.lang.CharSequence);
  public java.lang.Object replace(java.lang.Object);
}
```
