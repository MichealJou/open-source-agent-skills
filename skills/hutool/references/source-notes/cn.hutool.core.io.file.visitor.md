# cn.hutool.core.io.file.visitor

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.io.file.visitor.CopyVisitor` | `FileVisitResult preVisitDirectory(Path dir,BasicFileAttributes attrs)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.file.visitor.CopyVisitor` | `FileVisitResult visitFile(Path file,BasicFileAttributes attrs)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.file.visitor.DelVisitor` | `FileVisitResult postVisitDirectory(Path dir,IOException e)` | 访问目录结束后删除目录，当执行此方法时，子文件或目录都已访问（删除）完毕 理论上当执行到此方法时，目录下已经被清空了 |
| `cn.hutool.core.io.file.visitor.DelVisitor` | `FileVisitResult visitFile(Path file,BasicFileAttributes attrs)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.file.visitor.MoveVisitor` | `FileVisitResult preVisitDirectory(Path dir,BasicFileAttributes attrs)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.file.visitor.MoveVisitor` | `FileVisitResult visitFile(Path file,BasicFileAttributes attrs)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
