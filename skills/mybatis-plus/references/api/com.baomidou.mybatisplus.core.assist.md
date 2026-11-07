# com.baomidou.mybatisplus.core.assist

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.core.assist.AbstractSqlRunner`

```java
public abstract class com.baomidou.mybatisplus.core.assist.AbstractSqlRunner implements com.baomidou.mybatisplus.core.assist.ISqlRunner {
  public com.baomidou.mybatisplus.core.assist.AbstractSqlRunner();
}
```

## `com.baomidou.mybatisplus.core.assist.ISqlRunner`

```java
public interface com.baomidou.mybatisplus.core.assist.ISqlRunner {
  public abstract boolean insert(java.lang.String, java.lang.Object...);
  public abstract boolean delete(java.lang.String, java.lang.Object...);
  public abstract boolean update(java.lang.String, java.lang.Object...);
  public abstract java.util.List<java.util.Map<java.lang.String, java.lang.Object>> selectList(java.lang.String, java.lang.Object...);
  public abstract java.util.List<java.lang.Object> selectObjs(java.lang.String, java.lang.Object...);
  public abstract java.lang.Object selectObj(java.lang.String, java.lang.Object...);
  public abstract long selectCount(java.lang.String, java.lang.Object...);
  public abstract java.util.Map<java.lang.String, java.lang.Object> selectOne(java.lang.String, java.lang.Object...);
  public abstract <E extends com.baomidou.mybatisplus.core.metadata.IPage<java.util.Map<java.lang.String, java.lang.Object>>> E selectPage(E, java.lang.String, java.lang.Object...);
}
```
