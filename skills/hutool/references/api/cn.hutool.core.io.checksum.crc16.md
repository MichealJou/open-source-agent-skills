# cn.hutool.core.io.checksum.crc16

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.io.checksum.crc16.CRC16Ansi`

```java
public class cn.hutool.core.io.checksum.crc16.CRC16Ansi extends cn.hutool.core.io.checksum.crc16.CRC16Checksum {
  public cn.hutool.core.io.checksum.crc16.CRC16Ansi();
  public void reset();
  public void update(int);
}
```

## `cn.hutool.core.io.checksum.crc16.CRC16CCITT`

```java
public class cn.hutool.core.io.checksum.crc16.CRC16CCITT extends cn.hutool.core.io.checksum.crc16.CRC16Checksum {
  public cn.hutool.core.io.checksum.crc16.CRC16CCITT();
  public void update(int);
}
```

## `cn.hutool.core.io.checksum.crc16.CRC16CCITTFalse`

```java
public class cn.hutool.core.io.checksum.crc16.CRC16CCITTFalse extends cn.hutool.core.io.checksum.crc16.CRC16Checksum {
  public cn.hutool.core.io.checksum.crc16.CRC16CCITTFalse();
  public void reset();
  public void update(byte[], int, int);
  public void update(int);
}
```

## `cn.hutool.core.io.checksum.crc16.CRC16Checksum`

```java
public abstract class cn.hutool.core.io.checksum.crc16.CRC16Checksum implements java.util.zip.Checksum,java.io.Serializable {
  public cn.hutool.core.io.checksum.crc16.CRC16Checksum();
  public long getValue();
  public java.lang.String getHexValue();
  public java.lang.String getHexValue(boolean);
  public void reset();
  public void update(byte[]);
  public void update(byte[], int, int);
}
```

## `cn.hutool.core.io.checksum.crc16.CRC16DNP`

```java
public class cn.hutool.core.io.checksum.crc16.CRC16DNP extends cn.hutool.core.io.checksum.crc16.CRC16Checksum {
  public cn.hutool.core.io.checksum.crc16.CRC16DNP();
  public void update(byte[], int, int);
  public void update(int);
}
```

## `cn.hutool.core.io.checksum.crc16.CRC16IBM`

```java
public class cn.hutool.core.io.checksum.crc16.CRC16IBM extends cn.hutool.core.io.checksum.crc16.CRC16Checksum {
  public cn.hutool.core.io.checksum.crc16.CRC16IBM();
  public void update(int);
}
```

## `cn.hutool.core.io.checksum.crc16.CRC16Maxim`

```java
public class cn.hutool.core.io.checksum.crc16.CRC16Maxim extends cn.hutool.core.io.checksum.crc16.CRC16Checksum {
  public cn.hutool.core.io.checksum.crc16.CRC16Maxim();
  public void update(byte[], int, int);
  public void update(int);
}
```

## `cn.hutool.core.io.checksum.crc16.CRC16Modbus`

```java
public class cn.hutool.core.io.checksum.crc16.CRC16Modbus extends cn.hutool.core.io.checksum.crc16.CRC16Checksum {
  public cn.hutool.core.io.checksum.crc16.CRC16Modbus();
  public void reset();
  public void update(int);
}
```

## `cn.hutool.core.io.checksum.crc16.CRC16USB`

```java
public class cn.hutool.core.io.checksum.crc16.CRC16USB extends cn.hutool.core.io.checksum.crc16.CRC16Checksum {
  public cn.hutool.core.io.checksum.crc16.CRC16USB();
  public void reset();
  public void update(byte[], int, int);
  public void update(int);
}
```

## `cn.hutool.core.io.checksum.crc16.CRC16X25`

```java
public class cn.hutool.core.io.checksum.crc16.CRC16X25 extends cn.hutool.core.io.checksum.crc16.CRC16Checksum {
  public cn.hutool.core.io.checksum.crc16.CRC16X25();
  public void reset();
  public void update(byte[], int, int);
  public void update(int);
}
```

## `cn.hutool.core.io.checksum.crc16.CRC16XModem`

```java
public class cn.hutool.core.io.checksum.crc16.CRC16XModem extends cn.hutool.core.io.checksum.crc16.CRC16Checksum {
  public cn.hutool.core.io.checksum.crc16.CRC16XModem();
  public void update(byte[], int, int);
  public void update(int);
}
```
