# cn.hutool.system.oshi

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.system.oshi.CpuInfo`

```java
public class cn.hutool.system.oshi.CpuInfo {
  public cn.hutool.system.oshi.CpuInfo();
  public cn.hutool.system.oshi.CpuInfo(oshi.hardware.CentralProcessor, long);
  public cn.hutool.system.oshi.CpuInfo(java.lang.Integer, double, double, double, double, double, java.lang.String);
  public java.lang.Integer getCpuNum();
  public void setCpuNum(java.lang.Integer);
  public double getToTal();
  public void setToTal(double);
  public double getSys();
  public void setSys(double);
  public double getUser();
  public void setUser(double);
  public double getWait();
  public void setWait(double);
  public double getFree();
  public void setFree(double);
  public java.lang.String getCpuModel();
  public void setCpuModel(java.lang.String);
  public cn.hutool.system.oshi.CpuTicks getTicks();
  public void setTicks(cn.hutool.system.oshi.CpuTicks);
  public double getUsed();
  public java.lang.String toString();
}
```

## `cn.hutool.system.oshi.CpuTicks`

```java
public class cn.hutool.system.oshi.CpuTicks {
  public cn.hutool.system.oshi.CpuTicks(oshi.hardware.CentralProcessor, long);
  public long getIdle();
  public void setIdle(long);
  public long getNice();
  public void setNice(long);
  public long getIrq();
  public void setIrq(long);
  public long getSoftIrq();
  public void setSoftIrq(long);
  public long getSteal();
  public void setSteal(long);
  public long getcSys();
  public void setcSys(long);
  public long getUser();
  public void setUser(long);
  public long getIoWait();
  public void setIoWait(long);
  public long totalCpu();
  public java.lang.String toString();
}
```

## `cn.hutool.system.oshi.OshiUtil`

```java
public class cn.hutool.system.oshi.OshiUtil {
  public cn.hutool.system.oshi.OshiUtil();
  public static oshi.software.os.OperatingSystem getOs();
  public static oshi.software.os.OSProcess getCurrentProcess();
  public static oshi.hardware.HardwareAbstractionLayer getHardware();
  public static oshi.hardware.ComputerSystem getSystem();
  public static oshi.hardware.GlobalMemory getMemory();
  public static oshi.hardware.CentralProcessor getProcessor();
  public static oshi.hardware.Sensors getSensors();
  public static java.util.List<oshi.hardware.HWDiskStore> getDiskStores();
  public static java.util.List<oshi.hardware.NetworkIF> getNetworkIFs();
  public static cn.hutool.system.oshi.CpuInfo getCpuInfo();
  public static cn.hutool.system.oshi.CpuInfo getCpuInfo(long);
}
```
