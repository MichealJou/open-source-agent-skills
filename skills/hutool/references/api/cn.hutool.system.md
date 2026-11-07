# cn.hutool.system

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.system.HostInfo`

```java
public class cn.hutool.system.HostInfo implements java.io.Serializable {
  public cn.hutool.system.HostInfo();
  public final java.lang.String getName();
  public final java.lang.String getAddress();
  public final java.lang.String toString();
}
```

## `cn.hutool.system.JavaInfo`

```java
public class cn.hutool.system.JavaInfo implements java.io.Serializable {
  public cn.hutool.system.JavaInfo();
  public final java.lang.String getVersion();
  public final float getVersionFloat();
  public final int getVersionInt();
  public final java.lang.String getVendor();
  public final java.lang.String getVendorURL();
  public final boolean isJava1_1();
  public final boolean isJava1_2();
  public final boolean isJava1_3();
  public final boolean isJava1_4();
  public final boolean isJava1_5();
  public final boolean isJava1_6();
  public final boolean isJava1_7();
  public final boolean isJava1_8();
  public final boolean isJava9();
  public final boolean isJava10();
  public final boolean isJava11();
  public final boolean isJava12();
  public final boolean isJava13();
  public final boolean isJava14();
  public final boolean isJava15();
  public final boolean isJava16();
  public final boolean isJava17();
  public final boolean isJava18();
  public final boolean isJavaVersionAtLeast(float);
  public final boolean isJavaVersionAtLeast(int);
  public final java.lang.String toString();
}
```

## `cn.hutool.system.JavaRuntimeInfo`

```java
public class cn.hutool.system.JavaRuntimeInfo implements java.io.Serializable {
  public cn.hutool.system.JavaRuntimeInfo();
  public final java.lang.String getSunBoothClassPath();
  public final java.lang.String getSunArchDataModel();
  public final java.lang.String getName();
  public final java.lang.String getVersion();
  public final java.lang.String getHomeDir();
  public final java.lang.String getExtDirs();
  public final java.lang.String getEndorsedDirs();
  public final java.lang.String getClassPath();
  public final java.lang.String[] getClassPathArray();
  public final java.lang.String getClassVersion();
  public final java.lang.String getLibraryPath();
  public final java.lang.String[] getLibraryPathArray();
  public final java.lang.String getProtocolPackages();
  public final java.lang.String toString();
}
```

## `cn.hutool.system.JavaSpecInfo`

```java
public class cn.hutool.system.JavaSpecInfo implements java.io.Serializable {
  public cn.hutool.system.JavaSpecInfo();
  public final java.lang.String getName();
  public final java.lang.String getVersion();
  public final java.lang.String getVendor();
  public final java.lang.String toString();
}
```

## `cn.hutool.system.JvmInfo`

```java
public class cn.hutool.system.JvmInfo implements java.io.Serializable {
  public cn.hutool.system.JvmInfo();
  public final java.lang.String getName();
  public final java.lang.String getVersion();
  public final java.lang.String getVendor();
  public final java.lang.String getInfo();
  public final java.lang.String toString();
}
```

## `cn.hutool.system.JvmSpecInfo`

```java
public class cn.hutool.system.JvmSpecInfo implements java.io.Serializable {
  public cn.hutool.system.JvmSpecInfo();
  public final java.lang.String getName();
  public final java.lang.String getVersion();
  public final java.lang.String getVendor();
  public final java.lang.String toString();
}
```

## `cn.hutool.system.OsInfo`

```java
public class cn.hutool.system.OsInfo implements java.io.Serializable {
  public cn.hutool.system.OsInfo();
  public final java.lang.String getArch();
  public final java.lang.String getName();
  public final java.lang.String getVersion();
  public final boolean isAix();
  public final boolean isHpUx();
  public final boolean isIrix();
  public final boolean isLinux();
  public final boolean isMac();
  public final boolean isMacOsX();
  public final boolean isOs2();
  public final boolean isSolaris();
  public final boolean isSunOS();
  public final boolean isWindows();
  public final boolean isWindows2000();
  public final boolean isWindows95();
  public final boolean isWindows98();
  public final boolean isWindowsME();
  public final boolean isWindowsNT();
  public final boolean isWindowsXP();
  public final boolean isWindows7();
  public final boolean isWindows8();
  public final boolean isWindows8_1();
  public final boolean isWindows10();
  public final boolean isWindows11();
  public final java.lang.String getFileSeparator();
  public final java.lang.String getLineSeparator();
  public final java.lang.String getPathSeparator();
  public final java.lang.String toString();
}
```

## `cn.hutool.system.RuntimeInfo`

```java
public class cn.hutool.system.RuntimeInfo implements java.io.Serializable {
  public cn.hutool.system.RuntimeInfo();
  public final java.lang.Runtime getRuntime();
  public final long getMaxMemory();
  public final long getTotalMemory();
  public final long getFreeMemory();
  public final long getUsableMemory();
  public java.lang.String toString();
}
```

## `cn.hutool.system.SystemUtil`

```java
public class cn.hutool.system.SystemUtil extends cn.hutool.core.util.SystemPropsUtil {
  public cn.hutool.system.SystemUtil();
  public static long getCurrentPID();
  public static java.lang.management.ClassLoadingMXBean getClassLoadingMXBean();
  public static java.lang.management.MemoryMXBean getMemoryMXBean();
  public static java.lang.management.ThreadMXBean getThreadMXBean();
  public static java.lang.management.RuntimeMXBean getRuntimeMXBean();
  public static java.lang.management.CompilationMXBean getCompilationMXBean();
  public static java.lang.management.OperatingSystemMXBean getOperatingSystemMXBean();
  public static java.util.List<java.lang.management.MemoryPoolMXBean> getMemoryPoolMXBeans();
  public static java.util.List<java.lang.management.MemoryManagerMXBean> getMemoryManagerMXBeans();
  public static java.util.List<java.lang.management.GarbageCollectorMXBean> getGarbageCollectorMXBeans();
  public static cn.hutool.system.JvmSpecInfo getJvmSpecInfo();
  public static cn.hutool.system.JvmInfo getJvmInfo();
  public static cn.hutool.system.JavaSpecInfo getJavaSpecInfo();
  public static cn.hutool.system.JavaInfo getJavaInfo();
  public static cn.hutool.system.JavaRuntimeInfo getJavaRuntimeInfo();
  public static cn.hutool.system.OsInfo getOsInfo();
  public static cn.hutool.system.UserInfo getUserInfo();
  public static cn.hutool.system.HostInfo getHostInfo();
  public static cn.hutool.system.RuntimeInfo getRuntimeInfo();
  public static long getTotalMemory();
  public static long getFreeMemory();
  public static long getMaxMemory();
  public static int getTotalThreadCount();
  public static void dumpSystemInfo();
  public static void dumpSystemInfo(java.io.PrintWriter);
}
```

## `cn.hutool.system.UserInfo`

```java
public class cn.hutool.system.UserInfo implements java.io.Serializable {
  public cn.hutool.system.UserInfo();
  public final java.lang.String getName();
  public final java.lang.String getHomeDir();
  public final java.lang.String getCurrentDir();
  public final java.lang.String getTempDir();
  public final java.lang.String getLanguage();
  public final java.lang.String getCountry();
  public final java.lang.String toString();
}
```
