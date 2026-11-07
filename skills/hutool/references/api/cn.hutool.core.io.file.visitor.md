# cn.hutool.core.io.file.visitor

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.io.file.visitor.CopyVisitor`

```java
public class cn.hutool.core.io.file.visitor.CopyVisitor extends java.nio.file.SimpleFileVisitor<java.nio.file.Path> {
  public cn.hutool.core.io.file.visitor.CopyVisitor(java.nio.file.Path, java.nio.file.Path, java.nio.file.CopyOption...);
  public java.nio.file.FileVisitResult preVisitDirectory(java.nio.file.Path, java.nio.file.attribute.BasicFileAttributes) throws java.io.IOException;
  public java.nio.file.FileVisitResult visitFile(java.nio.file.Path, java.nio.file.attribute.BasicFileAttributes) throws java.io.IOException;
  public java.nio.file.FileVisitResult visitFile(java.lang.Object, java.nio.file.attribute.BasicFileAttributes) throws java.io.IOException;
  public java.nio.file.FileVisitResult preVisitDirectory(java.lang.Object, java.nio.file.attribute.BasicFileAttributes) throws java.io.IOException;
}
```

## `cn.hutool.core.io.file.visitor.DelVisitor`

```java
public class cn.hutool.core.io.file.visitor.DelVisitor extends java.nio.file.SimpleFileVisitor<java.nio.file.Path> {
  public cn.hutool.core.io.file.visitor.DelVisitor();
  public java.nio.file.FileVisitResult visitFile(java.nio.file.Path, java.nio.file.attribute.BasicFileAttributes) throws java.io.IOException;
  public java.nio.file.FileVisitResult postVisitDirectory(java.nio.file.Path, java.io.IOException) throws java.io.IOException;
  public java.nio.file.FileVisitResult postVisitDirectory(java.lang.Object, java.io.IOException) throws java.io.IOException;
  public java.nio.file.FileVisitResult visitFile(java.lang.Object, java.nio.file.attribute.BasicFileAttributes) throws java.io.IOException;
}
```

## `cn.hutool.core.io.file.visitor.MoveVisitor`

```java
public class cn.hutool.core.io.file.visitor.MoveVisitor extends java.nio.file.SimpleFileVisitor<java.nio.file.Path> {
  public cn.hutool.core.io.file.visitor.MoveVisitor(java.nio.file.Path, java.nio.file.Path, java.nio.file.CopyOption...);
  public java.nio.file.FileVisitResult preVisitDirectory(java.nio.file.Path, java.nio.file.attribute.BasicFileAttributes) throws java.io.IOException;
  public java.nio.file.FileVisitResult visitFile(java.nio.file.Path, java.nio.file.attribute.BasicFileAttributes) throws java.io.IOException;
  public java.nio.file.FileVisitResult visitFile(java.lang.Object, java.nio.file.attribute.BasicFileAttributes) throws java.io.IOException;
  public java.nio.file.FileVisitResult preVisitDirectory(java.lang.Object, java.nio.file.attribute.BasicFileAttributes) throws java.io.IOException;
}
```
