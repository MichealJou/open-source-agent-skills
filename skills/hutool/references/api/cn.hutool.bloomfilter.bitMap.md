# cn.hutool.bloomfilter.bitMap

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.bloomfilter.bitMap.BitMap`

```java
public interface cn.hutool.bloomfilter.bitMap.BitMap {
  public abstract void add(long);
  public abstract boolean contains(long);
  public abstract void remove(long);
}
```

## `cn.hutool.bloomfilter.bitMap.IntMap`

```java
public class cn.hutool.bloomfilter.bitMap.IntMap implements cn.hutool.bloomfilter.bitMap.BitMap,java.io.Serializable {
  public cn.hutool.bloomfilter.bitMap.IntMap();
  public cn.hutool.bloomfilter.bitMap.IntMap(int);
  public void add(long);
  public boolean contains(long);
  public void remove(long);
}
```

## `cn.hutool.bloomfilter.bitMap.LongMap`

```java
public class cn.hutool.bloomfilter.bitMap.LongMap implements cn.hutool.bloomfilter.bitMap.BitMap,java.io.Serializable {
  public cn.hutool.bloomfilter.bitMap.LongMap();
  public cn.hutool.bloomfilter.bitMap.LongMap(int);
  public void add(long);
  public boolean contains(long);
  public void remove(long);
}
```
