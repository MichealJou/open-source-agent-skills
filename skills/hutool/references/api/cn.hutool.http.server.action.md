# cn.hutool.http.server.action

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.http.server.action.Action`

```java
public interface cn.hutool.http.server.action.Action {
  public abstract void doAction(cn.hutool.http.server.HttpServerRequest, cn.hutool.http.server.HttpServerResponse) throws java.io.IOException;
}
```

## `cn.hutool.http.server.action.RootAction`

```java
public class cn.hutool.http.server.action.RootAction implements cn.hutool.http.server.action.Action {
  public cn.hutool.http.server.action.RootAction(java.lang.String);
  public cn.hutool.http.server.action.RootAction(java.io.File);
  public cn.hutool.http.server.action.RootAction(java.lang.String, java.lang.String...);
  public cn.hutool.http.server.action.RootAction(java.io.File, java.lang.String...);
  public void doAction(cn.hutool.http.server.HttpServerRequest, cn.hutool.http.server.HttpServerResponse);
}
```
