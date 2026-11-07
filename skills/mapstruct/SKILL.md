---
name: mapstruct
description: 使用或审查 MapStruct 对象转换、更新映射与字段兼容性。
---

# MapStruct

先查项目现有 Mapper/Converter、框架默认映射、依赖版本和注解处理器。根据项目已有约定复用映射，不为一次简单赋值新增平行转换器。

- 显式核对字段、枚举、时间、数值精度、嵌套对象及集合；不要将 ID 转为有损类型。
- 对更新映射区分字段未提供、显式 null、清空集合和覆盖现有值；确认项目的 null 处理和字段存在性规则。
- 检查生成代码与 Spring 等依赖注入配置；测试 null、部分更新、边界及自定义映射。

官方：[MapStruct 1.6.3 参考文档](https://mapstruct.org/documentation/stable/reference/html/)。使用前核对实际版本。

## 什么时候用，怎么用

先查项目已有 Mapper、公共配置和注解处理器，以下按 1.6.3 核对。

| 场景 | 选择 | 注意 |
| --- | --- | --- |
| 多处复用的对象转换 | `@Mapper` 声明映射方法 | 核对字段、类型、生成代码和组件注入配置。 |
| 更新已有对象且 null 不覆盖 | `@MappingTarget` 配合 `@BeanMapping` 的 null 策略 | 只改变该映射的 null 属性策略；集合和嵌套对象另查生成代码。 |
| 字段名不同 | `@Mapping(source = "...", target = "...")` | 显式核对数值精度、时间和枚举语义。 |

```java
@Mapper
interface UserMapper {
    @BeanMapping(nullValuePropertyMappingStrategy = NullValuePropertyMappingStrategy.IGNORE)
    void update(UserUpdate source, @MappingTarget User target);
}
```

注解来自 `org.mapstruct`。`IGNORE` 不等于区分“字段未传”和“显式传 null”；如果接口需要这两种不同语义，要有字段存在性信息及项目既有处理方式。不要为一次简单赋值新增映射器。

## 方法用途与优先级

按场景读取 [方法用途与选择](references/selection-guide.md) 和 [常用方法中文说明](references/usage-extended.md)，先核对已有项目能力、业务语义和当前依赖版本。未覆盖的方法继续查版本索引、源码与官方文档，不根据名称猜测。

## 查找全部方法

查看本技能的 [公开 API 索引](references/API-INDEX.md)，按包或名称定位方法与重载；调用前再查官方文档和项目实际版本。索引记录声明，不等于逐项解释、使用建议或兼容性保证；注意继承方法与索引范围。

## 源码方法说明

查看 [固定版本源码说明索引](references/source-notes/README.md) 按类和重载检索上游方法摘要；索引明确标记未翻译与无注释项，具体场景和优先级仍以本技能及项目规范为准。

查看 [MapStruct 公开方法与注解属性中文表](references/MapStruct方法中文.md)，并结合其英文源码说明核对具体声明的默认值和版本。
