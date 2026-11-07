# com.baomidou.mybatisplus.core.spi

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.core.spi.CompatibleHelper`

```java
public class com.baomidou.mybatisplus.core.spi.CompatibleHelper {
  public com.baomidou.mybatisplus.core.spi.CompatibleHelper();
  public static boolean hasCompatibleSet();
  public static void setCompatibleSet(com.baomidou.mybatisplus.core.spi.CompatibleSet);
  public static com.baomidou.mybatisplus.core.spi.CompatibleSet getCompatibleSet();
}
```

## `com.baomidou.mybatisplus.core.spi.CompatibleSet`

```java
public interface com.baomidou.mybatisplus.core.spi.CompatibleSet {
  public abstract org.apache.ibatis.session.SqlSession getSqlSession(org.apache.ibatis.session.SqlSessionFactory);
  public abstract void closeSqlSession(org.apache.ibatis.session.SqlSession, org.apache.ibatis.session.SqlSessionFactory);
  public abstract boolean executeBatch(org.apache.ibatis.session.SqlSessionFactory, org.apache.ibatis.logging.Log, java.util.function.Consumer<org.apache.ibatis.session.SqlSession>);
  public default java.io.InputStream getInputStream(java.lang.String) throws java.lang.Exception;
  public default <T> T getBean(java.lang.Class<T>);
  public default java.lang.Object getProxyTargetObject(java.lang.Object);
  public default void setContext(java.lang.Object);
}
```
