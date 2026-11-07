# com.baomidou.mybatisplus.extension.activerecord

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.extension.activerecord.AbstractModel` | `E selectPage(E page,Wrapper<T> queryWrapper)` | 翻页查询 |
| `com.baomidou.mybatisplus.extension.activerecord.AbstractModel` | `List<T> selectAll()` | 查询所有 |
| `com.baomidou.mybatisplus.extension.activerecord.AbstractModel` | `List<T> selectList(Wrapper<T> queryWrapper)` | 查询总记录数 |
| `com.baomidou.mybatisplus.extension.activerecord.AbstractModel` | `Serializable pkVal()` | 主键值 |
| `com.baomidou.mybatisplus.extension.activerecord.AbstractModel` | `T selectById()` | 根据主键查询 |
| `com.baomidou.mybatisplus.extension.activerecord.AbstractModel` | `T selectById(Serializable id)` | 根据 ID 查询 |
| `com.baomidou.mybatisplus.extension.activerecord.AbstractModel` | `T selectOne(Wrapper<T> queryWrapper)` | 查询一条记录 |
| `com.baomidou.mybatisplus.extension.activerecord.AbstractModel` | `boolean delete(Wrapper<T> queryWrapper)` | 删除记录 |
| `com.baomidou.mybatisplus.extension.activerecord.AbstractModel` | `boolean deleteById()` | 根据主键删除 |
| `com.baomidou.mybatisplus.extension.activerecord.AbstractModel` | `boolean deleteById(Serializable id)` | 根据 ID 删除 |
| `com.baomidou.mybatisplus.extension.activerecord.AbstractModel` | `boolean insert()` | 插入（字段选择插入） |
| `com.baomidou.mybatisplus.extension.activerecord.AbstractModel` | `boolean insertOrUpdate()` | 插入 OR 更新 |
| `com.baomidou.mybatisplus.extension.activerecord.AbstractModel` | `boolean update(Wrapper<T> updateWrapper)` | 执行 SQL 更新 |
| `com.baomidou.mybatisplus.extension.activerecord.AbstractModel` | `boolean updateById()` | 更新（字段选择更新） |
| `com.baomidou.mybatisplus.extension.activerecord.AbstractModel` | `long selectCount(Wrapper<T> queryWrapper)` | 查询总数 |
| `com.baomidou.mybatisplus.extension.activerecord.Model` | `SqlRunner sql()` | 执行 SQL |
