# cn.hutool.core.bean.copier.provider

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.bean.copier.provider.BeanValueProvider`

```java
public class cn.hutool.core.bean.copier.provider.BeanValueProvider implements cn.hutool.core.bean.copier.ValueProvider<java.lang.String> {
  public cn.hutool.core.bean.copier.provider.BeanValueProvider(java.lang.Object, boolean, boolean);
  public cn.hutool.core.bean.copier.provider.BeanValueProvider(java.lang.Object, boolean, boolean, cn.hutool.core.lang.Editor<java.lang.String>);
  public java.lang.Object value(java.lang.String, java.lang.reflect.Type);
  public boolean containsKey(java.lang.String);
  public boolean containsKey(java.lang.Object);
  public java.lang.Object value(java.lang.Object, java.lang.reflect.Type);
}
```

## `cn.hutool.core.bean.copier.provider.DynaBeanValueProvider`

```java
public class cn.hutool.core.bean.copier.provider.DynaBeanValueProvider implements cn.hutool.core.bean.copier.ValueProvider<java.lang.String> {
  public cn.hutool.core.bean.copier.provider.DynaBeanValueProvider(cn.hutool.core.bean.DynaBean, boolean);
  public java.lang.Object value(java.lang.String, java.lang.reflect.Type);
  public boolean containsKey(java.lang.String);
  public boolean containsKey(java.lang.Object);
  public java.lang.Object value(java.lang.Object, java.lang.reflect.Type);
}
```

## `cn.hutool.core.bean.copier.provider.MapValueProvider`

```java
public class cn.hutool.core.bean.copier.provider.MapValueProvider implements cn.hutool.core.bean.copier.ValueProvider<java.lang.String> {
  public cn.hutool.core.bean.copier.provider.MapValueProvider(java.util.Map);
  public java.lang.Object value(java.lang.String, java.lang.reflect.Type);
  public boolean containsKey(java.lang.String);
  public boolean containsKey(java.lang.Object);
  public java.lang.Object value(java.lang.Object, java.lang.reflect.Type);
}
```
