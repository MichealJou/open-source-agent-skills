# com.feilong.lib.javassist.tools

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.javassist.tools.Callback`

```java
public abstract class com.feilong.lib.javassist.tools.Callback {
  public com.feilong.lib.javassist.tools.Callback(java.lang.String);
  public abstract void result(java.lang.Object[]);
  public java.lang.String toString();
  public java.lang.String sourceCode();
  public static void insertBefore(com.feilong.lib.javassist.CtBehavior, com.feilong.lib.javassist.tools.Callback) throws com.feilong.lib.javassist.CannotCompileException;
  public static void insertAfter(com.feilong.lib.javassist.CtBehavior, com.feilong.lib.javassist.tools.Callback) throws com.feilong.lib.javassist.CannotCompileException;
  public static void insertAfter(com.feilong.lib.javassist.CtBehavior, com.feilong.lib.javassist.tools.Callback, boolean) throws com.feilong.lib.javassist.CannotCompileException;
  public static int insertAt(com.feilong.lib.javassist.CtBehavior, com.feilong.lib.javassist.tools.Callback, int) throws com.feilong.lib.javassist.CannotCompileException;
}
```
