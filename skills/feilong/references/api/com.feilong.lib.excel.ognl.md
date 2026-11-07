# com.feilong.lib.excel.ognl

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.excel.ognl.DefaultMemberAccess`

```java
public class com.feilong.lib.excel.ognl.DefaultMemberAccess implements com.feilong.lib.ognl.MemberAccess {
  public com.feilong.lib.excel.ognl.DefaultMemberAccess(boolean);
  public com.feilong.lib.excel.ognl.DefaultMemberAccess(boolean, boolean, boolean);
  public java.lang.Object setup(java.util.Map, java.lang.Object, java.lang.reflect.Member, java.lang.String);
  public void restore(java.util.Map, java.lang.Object, java.lang.reflect.Member, java.lang.String, java.lang.Object);
  public boolean isAccessible(java.util.Map, java.lang.Object, java.lang.reflect.Member, java.lang.String);
}
```

## `com.feilong.lib.excel.ognl.InstantiatingNullHandler`

```java
public class com.feilong.lib.excel.ognl.InstantiatingNullHandler implements com.feilong.lib.ognl.NullHandler {
  public com.feilong.lib.excel.ognl.InstantiatingNullHandler(com.feilong.lib.ognl.NullHandler, java.util.List<java.lang.String>);
  public java.lang.Object nullMethodResult(java.util.Map, java.lang.Object, java.lang.String, java.lang.Object[]);
  public java.lang.Object nullPropertyValue(java.util.Map, java.lang.Object, java.lang.Object);
}
```

## `com.feilong.lib.excel.ognl.OgnlStack`

```java
public class com.feilong.lib.excel.ognl.OgnlStack {
  public com.feilong.lib.excel.ognl.OgnlStack(java.lang.Object);
  public java.lang.Object getValue(java.lang.String);
  public void setValue(java.lang.String, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public void push(java.lang.Object);
  public java.lang.Object pop();
  public java.lang.Object peek();
  public void addContext(java.lang.String, java.lang.Object);
  public void removeContext(java.lang.String);
}
```
