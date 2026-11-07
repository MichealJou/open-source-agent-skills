# cn.hutool.system

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.system.HostInfo` | `String getAddress()` | 取得当前主机的地址。 例如： "192.168.0.1" |
| `cn.hutool.system.HostInfo` | `String getName()` | 取得当前主机的名称。 例如： "webserver1" |
| `cn.hutool.system.HostInfo` | `String toString()` | 将当前主机的信息转换成字符串。 |
| `cn.hutool.system.JavaInfo` | `String getVendor()` | 取得当前Java impl.的厂商（取自系统属性：java.vendor）。 例如Sun JDK 1.4.2："Sun Microsystems Inc." |
| `cn.hutool.system.JavaInfo` | `String getVendorURL()` | 取得当前Java impl.的厂商网站的URL（取自系统属性：java.vendor.url）。 例如Sun JDK 1.4.2：" http://java.sun.com/ " |
| `cn.hutool.system.JavaInfo` | `String getVersion()` | 取得当前Java impl.的版本（取自系统属性：java.version）。 例如Sun JDK 1.4.2："1.4.2" |
| `cn.hutool.system.JavaInfo` | `String toString()` | 将Java Implementation的信息转换成字符串。 |
| `cn.hutool.system.JavaInfo` | `boolean isJava10()` | 判断当前Java的版本。 如果不能取得系统属性java.version（因为Java安全限制），则总是返回 false |
| `cn.hutool.system.JavaInfo` | `boolean isJava11()` | 判断当前Java的版本。 如果不能取得系统属性java.version（因为Java安全限制），则总是返回 false |
| `cn.hutool.system.JavaInfo` | `boolean isJava12()` | 判断当前Java的版本。 如果不能取得系统属性java.version（因为Java安全限制），则总是返回 false |
| `cn.hutool.system.JavaInfo` | `boolean isJava13()` | 判断当前Java的版本。 如果不能取得系统属性java.version（因为Java安全限制），则总是返回 false |
| `cn.hutool.system.JavaInfo` | `boolean isJava14()` | 判断当前Java的版本。 如果不能取得系统属性java.version（因为Java安全限制），则总是返回 false |
| `cn.hutool.system.JavaInfo` | `boolean isJava15()` | 判断当前Java的版本。 如果不能取得系统属性java.version（因为Java安全限制），则总是返回 false |
| `cn.hutool.system.JavaInfo` | `boolean isJava16()` | 判断当前Java的版本。 如果不能取得系统属性java.version（因为Java安全限制），则总是返回 false |
| `cn.hutool.system.JavaInfo` | `boolean isJava17()` | 判断当前Java的版本。 如果不能取得系统属性java.version（因为Java安全限制），则总是返回 false |
| `cn.hutool.system.JavaInfo` | `boolean isJava18()` | 判断当前Java的版本。 如果不能取得系统属性java.version（因为Java安全限制），则总是返回 false |
| `cn.hutool.system.JavaInfo` | `boolean isJava1_1()` | 判断当前Java的版本。 如果不能取得系统属性java.version（因为Java安全限制），则总是返回 false |
| `cn.hutool.system.JavaInfo` | `boolean isJava1_2()` | 判断当前Java的版本。 如果不能取得系统属性java.version（因为Java安全限制），则总是返回 false |
| `cn.hutool.system.JavaInfo` | `boolean isJava1_3()` | 判断当前Java的版本。 如果不能取得系统属性java.version（因为Java安全限制），则总是返回 false |
| `cn.hutool.system.JavaInfo` | `boolean isJava1_4()` | 判断当前Java的版本。 如果不能取得系统属性java.version（因为Java安全限制），则总是返回 false |
| `cn.hutool.system.JavaInfo` | `boolean isJava1_5()` | 判断当前Java的版本。 如果不能取得系统属性java.version（因为Java安全限制），则总是返回 false |
| `cn.hutool.system.JavaInfo` | `boolean isJava1_6()` | 判断当前Java的版本。 如果不能取得系统属性java.version（因为Java安全限制），则总是返回 false |
| `cn.hutool.system.JavaInfo` | `boolean isJava1_7()` | 判断当前Java的版本。 如果不能取得系统属性java.version（因为Java安全限制），则总是返回 false |
| `cn.hutool.system.JavaInfo` | `boolean isJava1_8()` | 判断当前Java的版本。 如果不能取得系统属性java.version（因为Java安全限制），则总是返回 false |
| `cn.hutool.system.JavaInfo` | `boolean isJava9()` | 判断当前Java的版本。 如果不能取得系统属性java.version（因为Java安全限制），则总是返回 false |
| `cn.hutool.system.JavaInfo` | `boolean isJavaVersionAtLeast(final float requiredVersion)` | 判定当前Java的版本是否大于等于指定的版本号。 例如： 测试JDK 1.2：isJavaVersionAtLeast(1.2f) 测试JDK 1.2.1：isJavaVersionAtLeast(1.31f) |
| `cn.hutool.system.JavaInfo` | `boolean isJavaVersionAtLeast(final int requiredVersion)` | 判定当前Java的版本是否大于等于指定的版本号。 例如： 测试JDK 1.2：isJavaVersionAtLeast(120) 测试JDK 1.2.1：isJavaVersionAtLeast(131) |
| `cn.hutool.system.JavaInfo` | `float getVersionFloat()` | 取得当前Java impl.的版本（取自系统属性：java.version）。 例如： JDK 1.2：1.2f。 JDK 1.3.1：1.31f |
| `cn.hutool.system.JavaInfo` | `int getVersionInt()` | 取得当前Java impl.的版本（取自系统属性：java.version），java10及其之后的版本返回值为4位。 例如： JDK 1.2：120。 JDK 1.3.1：131 JDK 11.0.2：1102 |
| `cn.hutool.system.JavaRuntimeInfo` | `String getClassPath()` | 取得当前JRE的系统classpath（取自系统属性： java.class.path ）。 例如： "/home/admin/myclasses:/home/admin/..." |
| `cn.hutool.system.JavaRuntimeInfo` | `String getClassVersion()` | 取得当前JRE的class文件格式的版本（取自系统属性： java.class.version ）。 例如Sun JDK 1.4.2： "48.0" |
| `cn.hutool.system.JavaRuntimeInfo` | `String getEndorsedDirs()` | 取得当前JRE的endorsed目录列表（取自系统属性： java.endorsed.dirs ）。 例如Sun JDK 1.4.2： "/opt/jdk1.4.2/jre/lib/endorsed:..." |
| `cn.hutool.system.JavaRuntimeInfo` | `String getExtDirs()` | 取得当前JRE的扩展目录列表（取自系统属性： java.ext.dirs ）。 例如Sun JDK 1.4.2： "/opt/jdk1.4.2/jre/lib/ext:..." |
| `cn.hutool.system.JavaRuntimeInfo` | `String getHomeDir()` | 取得当前JRE的安装目录（取自系统属性： java.home ）。 例如Sun JDK 1.4.2： "/opt/jdk1.4.2/jre" |
| `cn.hutool.system.JavaRuntimeInfo` | `String getLibraryPath()` | 取得当前JRE的library搜索路径（取自系统属性： java.library.path ）。 例如Sun JDK 1.4.2： "/opt/jdk1.4.2/bin:..." |
| `cn.hutool.system.JavaRuntimeInfo` | `String getName()` | 取得当前JRE的名称（取自系统属性： java.runtime.name ）。 例如Sun JDK 1.4.2： "Java(TM) 2 Runtime Environment, Standard Edition" |
| `cn.hutool.system.JavaRuntimeInfo` | `String getProtocolPackages()` | 取得当前JRE的URL协议packages列表（取自系统属性： java.library.path ）。 例如Sun JDK 1.4.2： "sun.net.www.protocol\|..." |
| `cn.hutool.system.JavaRuntimeInfo` | `String getSunArchDataModel()` | 【原文待译】JVM is 32M or 64M |
| `cn.hutool.system.JavaRuntimeInfo` | `String getSunBoothClassPath()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.system.JavaRuntimeInfo` | `String getVersion()` | 取得当前JRE的版本（取自系统属性： java.runtime.version ）。 例如Sun JDK 1.4.2： "1.4.2-b28" |
| `cn.hutool.system.JavaRuntimeInfo` | `String toString()` | 将当前运行的JRE信息转换成字符串。 |
| `cn.hutool.system.JavaRuntimeInfo` | `String[] getClassPathArray()` | 取得当前JRE的系统classpath（取自系统属性： java.class.path ）。 例如： "/home/admin/myclasses:/home/admin/..." |
| `cn.hutool.system.JavaRuntimeInfo` | `String[] getLibraryPathArray()` | 取得当前JRE的library搜索路径（取自系统属性： java.library.path ）。 例如Sun JDK 1.4.2： "/opt/jdk1.4.2/bin:..." |
| `cn.hutool.system.JavaSpecInfo` | `String getName()` | 取得当前Java Spec.的名称（取自系统属性： java.specification.name ）。 例如Sun JDK 1.4.2： "Java Platform API Specification" |
| `cn.hutool.system.JavaSpecInfo` | `String getVendor()` | 取得当前Java Spec.的厂商（取自系统属性： java.specification.vendor ）。 例如Sun JDK 1.4.2： "Sun Microsystems Inc." |
| `cn.hutool.system.JavaSpecInfo` | `String getVersion()` | 取得当前Java Spec.的版本（取自系统属性： java.specification.version ）。 例如Sun JDK 1.4.2： "1.4" |
| `cn.hutool.system.JavaSpecInfo` | `String toString()` | 将Java Specification的信息转换成字符串。 |
| `cn.hutool.system.JvmInfo` | `String getInfo()` | 取得当前JVM impl.的信息（取自系统属性： java.vm.info ）。 例如Sun JDK 1.4.2： "mixed mode" |
| `cn.hutool.system.JvmInfo` | `String getName()` | 取得当前JVM impl.的名称（取自系统属性： java.vm.name ）。 例如Sun JDK 1.4.2： "Java HotSpot(TM) Client VM" |
| `cn.hutool.system.JvmInfo` | `String getVendor()` | 取得当前JVM impl.的厂商（取自系统属性： java.vm.vendor ）。 例如Sun JDK 1.4.2： "Sun Microsystems Inc." |
| `cn.hutool.system.JvmInfo` | `String getVersion()` | 取得当前JVM impl.的版本（取自系统属性： java.vm.version ）。 例如Sun JDK 1.4.2： "1.4.2-b28" |
| `cn.hutool.system.JvmInfo` | `String toString()` | 将Java Virtual Machine Implementation的信息转换成字符串。 |
| `cn.hutool.system.JvmSpecInfo` | `String getName()` | 取得当前JVM spec.的名称（取自系统属性： java.vm.specification.name ）。 例如Sun JDK 1.4.2： "Java Virtual Machine Specification" |
| `cn.hutool.system.JvmSpecInfo` | `String getVendor()` | 取得当前JVM spec.的厂商（取自系统属性： java.vm.specification.vendor ）。 例如Sun JDK 1.4.2： "Sun Microsystems Inc." |
| `cn.hutool.system.JvmSpecInfo` | `String getVersion()` | 取得当前JVM spec.的版本（取自系统属性： java.vm.specification.version ）。 例如Sun JDK 1.4.2： "1.0" |
| `cn.hutool.system.JvmSpecInfo` | `String toString()` | 将Java Virtual Machine Specification的信息转换成字符串。 |
| `cn.hutool.system.OsInfo` | `String getArch()` | 取得当前OS的架构（取自系统属性：os.arch）。 例如："x86" |
| `cn.hutool.system.OsInfo` | `String getFileSeparator()` | 取得OS的文件路径的分隔符（取自系统属性：file.separator）。 例如：Unix为"/"，Windows为"\\"。 |
| `cn.hutool.system.OsInfo` | `String getLineSeparator()` | 取得OS的文本文件换行符（取自系统属性：line.separator）。 例如：Unix为"\n"，Windows为"\r\n"。 |
| `cn.hutool.system.OsInfo` | `String getName()` | 取得当前OS的名称（取自系统属性：os.name）。 例如："Windows XP" |
| `cn.hutool.system.OsInfo` | `String getPathSeparator()` | 取得OS的搜索路径分隔符（取自系统属性：path.separator）。 例如：Unix为":"，Windows为";"。 |
| `cn.hutool.system.OsInfo` | `String getVersion()` | 取得当前OS的版本（取自系统属性：os.version）。 例如："5.1" |
| `cn.hutool.system.OsInfo` | `String toString()` | 将OS的信息转换成字符串。 |
| `cn.hutool.system.OsInfo` | `boolean isAix()` | 判断当前OS的类型。 如果不能取得系统属性os.name（因为Java安全限制），则总是返回false |
| `cn.hutool.system.OsInfo` | `boolean isHpUx()` | 判断当前OS的类型。 如果不能取得系统属性os.name（因为Java安全限制），则总是返回false |
| `cn.hutool.system.OsInfo` | `boolean isIrix()` | 判断当前OS的类型。 如果不能取得系统属性os.name（因为Java安全限制），则总是返回false |
| `cn.hutool.system.OsInfo` | `boolean isLinux()` | 判断当前OS的类型。 如果不能取得系统属性os.name（因为Java安全限制），则总是返回false |
| `cn.hutool.system.OsInfo` | `boolean isMac()` | 判断当前OS的类型。 如果不能取得系统属性os.name（因为Java安全限制），则总是返回false |
| `cn.hutool.system.OsInfo` | `boolean isMacOsX()` | 判断当前OS的类型。 如果不能取得系统属性os.name（因为Java安全限制），则总是返回false |
| `cn.hutool.system.OsInfo` | `boolean isOs2()` | 判断当前OS的类型。 如果不能取得系统属性os.name（因为Java安全限制），则总是返回false |
| `cn.hutool.system.OsInfo` | `boolean isSolaris()` | 判断当前OS的类型。 如果不能取得系统属性os.name（因为Java安全限制），则总是返回false |
| `cn.hutool.system.OsInfo` | `boolean isSunOS()` | 判断当前OS的类型。 如果不能取得系统属性os.name（因为Java安全限制），则总是返回false |
| `cn.hutool.system.OsInfo` | `boolean isWindows()` | 判断当前OS的类型。 如果不能取得系统属性os.name（因为Java安全限制），则总是返回false |
| `cn.hutool.system.OsInfo` | `boolean isWindows10()` | 判断当前OS的类型。 如果不能取得系统属性os.name（因为Java安全限制），则总是返回false |
| `cn.hutool.system.OsInfo` | `boolean isWindows11()` | 判断当前OS的类型。 如果不能取得系统属性os.name（因为Java安全限制），则总是返回false |
| `cn.hutool.system.OsInfo` | `boolean isWindows2000()` | 判断当前OS的类型。 如果不能取得系统属性os.name（因为Java安全限制），则总是返回false |
| `cn.hutool.system.OsInfo` | `boolean isWindows7()` | 判断当前OS的类型。 如果不能取得系统属性os.name（因为Java安全限制），则总是返回false |
| `cn.hutool.system.OsInfo` | `boolean isWindows8()` | 判断当前OS的类型。 如果不能取得系统属性os.name（因为Java安全限制），则总是返回false |
| `cn.hutool.system.OsInfo` | `boolean isWindows8_1()` | 判断当前OS的类型。 如果不能取得系统属性os.name（因为Java安全限制），则总是返回false |
| `cn.hutool.system.OsInfo` | `boolean isWindows95()` | 判断当前OS的类型。 如果不能取得系统属性os.name（因为Java安全限制），则总是返回false |
| `cn.hutool.system.OsInfo` | `boolean isWindows98()` | 判断当前OS的类型。 如果不能取得系统属性os.name（因为Java安全限制），则总是返回false |
| `cn.hutool.system.OsInfo` | `boolean isWindowsME()` | 判断当前OS的类型。 如果不能取得系统属性os.name（因为Java安全限制），则总是返回false |
| `cn.hutool.system.OsInfo` | `boolean isWindowsNT()` | 判断当前OS的类型。 如果不能取得系统属性os.name（因为Java安全限制），则总是返回false |
| `cn.hutool.system.OsInfo` | `boolean isWindowsXP()` | 判断当前OS的类型。 如果不能取得系统属性os.name（因为Java安全限制），则总是返回false |
| `cn.hutool.system.RuntimeInfo` | `Runtime getRuntime()` | 获得运行时对象 |
| `cn.hutool.system.RuntimeInfo` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.system.RuntimeInfo` | `long getFreeMemory()` | 获得JVM已分配内存中的剩余空间 |
| `cn.hutool.system.RuntimeInfo` | `long getMaxMemory()` | 获得JVM最大内存 |
| `cn.hutool.system.RuntimeInfo` | `long getTotalMemory()` | 获得JVM已分配内存 |
| `cn.hutool.system.RuntimeInfo` | `long getUsableMemory()` | 获得JVM最大可用内存 |
| `cn.hutool.system.SystemUtil` | `ClassLoadingMXBean getClassLoadingMXBean()` | 返回Java虚拟机类加载系统相关属性 |
| `cn.hutool.system.SystemUtil` | `CompilationMXBean getCompilationMXBean()` | 返回Java虚拟机编译系统相关属性 如果没有编译系统，则返回null |
| `cn.hutool.system.SystemUtil` | `HostInfo getHostInfo()` | 取得Host的信息。 |
| `cn.hutool.system.SystemUtil` | `JavaInfo getJavaInfo()` | 取得Java Implementation的信息。 |
| `cn.hutool.system.SystemUtil` | `JavaRuntimeInfo getJavaRuntimeInfo()` | 取得当前运行的JRE的信息。 |
| `cn.hutool.system.SystemUtil` | `JavaSpecInfo getJavaSpecInfo()` | 取得Java Specification的信息。 |
| `cn.hutool.system.SystemUtil` | `JvmInfo getJvmInfo()` | 取得Java Virtual Machine Implementation的信息。 |
| `cn.hutool.system.SystemUtil` | `JvmSpecInfo getJvmSpecInfo()` | 取得Java Virtual Machine Specification的信息。 |
| `cn.hutool.system.SystemUtil` | `List<GarbageCollectorMXBean> getGarbageCollectorMXBeans()` | 获取Java虚拟机中的GarbageCollectorMXBean列表 |
| `cn.hutool.system.SystemUtil` | `List<MemoryManagerMXBean> getMemoryManagerMXBeans()` | 获取Java虚拟机中的MemoryManagerMXBean列表 The Java virtual machine can have one or more memory managers. It may add or remove memory managers during execution. |
| `cn.hutool.system.SystemUtil` | `List<MemoryPoolMXBean> getMemoryPoolMXBeans()` | 获取Java虚拟机中的MemoryPoolMXBean列表 The Java virtual machine can have one or more memory pools. It may add or remove memory pools during execution. |
| `cn.hutool.system.SystemUtil` | `MemoryMXBean getMemoryMXBean()` | 返回Java虚拟机内存系统相关属性 |
| `cn.hutool.system.SystemUtil` | `OperatingSystemMXBean getOperatingSystemMXBean()` | 返回Java虚拟机运行下的操作系统相关信息属性 |
| `cn.hutool.system.SystemUtil` | `OsInfo getOsInfo()` | 取得OS的信息。 |
| `cn.hutool.system.SystemUtil` | `RuntimeInfo getRuntimeInfo()` | 取得Runtime的信息。 |
| `cn.hutool.system.SystemUtil` | `RuntimeMXBean getRuntimeMXBean()` | 返回Java虚拟机运行时系统相关属性 |
| `cn.hutool.system.SystemUtil` | `ThreadMXBean getThreadMXBean()` | 返回Java虚拟机线程系统相关属性 |
| `cn.hutool.system.SystemUtil` | `UserInfo getUserInfo()` | 取得User的信息。 |
| `cn.hutool.system.SystemUtil` | `int getTotalThreadCount()` | 获取总线程数 |
| `cn.hutool.system.SystemUtil` | `long getCurrentPID()` | 获取当前进程 PID |
| `cn.hutool.system.SystemUtil` | `long getFreeMemory()` | 获取JVM中内存剩余大小 |
| `cn.hutool.system.SystemUtil` | `long getMaxMemory()` | 获取JVM可用的内存总大小 |
| `cn.hutool.system.SystemUtil` | `long getTotalMemory()` | 获取JVM中内存总大小 |
| `cn.hutool.system.SystemUtil` | `void dumpSystemInfo()` | 将系统信息输出到System#out中。 |
| `cn.hutool.system.SystemUtil` | `void dumpSystemInfo(PrintWriter out)` | 将系统信息输出到指定PrintWriter中。 |
| `cn.hutool.system.UserInfo` | `String getCountry()` | 取得当前登录用户的国家或区域设置（取自系统属性：JDK1.4 user.country或JDK1.2 user.region）。 例如："CN"、"US"等 |
| `cn.hutool.system.UserInfo` | `String getCurrentDir()` | 取得当前目录（取自系统属性：user.dir）。 例如："/home/admin/working/" |
| `cn.hutool.system.UserInfo` | `String getHomeDir()` | 取得当前登录用户的home目录（取自系统属性：user.home）。 例如："/home/admin/" |
| `cn.hutool.system.UserInfo` | `String getLanguage()` | 取得当前登录用户的语言设置（取自系统属性：user.language）。 例如："zh"、"en"等 |
| `cn.hutool.system.UserInfo` | `String getName()` | 取得当前登录用户的名字（取自系统属性：user.name）。 例如："admin" |
| `cn.hutool.system.UserInfo` | `String getTempDir()` | 取得临时目录（取自系统属性：java.io.tmpdir）。 例如："/tmp/" |
| `cn.hutool.system.UserInfo` | `String toString()` | 将当前用户的信息转换成字符串。 |
