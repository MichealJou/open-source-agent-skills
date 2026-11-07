# com.baomidou.mybatisplus.extension.activerecord

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.extension.activerecord.AbstractModel`

```java
public abstract class com.baomidou.mybatisplus.extension.activerecord.AbstractModel<T extends com.baomidou.mybatisplus.extension.activerecord.AbstractModel<?>> implements java.io.Serializable {
  public com.baomidou.mybatisplus.extension.activerecord.AbstractModel();
  public boolean insert();
  public boolean insertOrUpdate();
  public boolean deleteById(java.io.Serializable);
  public boolean deleteById();
  public boolean delete(com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public boolean updateById();
  public boolean update(com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public java.util.List<T> selectAll();
  public T selectById(java.io.Serializable);
  public T selectById();
  public java.util.List<T> selectList(com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public T selectOne(com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public <E extends com.baomidou.mybatisplus.core.metadata.IPage<T>> E selectPage(E, com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public long selectCount(com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public java.io.Serializable pkVal();
}
```

## `com.baomidou.mybatisplus.extension.activerecord.Model`

```java
public abstract class com.baomidou.mybatisplus.extension.activerecord.Model<T extends com.baomidou.mybatisplus.extension.activerecord.Model<?>> extends com.baomidou.mybatisplus.extension.activerecord.AbstractModel<T> {
  public com.baomidou.mybatisplus.extension.activerecord.Model();
  public com.baomidou.mybatisplus.extension.toolkit.SqlRunner sql();
}
```
