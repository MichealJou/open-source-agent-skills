# com.feilong.lib.javassist.bytecode.analysis

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.javassist.bytecode.analysis.Analyzer`

```java
public class com.feilong.lib.javassist.bytecode.analysis.Analyzer implements com.feilong.lib.javassist.bytecode.Opcode {
  public com.feilong.lib.javassist.bytecode.analysis.Analyzer();
  public com.feilong.lib.javassist.bytecode.analysis.Frame[] analyze(com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.bytecode.MethodInfo) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public com.feilong.lib.javassist.bytecode.analysis.Frame[] analyze(com.feilong.lib.javassist.CtMethod) throws com.feilong.lib.javassist.bytecode.BadBytecode;
}
```

## `com.feilong.lib.javassist.bytecode.analysis.ControlFlow`

```java
public class com.feilong.lib.javassist.bytecode.analysis.ControlFlow {
  public com.feilong.lib.javassist.bytecode.analysis.ControlFlow(com.feilong.lib.javassist.CtMethod) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public com.feilong.lib.javassist.bytecode.analysis.ControlFlow(com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.bytecode.MethodInfo) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public com.feilong.lib.javassist.bytecode.analysis.ControlFlow$Block[] basicBlocks();
  public com.feilong.lib.javassist.bytecode.analysis.Frame frameAt(int) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public com.feilong.lib.javassist.bytecode.analysis.ControlFlow$Node[] dominatorTree();
  public com.feilong.lib.javassist.bytecode.analysis.ControlFlow$Node[] postDominatorTree();
}
```

## `com.feilong.lib.javassist.bytecode.analysis.ControlFlow$Block`

```java
public class com.feilong.lib.javassist.bytecode.analysis.ControlFlow$Block extends com.feilong.lib.javassist.bytecode.stackmap.BasicBlock {
  public int index();
  public int position();
  public int length();
  public int incomings();
  public com.feilong.lib.javassist.bytecode.analysis.ControlFlow$Block incoming(int);
  public int exits();
  public com.feilong.lib.javassist.bytecode.analysis.ControlFlow$Block exit(int);
  public com.feilong.lib.javassist.bytecode.analysis.ControlFlow$Catcher[] catchers();
}
```

## `com.feilong.lib.javassist.bytecode.analysis.ControlFlow$Catcher`

```java
public class com.feilong.lib.javassist.bytecode.analysis.ControlFlow$Catcher {
  public com.feilong.lib.javassist.bytecode.analysis.ControlFlow$Block block();
  public java.lang.String type();
}
```

## `com.feilong.lib.javassist.bytecode.analysis.ControlFlow$Node`

```java
public class com.feilong.lib.javassist.bytecode.analysis.ControlFlow$Node {
  public java.lang.String toString();
  public com.feilong.lib.javassist.bytecode.analysis.ControlFlow$Block block();
  public com.feilong.lib.javassist.bytecode.analysis.ControlFlow$Node parent();
  public int children();
  public com.feilong.lib.javassist.bytecode.analysis.ControlFlow$Node child(int);
}
```

## `com.feilong.lib.javassist.bytecode.analysis.Executor`

```java
public class com.feilong.lib.javassist.bytecode.analysis.Executor implements com.feilong.lib.javassist.bytecode.Opcode {
  public com.feilong.lib.javassist.bytecode.analysis.Executor(com.feilong.lib.javassist.ClassPool, com.feilong.lib.javassist.bytecode.ConstPool);
  public void execute(com.feilong.lib.javassist.bytecode.MethodInfo, int, com.feilong.lib.javassist.bytecode.CodeIterator, com.feilong.lib.javassist.bytecode.analysis.Frame, com.feilong.lib.javassist.bytecode.analysis.Subroutine) throws com.feilong.lib.javassist.bytecode.BadBytecode;
}
```

## `com.feilong.lib.javassist.bytecode.analysis.Frame`

```java
public class com.feilong.lib.javassist.bytecode.analysis.Frame {
  public com.feilong.lib.javassist.bytecode.analysis.Frame(int, int);
  public com.feilong.lib.javassist.bytecode.analysis.Type getLocal(int);
  public void setLocal(int, com.feilong.lib.javassist.bytecode.analysis.Type);
  public com.feilong.lib.javassist.bytecode.analysis.Type getStack(int);
  public void setStack(int, com.feilong.lib.javassist.bytecode.analysis.Type);
  public void clearStack();
  public int getTopIndex();
  public int localsLength();
  public com.feilong.lib.javassist.bytecode.analysis.Type peek();
  public com.feilong.lib.javassist.bytecode.analysis.Type pop();
  public void push(com.feilong.lib.javassist.bytecode.analysis.Type);
  public com.feilong.lib.javassist.bytecode.analysis.Frame copy();
  public com.feilong.lib.javassist.bytecode.analysis.Frame copyStack();
  public boolean mergeStack(com.feilong.lib.javassist.bytecode.analysis.Frame);
  public boolean merge(com.feilong.lib.javassist.bytecode.analysis.Frame);
  public java.lang.String toString();
}
```

## `com.feilong.lib.javassist.bytecode.analysis.FramePrinter`

```java
public final class com.feilong.lib.javassist.bytecode.analysis.FramePrinter {
  public com.feilong.lib.javassist.bytecode.analysis.FramePrinter(java.io.PrintStream);
  public static void print(com.feilong.lib.javassist.CtClass, java.io.PrintStream);
  public void print(com.feilong.lib.javassist.CtClass);
  public void print(com.feilong.lib.javassist.CtMethod);
}
```

## `com.feilong.lib.javassist.bytecode.analysis.MultiArrayType`

```java
public class com.feilong.lib.javassist.bytecode.analysis.MultiArrayType extends com.feilong.lib.javassist.bytecode.analysis.Type {
  public com.feilong.lib.javassist.bytecode.analysis.MultiArrayType(com.feilong.lib.javassist.bytecode.analysis.MultiType, int);
  public com.feilong.lib.javassist.CtClass getCtClass();
  public int getDimensions();
  public com.feilong.lib.javassist.bytecode.analysis.Type getComponent();
  public int getSize();
  public boolean isArray();
  public boolean isAssignableFrom(com.feilong.lib.javassist.bytecode.analysis.Type);
  public boolean isReference();
  public boolean isAssignableTo(com.feilong.lib.javassist.bytecode.analysis.Type);
  public int hashCode();
  public boolean equals(java.lang.Object);
  public java.lang.String toString();
}
```

## `com.feilong.lib.javassist.bytecode.analysis.MultiType`

```java
public class com.feilong.lib.javassist.bytecode.analysis.MultiType extends com.feilong.lib.javassist.bytecode.analysis.Type {
  public com.feilong.lib.javassist.bytecode.analysis.MultiType(java.util.Map<java.lang.String, com.feilong.lib.javassist.CtClass>);
  public com.feilong.lib.javassist.bytecode.analysis.MultiType(java.util.Map<java.lang.String, com.feilong.lib.javassist.CtClass>, com.feilong.lib.javassist.bytecode.analysis.Type);
  public com.feilong.lib.javassist.CtClass getCtClass();
  public com.feilong.lib.javassist.bytecode.analysis.Type getComponent();
  public int getSize();
  public boolean isArray();
  public boolean isAssignableFrom(com.feilong.lib.javassist.bytecode.analysis.Type);
  public boolean isAssignableTo(com.feilong.lib.javassist.bytecode.analysis.Type);
  public boolean isReference();
  public com.feilong.lib.javassist.bytecode.analysis.Type merge(com.feilong.lib.javassist.bytecode.analysis.Type);
  public int hashCode();
  public boolean equals(java.lang.Object);
  public java.lang.String toString();
}
```

## `com.feilong.lib.javassist.bytecode.analysis.Subroutine`

```java
public class com.feilong.lib.javassist.bytecode.analysis.Subroutine {
  public com.feilong.lib.javassist.bytecode.analysis.Subroutine(int, int);
  public void addCaller(int);
  public int start();
  public void access(int);
  public boolean isAccessed(int);
  public java.util.Collection<java.lang.Integer> accessed();
  public java.util.Collection<java.lang.Integer> callers();
  public java.lang.String toString();
}
```

## `com.feilong.lib.javassist.bytecode.analysis.SubroutineScanner`

```java
public class com.feilong.lib.javassist.bytecode.analysis.SubroutineScanner implements com.feilong.lib.javassist.bytecode.Opcode {
  public com.feilong.lib.javassist.bytecode.analysis.SubroutineScanner();
  public com.feilong.lib.javassist.bytecode.analysis.Subroutine[] scan(com.feilong.lib.javassist.bytecode.MethodInfo) throws com.feilong.lib.javassist.bytecode.BadBytecode;
}
```

## `com.feilong.lib.javassist.bytecode.analysis.Type`

```java
public class com.feilong.lib.javassist.bytecode.analysis.Type {
  public static com.feilong.lib.javassist.bytecode.analysis.Type get(com.feilong.lib.javassist.CtClass);
  public int getSize();
  public com.feilong.lib.javassist.CtClass getCtClass();
  public boolean isReference();
  public boolean isSpecial();
  public boolean isArray();
  public int getDimensions();
  public com.feilong.lib.javassist.bytecode.analysis.Type getComponent();
  public boolean isAssignableFrom(com.feilong.lib.javassist.bytecode.analysis.Type);
  public com.feilong.lib.javassist.bytecode.analysis.Type merge(com.feilong.lib.javassist.bytecode.analysis.Type);
  public int hashCode();
  public boolean equals(java.lang.Object);
  public java.lang.String toString();
}
```

## `com.feilong.lib.javassist.bytecode.analysis.Util`

```java
public class com.feilong.lib.javassist.bytecode.analysis.Util implements com.feilong.lib.javassist.bytecode.Opcode {
  public com.feilong.lib.javassist.bytecode.analysis.Util();
  public static int getJumpTarget(int, com.feilong.lib.javassist.bytecode.CodeIterator);
  public static boolean isJumpInstruction(int);
  public static boolean isGoto(int);
  public static boolean isJsr(int);
  public static boolean isReturn(int);
}
```
