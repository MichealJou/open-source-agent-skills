# cn.hutool.core.compiler

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.compiler.CompilerUtil` | `JavaCompiler.CompilationTask getTask(JavaFileManager fileManager,DiagnosticListener<? super JavaFileObject> diagnosticListener,Iterable<String> options,Iterable<? extends JavaFileObject> compilationUnits)` | 新建编译任务 |
| `cn.hutool.core.compiler.CompilerUtil` | `JavaSourceCompiler getCompiler(ClassLoader parent)` | 获取JavaSourceCompiler |
| `cn.hutool.core.compiler.CompilerUtil` | `StandardJavaFileManager getFileManager()` | 获取StandardJavaFileManager |
| `cn.hutool.core.compiler.CompilerUtil` | `StandardJavaFileManager getFileManager(DiagnosticListener<? super JavaFileObject> diagnosticListener)` | 获取StandardJavaFileManager |
| `cn.hutool.core.compiler.CompilerUtil` | `boolean compile(String... sourceFiles)` | 编译指定的源码文件 |
| `cn.hutool.core.compiler.DiagnosticUtil` | `String getMessages(DiagnosticCollector<?> collector)` | 获取DiagnosticCollector收集到的诊断信息，以文本返回 |
| `cn.hutool.core.compiler.JavaFileObjectUtil` | `List<JavaFileObject> getJavaFileObjects(File file)` | 获取指定文件下的所有待编译的java文件，并以JavaFileObject形式返回 |
| `cn.hutool.core.compiler.JavaFileObjectUtil` | `boolean isJarOrZipFile(String fileName)` | 是否是jar 或 zip 文件 |
| `cn.hutool.core.compiler.JavaFileObjectUtil` | `boolean isJavaFile(String fileName)` | 是否是java文件 |
| `cn.hutool.core.compiler.JavaSourceCompiler` | `ClassLoader compile()` | 编译所有文件并返回类加载器 |
| `cn.hutool.core.compiler.JavaSourceCompiler` | `ClassLoader compile(List<String> options)` | 编译所有文件并返回类加载器 |
| `cn.hutool.core.compiler.JavaSourceCompiler` | `JavaSourceCompiler addLibrary(File... files)` | 加入编译Java源码时所需要的jar包，jar包中必须为字节码 |
| `cn.hutool.core.compiler.JavaSourceCompiler` | `JavaSourceCompiler addSource(File... files)` | 向编译器中加入待编译的文件 支持 .java, 文件夹, 压缩文件 递归搜索文件夹内的压缩文件和jar包 |
| `cn.hutool.core.compiler.JavaSourceCompiler` | `JavaSourceCompiler addSource(Map<String, String> sourceCodeMap)` | 向编译器中加入待编译的源码Map |
| `cn.hutool.core.compiler.JavaSourceCompiler` | `JavaSourceCompiler addSource(Resource... resources)` | 向编译器中加入待编译的资源 支持 .java, 文件夹, 压缩文件 递归搜索文件夹内的压缩文件和jar包 |
| `cn.hutool.core.compiler.JavaSourceCompiler` | `JavaSourceCompiler addSource(String className,String sourceCode)` | 向编译器中加入待编译的源码 |
| `cn.hutool.core.compiler.JavaSourceCompiler` | `JavaSourceCompiler create(ClassLoader parent)` | 创建Java源码编译器 |
