# org.mapstruct.control

版本：1.6.3。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `org.mapstruct.control.MappingControl`

```java
public interface org.mapstruct.control.MappingControl extends java.lang.annotation.Annotation {
  public abstract org.mapstruct.control.MappingControl$Use value();
}
```

## `org.mapstruct.control.MappingControl$Use`

```java
public final class org.mapstruct.control.MappingControl$Use extends java.lang.Enum<org.mapstruct.control.MappingControl$Use> {
  public static org.mapstruct.control.MappingControl$Use[] values();
  public static org.mapstruct.control.MappingControl$Use valueOf(java.lang.String);
}
```

## `org.mapstruct.control.MappingControls`

```java
public interface org.mapstruct.control.MappingControls extends java.lang.annotation.Annotation {
  public abstract org.mapstruct.control.MappingControl[] value();
}
```
