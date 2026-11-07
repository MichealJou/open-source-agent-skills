# cn.hutool.core.io.checksum

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.io.checksum.CRC16`

```java
public class cn.hutool.core.io.checksum.CRC16 implements java.util.zip.Checksum,java.io.Serializable {
  public cn.hutool.core.io.checksum.CRC16();
  public cn.hutool.core.io.checksum.CRC16(cn.hutool.core.io.checksum.crc16.CRC16Checksum);
  public java.lang.String getHexValue();
  public java.lang.String getHexValue(boolean);
  public long getValue();
  public void reset();
  public void update(byte[], int, int);
  public void update(int);
}
```

## `cn.hutool.core.io.checksum.CRC8`

```java
public class cn.hutool.core.io.checksum.CRC8 implements java.util.zip.Checksum,java.io.Serializable {
  public cn.hutool.core.io.checksum.CRC8(int, short);
  public void update(byte[], int, int);
  public void update(byte[]);
  public void update(int);
  public long getValue();
  public void reset();
}
```
