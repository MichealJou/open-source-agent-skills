# com.feilong.lib.javassist.expr

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.javassist.expr.Cast`

```java
public class com.feilong.lib.javassist.expr.Cast extends com.feilong.lib.javassist.expr.Expr {
  public com.feilong.lib.javassist.CtBehavior where();
  public int getLineNumber();
  public java.lang.String getFileName();
  public com.feilong.lib.javassist.CtClass getType() throws com.feilong.lib.javassist.NotFoundException;
  public com.feilong.lib.javassist.CtClass[] mayThrow();
  public void replace(java.lang.String) throws com.feilong.lib.javassist.CannotCompileException;
}
```

## `com.feilong.lib.javassist.expr.ConstructorCall`

```java
public class com.feilong.lib.javassist.expr.ConstructorCall extends com.feilong.lib.javassist.expr.MethodCall {
  public java.lang.String getMethodName();
  public com.feilong.lib.javassist.CtMethod getMethod() throws com.feilong.lib.javassist.NotFoundException;
  public com.feilong.lib.javassist.CtConstructor getConstructor() throws com.feilong.lib.javassist.NotFoundException;
  public boolean isSuper();
}
```

## `com.feilong.lib.javassist.expr.Expr`

```java
public abstract class com.feilong.lib.javassist.expr.Expr implements com.feilong.lib.javassist.bytecode.Opcode {
  public com.feilong.lib.javassist.CtClass getEnclosingClass();
  public com.feilong.lib.javassist.CtBehavior where();
  public com.feilong.lib.javassist.CtClass[] mayThrow();
  public int indexOfBytecode();
  public int getLineNumber();
  public java.lang.String getFileName();
  public abstract void replace(java.lang.String) throws com.feilong.lib.javassist.CannotCompileException;
  public void replace(java.lang.String, com.feilong.lib.javassist.expr.ExprEditor) throws com.feilong.lib.javassist.CannotCompileException;
}
```

## `com.feilong.lib.javassist.expr.ExprEditor`

```java
public class com.feilong.lib.javassist.expr.ExprEditor {
  public com.feilong.lib.javassist.expr.ExprEditor();
  public boolean doit(com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.bytecode.MethodInfo) throws com.feilong.lib.javassist.CannotCompileException;
  public void edit(com.feilong.lib.javassist.expr.NewExpr) throws com.feilong.lib.javassist.CannotCompileException;
  public void edit(com.feilong.lib.javassist.expr.NewArray) throws com.feilong.lib.javassist.CannotCompileException;
  public void edit(com.feilong.lib.javassist.expr.MethodCall) throws com.feilong.lib.javassist.CannotCompileException;
  public void edit(com.feilong.lib.javassist.expr.ConstructorCall) throws com.feilong.lib.javassist.CannotCompileException;
  public void edit(com.feilong.lib.javassist.expr.FieldAccess) throws com.feilong.lib.javassist.CannotCompileException;
  public void edit(com.feilong.lib.javassist.expr.Instanceof) throws com.feilong.lib.javassist.CannotCompileException;
  public void edit(com.feilong.lib.javassist.expr.Cast) throws com.feilong.lib.javassist.CannotCompileException;
  public void edit(com.feilong.lib.javassist.expr.Handler) throws com.feilong.lib.javassist.CannotCompileException;
}
```

## `com.feilong.lib.javassist.expr.FieldAccess`

```java
public class com.feilong.lib.javassist.expr.FieldAccess extends com.feilong.lib.javassist.expr.Expr {
  public com.feilong.lib.javassist.CtBehavior where();
  public int getLineNumber();
  public java.lang.String getFileName();
  public boolean isStatic();
  public boolean isReader();
  public boolean isWriter();
  public java.lang.String getClassName();
  public java.lang.String getFieldName();
  public com.feilong.lib.javassist.CtField getField() throws com.feilong.lib.javassist.NotFoundException;
  public com.feilong.lib.javassist.CtClass[] mayThrow();
  public java.lang.String getSignature();
  public void replace(java.lang.String) throws com.feilong.lib.javassist.CannotCompileException;
}
```

## `com.feilong.lib.javassist.expr.Handler`

```java
public class com.feilong.lib.javassist.expr.Handler extends com.feilong.lib.javassist.expr.Expr {
  public com.feilong.lib.javassist.CtBehavior where();
  public int getLineNumber();
  public java.lang.String getFileName();
  public com.feilong.lib.javassist.CtClass[] mayThrow();
  public com.feilong.lib.javassist.CtClass getType() throws com.feilong.lib.javassist.NotFoundException;
  public boolean isFinally();
  public void replace(java.lang.String) throws com.feilong.lib.javassist.CannotCompileException;
  public void insertBefore(java.lang.String) throws com.feilong.lib.javassist.CannotCompileException;
}
```

## `com.feilong.lib.javassist.expr.Instanceof`

```java
public class com.feilong.lib.javassist.expr.Instanceof extends com.feilong.lib.javassist.expr.Expr {
  public com.feilong.lib.javassist.CtBehavior where();
  public int getLineNumber();
  public java.lang.String getFileName();
  public com.feilong.lib.javassist.CtClass getType() throws com.feilong.lib.javassist.NotFoundException;
  public com.feilong.lib.javassist.CtClass[] mayThrow();
  public void replace(java.lang.String) throws com.feilong.lib.javassist.CannotCompileException;
}
```

## `com.feilong.lib.javassist.expr.MethodCall`

```java
public class com.feilong.lib.javassist.expr.MethodCall extends com.feilong.lib.javassist.expr.Expr {
  public com.feilong.lib.javassist.CtBehavior where();
  public int getLineNumber();
  public java.lang.String getFileName();
  public java.lang.String getClassName();
  public java.lang.String getMethodName();
  public com.feilong.lib.javassist.CtMethod getMethod() throws com.feilong.lib.javassist.NotFoundException;
  public java.lang.String getSignature();
  public com.feilong.lib.javassist.CtClass[] mayThrow();
  public boolean isSuper();
  public void replace(java.lang.String) throws com.feilong.lib.javassist.CannotCompileException;
}
```

## `com.feilong.lib.javassist.expr.NewArray`

```java
public class com.feilong.lib.javassist.expr.NewArray extends com.feilong.lib.javassist.expr.Expr {
  public com.feilong.lib.javassist.CtBehavior where();
  public int getLineNumber();
  public java.lang.String getFileName();
  public com.feilong.lib.javassist.CtClass[] mayThrow();
  public com.feilong.lib.javassist.CtClass getComponentType() throws com.feilong.lib.javassist.NotFoundException;
  public int getDimension();
  public int getCreatedDimensions();
  public void replace(java.lang.String) throws com.feilong.lib.javassist.CannotCompileException;
}
```

## `com.feilong.lib.javassist.expr.NewExpr`

```java
public class com.feilong.lib.javassist.expr.NewExpr extends com.feilong.lib.javassist.expr.Expr {
  public com.feilong.lib.javassist.CtBehavior where();
  public int getLineNumber();
  public java.lang.String getFileName();
  public java.lang.String getClassName();
  public java.lang.String getSignature();
  public com.feilong.lib.javassist.CtConstructor getConstructor() throws com.feilong.lib.javassist.NotFoundException;
  public com.feilong.lib.javassist.CtClass[] mayThrow();
  public void replace(java.lang.String) throws com.feilong.lib.javassist.CannotCompileException;
}
```
