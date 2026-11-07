# com.baomidou.mybatisplus.extension.spi

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.extension.spi.CompatibleHelper`

```java
public class com.baomidou.mybatisplus.extension.spi.CompatibleHelper {
  public com.baomidou.mybatisplus.extension.spi.CompatibleHelper();
  public static boolean hasCompatibleSet();
  public static void setCompatibleSet(com.baomidou.mybatisplus.extension.spi.CompatibleSet);
  public static com.baomidou.mybatisplus.extension.spi.CompatibleSet getCompatibleSet();
}
```

## `com.baomidou.mybatisplus.extension.spi.SpringCompatibleSet`

```java
public class com.baomidou.mybatisplus.extension.spi.SpringCompatibleSet implements com.baomidou.mybatisplus.extension.spi.CompatibleSet {
  public com.baomidou.mybatisplus.extension.spi.SpringCompatibleSet();
  public org.apache.ibatis.session.SqlSession getSqlSession(org.apache.ibatis.session.SqlSessionFactory);
  public void closeSqlSession(org.apache.ibatis.session.SqlSession, org.apache.ibatis.session.SqlSessionFactory);
  public boolean executeBatch(org.apache.ibatis.session.SqlSessionFactory, org.apache.ibatis.logging.Log, java.util.function.Consumer<org.apache.ibatis.session.SqlSession>);
  public java.io.InputStream getInputStream(java.lang.String) throws java.lang.Exception;
  public <T> T getBean(java.lang.Class<T>);
  public java.lang.Object getProxyTargetObject(java.lang.Object);
  public void setContext(java.lang.Object);
}
```
