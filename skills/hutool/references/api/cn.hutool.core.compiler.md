# cn.hutool.core.compiler

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.compiler.CompilerException`

```java
public class cn.hutool.core.compiler.CompilerException extends java.lang.RuntimeException {
  public cn.hutool.core.compiler.CompilerException(java.lang.Throwable);
  public cn.hutool.core.compiler.CompilerException(java.lang.String);
  public cn.hutool.core.compiler.CompilerException(java.lang.String, java.lang.Object...);
  public cn.hutool.core.compiler.CompilerException(java.lang.String, java.lang.Throwable);
  public cn.hutool.core.compiler.CompilerException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.core.compiler.CompilerUtil`

```java
public class cn.hutool.core.compiler.CompilerUtil {
  public cn.hutool.core.compiler.CompilerUtil();
  public static boolean compile(java.lang.String...);
  public static javax.tools.StandardJavaFileManager getFileManager();
  public static javax.tools.StandardJavaFileManager getFileManager(javax.tools.DiagnosticListener<? super javax.tools.JavaFileObject>);
  public static javax.tools.JavaCompiler$CompilationTask getTask(javax.tools.JavaFileManager, javax.tools.DiagnosticListener<? super javax.tools.JavaFileObject>, java.lang.Iterable<java.lang.String>, java.lang.Iterable<? extends javax.tools.JavaFileObject>);
  public static cn.hutool.core.compiler.JavaSourceCompiler getCompiler(java.lang.ClassLoader);
}
```

## `cn.hutool.core.compiler.DiagnosticUtil`

```java
public class cn.hutool.core.compiler.DiagnosticUtil {
  public cn.hutool.core.compiler.DiagnosticUtil();
  public static java.lang.String getMessages(javax.tools.DiagnosticCollector<?>);
}
```

## `cn.hutool.core.compiler.JavaFileObjectUtil`

```java
public class cn.hutool.core.compiler.JavaFileObjectUtil {
  public cn.hutool.core.compiler.JavaFileObjectUtil();
  public static java.util.List<javax.tools.JavaFileObject> getJavaFileObjects(java.io.File);
  public static boolean isJarOrZipFile(java.lang.String);
  public static boolean isJavaFile(java.lang.String);
}
```

## `cn.hutool.core.compiler.JavaSourceCompiler`

```java
public class cn.hutool.core.compiler.JavaSourceCompiler {
  public static cn.hutool.core.compiler.JavaSourceCompiler create(java.lang.ClassLoader);
  public cn.hutool.core.compiler.JavaSourceCompiler addSource(cn.hutool.core.io.resource.Resource...);
  public cn.hutool.core.compiler.JavaSourceCompiler addSource(java.io.File...);
  public cn.hutool.core.compiler.JavaSourceCompiler addSource(java.util.Map<java.lang.String, java.lang.String>);
  public cn.hutool.core.compiler.JavaSourceCompiler addSource(java.lang.String, java.lang.String);
  public cn.hutool.core.compiler.JavaSourceCompiler addLibrary(java.io.File...);
  public java.lang.ClassLoader compile();
  public java.lang.ClassLoader compile(java.util.List<java.lang.String>);
}
```
