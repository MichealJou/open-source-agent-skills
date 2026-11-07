# com.feilong.core.lang.annotation

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.core.lang.annotation.AnnotationToStringBuilder`

```java
public interface com.feilong.core.lang.annotation.AnnotationToStringBuilder<T extends java.lang.annotation.Annotation> {
  public abstract java.lang.String build(T);
}
```

## `com.feilong.core.lang.annotation.DefaultAnnotationToStringBuilder`

```java
public class com.feilong.core.lang.annotation.DefaultAnnotationToStringBuilder<T extends java.lang.annotation.Annotation> implements com.feilong.core.lang.annotation.AnnotationToStringBuilder<T> {
  public com.feilong.core.lang.annotation.DefaultAnnotationToStringBuilder();
  public java.lang.String build(T);
  public static final <T extends java.lang.annotation.Annotation> com.feilong.core.lang.annotation.DefaultAnnotationToStringBuilder<T> instance();
}
```
