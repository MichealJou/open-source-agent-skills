# com.feilong.lib.javassist.convert

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.javassist.convert.TransformReadField`

```java
public class com.feilong.lib.javassist.convert.TransformReadField extends com.feilong.lib.javassist.convert.Transformer {
  public com.feilong.lib.javassist.convert.TransformReadField(com.feilong.lib.javassist.convert.Transformer, com.feilong.lib.javassist.CtField, java.lang.String, java.lang.String);
  public int transform(com.feilong.lib.javassist.CtClass, int, com.feilong.lib.javassist.bytecode.CodeIterator, com.feilong.lib.javassist.bytecode.ConstPool) throws com.feilong.lib.javassist.bytecode.BadBytecode;
}
```

## `com.feilong.lib.javassist.convert.TransformWriteField`

```java
public final class com.feilong.lib.javassist.convert.TransformWriteField extends com.feilong.lib.javassist.convert.TransformReadField {
  public com.feilong.lib.javassist.convert.TransformWriteField(com.feilong.lib.javassist.convert.Transformer, com.feilong.lib.javassist.CtField, java.lang.String, java.lang.String);
  public int transform(com.feilong.lib.javassist.CtClass, int, com.feilong.lib.javassist.bytecode.CodeIterator, com.feilong.lib.javassist.bytecode.ConstPool) throws com.feilong.lib.javassist.bytecode.BadBytecode;
}
```

## `com.feilong.lib.javassist.convert.Transformer`

```java
public abstract class com.feilong.lib.javassist.convert.Transformer implements com.feilong.lib.javassist.bytecode.Opcode {
  public com.feilong.lib.javassist.convert.Transformer(com.feilong.lib.javassist.convert.Transformer);
  public com.feilong.lib.javassist.convert.Transformer getNext();
  public void initialize(com.feilong.lib.javassist.bytecode.ConstPool, com.feilong.lib.javassist.bytecode.CodeAttribute);
  public void initialize(com.feilong.lib.javassist.bytecode.ConstPool, com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.bytecode.MethodInfo) throws com.feilong.lib.javassist.CannotCompileException;
  public void clean();
  public abstract int transform(com.feilong.lib.javassist.CtClass, int, com.feilong.lib.javassist.bytecode.CodeIterator, com.feilong.lib.javassist.bytecode.ConstPool) throws com.feilong.lib.javassist.CannotCompileException, com.feilong.lib.javassist.bytecode.BadBytecode;
  public int extraLocals();
  public int extraStack();
}
```
