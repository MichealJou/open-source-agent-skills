# cn.hutool.core.lang.copier

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.lang.copier.Copier`

```java
public interface cn.hutool.core.lang.copier.Copier<T> {
  public abstract T copy();
}
```

## `cn.hutool.core.lang.copier.SrcToDestCopier`

```java
public abstract class cn.hutool.core.lang.copier.SrcToDestCopier<T, C extends cn.hutool.core.lang.copier.SrcToDestCopier<T, C>> implements cn.hutool.core.lang.copier.Copier<T>, java.io.Serializable {
  public cn.hutool.core.lang.copier.SrcToDestCopier();
  public T getSrc();
  public C setSrc(T);
  public T getDest();
  public C setDest(T);
  public cn.hutool.core.lang.Filter<T> getCopyFilter();
  public C setCopyFilter(cn.hutool.core.lang.Filter<T>);
}
```
