# com.baomidou.mybatisplus.extension.plugins

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.extension.plugins.MybatisPlusInterceptor`

```java
public class com.baomidou.mybatisplus.extension.plugins.MybatisPlusInterceptor implements org.apache.ibatis.plugin.Interceptor {
  public com.baomidou.mybatisplus.extension.plugins.MybatisPlusInterceptor();
  public java.lang.Object intercept(org.apache.ibatis.plugin.Invocation) throws java.lang.Throwable;
  public java.lang.Object plugin(java.lang.Object);
  public void addInnerInterceptor(com.baomidou.mybatisplus.extension.plugins.inner.InnerInterceptor);
  public java.util.List<com.baomidou.mybatisplus.extension.plugins.inner.InnerInterceptor> getInterceptors();
  public void setProperties(java.util.Properties);
  public java.lang.String toString();
  public void setInterceptors(java.util.List<com.baomidou.mybatisplus.extension.plugins.inner.InnerInterceptor>);
}
```
