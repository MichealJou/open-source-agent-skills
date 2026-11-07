# cn.hutool.bloomfilter

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.bloomfilter.BitMapBloomFilter`

```java
public class cn.hutool.bloomfilter.BitMapBloomFilter implements cn.hutool.bloomfilter.BloomFilter {
  public cn.hutool.bloomfilter.BitMapBloomFilter(int);
  public cn.hutool.bloomfilter.BitMapBloomFilter(int, cn.hutool.bloomfilter.BloomFilter...);
  public boolean add(java.lang.String);
  public boolean contains(java.lang.String);
}
```

## `cn.hutool.bloomfilter.BitSetBloomFilter`

```java
public class cn.hutool.bloomfilter.BitSetBloomFilter implements cn.hutool.bloomfilter.BloomFilter {
  public cn.hutool.bloomfilter.BitSetBloomFilter(int, int, int);
  public void init(java.lang.String, java.lang.String) throws java.io.IOException;
  public void init(java.lang.String, java.nio.charset.Charset) throws java.io.IOException;
  public boolean add(java.lang.String);
  public boolean contains(java.lang.String);
  public double getFalsePositiveProbability();
  public static int[] createHashes(java.lang.String, int);
  public static int hash(java.lang.String, int);
}
```

## `cn.hutool.bloomfilter.BloomFilter`

```java
public interface cn.hutool.bloomfilter.BloomFilter extends java.io.Serializable {
  public abstract boolean contains(java.lang.String);
  public abstract boolean add(java.lang.String);
}
```

## `cn.hutool.bloomfilter.BloomFilterUtil`

```java
public class cn.hutool.bloomfilter.BloomFilterUtil {
  public cn.hutool.bloomfilter.BloomFilterUtil();
  public static cn.hutool.bloomfilter.BitSetBloomFilter createBitSet(int, int, int);
  public static cn.hutool.bloomfilter.BitMapBloomFilter createBitMap(int);
}
```
