# mapstruct 方法用途与选择

核对版本：1.6.3。本文只标明已核对的方法；同名重载的签名、空值与异常以该版本源码为准。

## 映射方法怎么选

项目已有 Mapper/Converter 和配置优先；一次简单赋值直接赋值。需要可复用对象映射时，按项目已有 MapStruct 模式处理；`BeanUtil.copyProperties` 不替代项目既有映射契约。

| 注解或属性 | 中文用途与场景 | 优先级与边界 |
| --- | --- | --- |
| `@Mapper` | 声明由 MapStruct 生成实现的映射器 | 优先复用已有 Mapper 和统一组件配置。 |
| `@Mapping(source, target)` | 将来源属性映射到不同名称的目标属性 | 核对字段类型、ID 精度和兼容性。 |
| `@Mapping(ignore = true)` | 显式排除目标字段 | 敏感字段和更新字段按项目契约处理。 |
| `@MappingTarget` | 更新已有目标对象 | 更新与创建语义不同；检查生成代码和集合处理。 |
| `@BeanMapping(nullValuePropertyMappingStrategy = IGNORE)` | 更新时不以 null 属性覆盖目标 | 不代表能区分未提供和显式 null。 |
| `@Named` / `qualifiedByName` | 选择带名称的自定义映射方法 | 优先复用现有转换；限定符名称需一致。 |
| `@MapperConfig` | 在映射器间共享配置 | 先用项目已有配置，避免平行配置。 |
| `@AfterMapping` / `@BeforeMapping` | 映射前后执行额外处理 | 不应在映射中隐藏业务副作用；核对执行时机。 |

带方法的注解属性见 [MapStruct 公开 API](api/org.mapstruct.md)。`MappingTarget`、`BeforeMapping` 和 `AfterMapping` 是没有自身方法的标记注解，不包含在方法签名索引中；未列出的注解和属性仍需查官方手册和生成代码。
