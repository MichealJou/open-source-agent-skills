# com.feilong.context.filecreator

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.context.filecreator.FileCreator`

```java
public interface com.feilong.context.filecreator.FileCreator<T> {
  public abstract java.lang.String create(T);
}
```

## `com.feilong.context.filecreator.RequestFileCreatorDetector`

```java
public interface com.feilong.context.filecreator.RequestFileCreatorDetector {
  public abstract com.feilong.context.filecreator.RequestFileCreator detect(javax.servlet.http.HttpServletRequest);
}
```
