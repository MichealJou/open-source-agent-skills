# cn.hutool.bloomfilter.filter

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.bloomfilter.filter.AbstractFilter`

```java
public abstract class cn.hutool.bloomfilter.filter.AbstractFilter implements cn.hutool.bloomfilter.BloomFilter {
  public cn.hutool.bloomfilter.filter.AbstractFilter(long, int);
  public cn.hutool.bloomfilter.filter.AbstractFilter(long);
  public void init(long, int);
  public boolean contains(java.lang.String);
  public boolean add(java.lang.String);
  public abstract long hash(java.lang.String);
}
```

## `cn.hutool.bloomfilter.filter.DefaultFilter`

```java
public class cn.hutool.bloomfilter.filter.DefaultFilter extends cn.hutool.bloomfilter.filter.FuncFilter {
  public cn.hutool.bloomfilter.filter.DefaultFilter(long);
  public cn.hutool.bloomfilter.filter.DefaultFilter(long, int);
}
```

## `cn.hutool.bloomfilter.filter.ELFFilter`

```java
public class cn.hutool.bloomfilter.filter.ELFFilter extends cn.hutool.bloomfilter.filter.FuncFilter {
  public cn.hutool.bloomfilter.filter.ELFFilter(long);
  public cn.hutool.bloomfilter.filter.ELFFilter(long, int);
}
```

## `cn.hutool.bloomfilter.filter.FNVFilter`

```java
public class cn.hutool.bloomfilter.filter.FNVFilter extends cn.hutool.bloomfilter.filter.FuncFilter {
  public cn.hutool.bloomfilter.filter.FNVFilter(long);
  public cn.hutool.bloomfilter.filter.FNVFilter(long, int);
}
```

## `cn.hutool.bloomfilter.filter.FuncFilter`

```java
public class cn.hutool.bloomfilter.filter.FuncFilter extends cn.hutool.bloomfilter.filter.AbstractFilter {
  public cn.hutool.bloomfilter.filter.FuncFilter(long, java.util.function.Function<java.lang.String, java.lang.Number>);
  public cn.hutool.bloomfilter.filter.FuncFilter(long, int, java.util.function.Function<java.lang.String, java.lang.Number>);
  public long hash(java.lang.String);
}
```

## `cn.hutool.bloomfilter.filter.HfFilter`

```java
public class cn.hutool.bloomfilter.filter.HfFilter extends cn.hutool.bloomfilter.filter.FuncFilter {
  public cn.hutool.bloomfilter.filter.HfFilter(long);
  public cn.hutool.bloomfilter.filter.HfFilter(long, int);
}
```

## `cn.hutool.bloomfilter.filter.HfIpFilter`

```java
public class cn.hutool.bloomfilter.filter.HfIpFilter extends cn.hutool.bloomfilter.filter.FuncFilter {
  public cn.hutool.bloomfilter.filter.HfIpFilter(long);
  public cn.hutool.bloomfilter.filter.HfIpFilter(long, int);
}
```

## `cn.hutool.bloomfilter.filter.JSFilter`

```java
public class cn.hutool.bloomfilter.filter.JSFilter extends cn.hutool.bloomfilter.filter.FuncFilter {
  public cn.hutool.bloomfilter.filter.JSFilter(long);
  public cn.hutool.bloomfilter.filter.JSFilter(long, int);
}
```

## `cn.hutool.bloomfilter.filter.PJWFilter`

```java
public class cn.hutool.bloomfilter.filter.PJWFilter extends cn.hutool.bloomfilter.filter.FuncFilter {
  public cn.hutool.bloomfilter.filter.PJWFilter(long);
  public cn.hutool.bloomfilter.filter.PJWFilter(long, int);
}
```

## `cn.hutool.bloomfilter.filter.RSFilter`

```java
public class cn.hutool.bloomfilter.filter.RSFilter extends cn.hutool.bloomfilter.filter.FuncFilter {
  public cn.hutool.bloomfilter.filter.RSFilter(long);
  public cn.hutool.bloomfilter.filter.RSFilter(long, int);
}
```

## `cn.hutool.bloomfilter.filter.SDBMFilter`

```java
public class cn.hutool.bloomfilter.filter.SDBMFilter extends cn.hutool.bloomfilter.filter.FuncFilter {
  public cn.hutool.bloomfilter.filter.SDBMFilter(long);
  public cn.hutool.bloomfilter.filter.SDBMFilter(long, int);
}
```

## `cn.hutool.bloomfilter.filter.TianlFilter`

```java
public class cn.hutool.bloomfilter.filter.TianlFilter extends cn.hutool.bloomfilter.filter.FuncFilter {
  public cn.hutool.bloomfilter.filter.TianlFilter(long);
  public cn.hutool.bloomfilter.filter.TianlFilter(long, int);
}
```
