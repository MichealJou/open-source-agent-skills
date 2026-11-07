# cn.hutool.aop.aspects

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.aop.aspects.Aspect`

```java
public interface cn.hutool.aop.aspects.Aspect {
  public abstract boolean before(java.lang.Object, java.lang.reflect.Method, java.lang.Object[]);
  public abstract boolean after(java.lang.Object, java.lang.reflect.Method, java.lang.Object[], java.lang.Object);
  public abstract boolean afterException(java.lang.Object, java.lang.reflect.Method, java.lang.Object[], java.lang.Throwable);
}
```

## `cn.hutool.aop.aspects.SimpleAspect`

```java
public class cn.hutool.aop.aspects.SimpleAspect implements cn.hutool.aop.aspects.Aspect,java.io.Serializable {
  public cn.hutool.aop.aspects.SimpleAspect();
  public boolean before(java.lang.Object, java.lang.reflect.Method, java.lang.Object[]);
  public boolean after(java.lang.Object, java.lang.reflect.Method, java.lang.Object[], java.lang.Object);
  public boolean afterException(java.lang.Object, java.lang.reflect.Method, java.lang.Object[], java.lang.Throwable);
}
```

## `cn.hutool.aop.aspects.TimeIntervalAspect`

```java
public class cn.hutool.aop.aspects.TimeIntervalAspect extends cn.hutool.aop.aspects.SimpleAspect {
  public cn.hutool.aop.aspects.TimeIntervalAspect();
  public boolean before(java.lang.Object, java.lang.reflect.Method, java.lang.Object[]);
  public boolean after(java.lang.Object, java.lang.reflect.Method, java.lang.Object[], java.lang.Object);
}
```
