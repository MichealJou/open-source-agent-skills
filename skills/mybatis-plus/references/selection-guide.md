# mybatis-plus 方法用途与选择

核对版本：3.5.16。本文只标明已核对的方法；同名重载的签名、空值与异常以该版本源码为准。

## 数据访问如何选

先查所属业务 Service、框架封装和现有查询，再考虑 MyBatis-Plus；只有已有能力不能满足时才按项目规则考虑 Mapper XML。业务权限、租户和逻辑删除不可省略。

| 方法或方法族 | 中文用途与场景 | 优先级与边界 |
| --- | --- | --- |
| Service `getById` / Mapper `selectById` | 按主键查询单条 | 优先所属 Service；查不到的处理遵循业务约定。 |
| Service `lambdaQuery` / `LambdaQueryWrapper` | 以属性引用构建条件查询 | 先查现有查询；注意权限和条件为空时的范围。 |
| `eq` / `ne` | 相等 / 不相等条件 | 核对字段类型和 null 语义；动态条件不要拼接 SQL。 |
| `gt` / `ge` / `lt` / `le` | 大于、大于等于、小于、小于等于条件 | 数值精度与日期边界按业务明确。 |
| `in` / `notIn` | 按集合包含 / 排除条件 | 控制集合大小，空集合行为先核对实际版本及业务。 |
| `like` / `likeLeft` / `likeRight` | 模糊匹配 | 核对通配符、匹配方向、索引和输入边界。 |
| Mapper `selectOne` | 查询期望唯一的记录 | 必须保证唯一或明确多条的处理，不要随意截取掩盖脏数据。 |
| Mapper `exists` / `selectCount` | 判断是否存在 / 统计数量 | 有对应 Service 时优先 Service；保持查询条件和权限一致。 |
| Service 分页 / Mapper `selectPage` | 在数据库分页 | 优先项目分页封装；不先取全量再内存截取。 |
| `insert` / `updateById` / `deleteById` | 插入 / 按主键更新 / 删除 | 优先已有 Service；核对事务、更新字段、逻辑删除与影响范围。 |

完整重载见 [BaseMapper](api/com.baomidou.mybatisplus.core.mapper.md) 和条件构造器对应包。SQL 及事务具体规则以项目规范为准。
