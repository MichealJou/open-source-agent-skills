# com.baomidou.mybatisplus.extension.service

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.extension.service.IService`

```java
public interface com.baomidou.mybatisplus.extension.service.IService<T> extends com.baomidou.mybatisplus.extension.repository.IRepository<T> {
  public default boolean saveBatch(java.util.Collection<T>);
  public default boolean saveOrUpdateBatch(java.util.Collection<T>);
  public default boolean removeBatchByIds(java.util.Collection<?>);
  public default boolean updateBatchById(java.util.Collection<T>);
}
```
