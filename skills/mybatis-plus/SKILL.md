---
name: mybatis-plus
description: 在 Java 项目使用或审查 MyBatis-Plus 的 Service、条件构造、分页和数据访问。
---

# MyBatis-Plus

先核对项目版本、数据源、已有 Service 和框架封装。优先复用数据所属 Service 与现有查询方法；确认业务筛选、权限、租户和分页语义后再选择 Wrapper 或自定义 SQL。

- 根据项目实际版本核对 `IService`、链式查询、Lambda Wrapper 和分页接口；不要照搬更高版本的 API。
- 过滤、排序和分页应保持业务正确性，避免全量加载后截取、分页后再过滤、N+1 和无界 IN。
- 字段和排序必须有可信映射；不拼接未校验的客户端 SQL。自定义 SQL、跨模块访问和事务遵守所属项目规则。
- 核对更新字段、null、逻辑删除、租户拦截以及批量写入的行为，测试空结果、边界和权限范围。

官方：[持久层接口](https://baomidou.com/guides/data-interface/)、[条件构造器](https://baomidou.com/guides/wrapper/)。

## 什么时候用，怎么用

先查已有 Service 和项目封装；以下以 3.5.16 为核验基线。

| 场景 | 选择 | 注意 |
| --- | --- | --- |
| 按 ID 查询 | 已有 Service 的 `getById(id)` | 依照项目规则处理不存在、权限和租户。 |
| 条件组合 | Service 的 `lambdaQuery()` / Lambda Wrapper | 属性引用避免硬编码字段名；条件值仍需校验。 |
| 分页 | 现有分页封装或 Service 的分页 API | 过滤和排序在数据库内完成，分页参数限制按项目规范。 |
| 多表复杂查询 | 现有 Mapper XML | 先确认现有接口；租户、逻辑删除和参数化不能遗漏。 |

```java
List<User> users = userService.lambdaQuery()
        .eq(User::getStatus, status)
        .list();
```

示例仅适合结果规模有界的场景；`User`、状态及权限条件由实际业务定义。不要全量查询后在内存分页，也不要拼接未校验的排序字段或 SQL。自定义 SQL 与访问层的具体选择以项目规则为准。

## 方法用途与优先级

按场景读取 [方法用途与选择](references/selection-guide.md)，先核对已有项目能力、业务语义和当前依赖版本。未覆盖的方法继续查版本索引、源码与官方文档，不根据名称猜测。

## 查找全部方法

查看本技能的 [公开 API 索引](references/API-INDEX.md)，按包或名称定位方法与重载；调用前再查官方文档和项目实际版本。索引记录声明，不等于逐项解释、使用建议或兼容性保证；注意继承方法与索引范围。
