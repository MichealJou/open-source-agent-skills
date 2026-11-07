# com.baomidou.mybatisplus.extension.service

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.extension.service.IService` | `boolean removeBatchByIds(Collection<?> list)` | 批量删除(jdbc批量提交) |
| `com.baomidou.mybatisplus.extension.service.IService` | `boolean saveBatch(Collection<T> entityList)` | 插入（批量） |
| `com.baomidou.mybatisplus.extension.service.IService` | `boolean saveOrUpdateBatch(Collection<T> entityList)` | 批量修改插入 |
| `com.baomidou.mybatisplus.extension.service.IService` | `boolean updateBatchById(Collection<T> entityList)` | 根据ID 批量更新 |
