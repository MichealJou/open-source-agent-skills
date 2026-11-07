# MapStruct 1.6.3 方法与注解属性中文说明

本表逐项列出源码提取到的公开方法和注解属性。属性属于声明所在注解，并非都作为普通 Java 方法调用；完整英文摘要及类型见[源码索引](source-notes/README.md)。

统一选择顺序：项目现有转换器与 `@MapperConfig` 优先；需要改变某次映射时，再在该 Mapper、方法或属性级配置。具体属性层级是否可用以及覆盖顺序以 1.6.3 文档为准。简单赋值不必新增 Mapper。

| 声明类 | 方法或属性 | 中文用途与使用场景 |
| --- | --- | --- |
| `org.mapstruct.AnnotateWith` | `elements` | 指定要生成的注解元素配置；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.AnnotateWith` | `value` | 指定需要加到生成代码上的注解类型；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.AnnotateWith$Element` | `booleans` | 为生成的注解元素提供布尔值；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.AnnotateWith$Element` | `bytes` | 为生成的注解元素提供 byte 值；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.AnnotateWith$Element` | `chars` | 为生成的注解元素提供字符值；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.AnnotateWith$Element` | `classes` | 为生成的注解元素提供类型值；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.AnnotateWith$Element` | `doubles` | 为生成的注解元素提供 double 值；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.AnnotateWith$Element` | `enumClass` | 指定生成的注解元素所用枚举类型；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.AnnotateWith$Element` | `enums` | 指定生成的注解元素所用枚举值；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.AnnotateWith$Element` | `floats` | 为生成的注解元素提供 float 值；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.AnnotateWith$Element` | `ints` | 为生成的注解元素提供 int 值；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.AnnotateWith$Element` | `longs` | 为生成的注解元素提供 long 值；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.AnnotateWith$Element` | `name` | 指定要继承的映射方法名或注解元素名；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.AnnotateWith$Element` | `shorts` | 为生成的注解元素提供 short 值；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.AnnotateWith$Element` | `strings` | 为生成的注解元素提供字符串值；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.AnnotateWiths` | `value` | 列出需要应用的附加注解配置；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.BeanMapping` | `builder` | 配置映射时的构建器行为；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.BeanMapping` | `ignoreByDefault` | 控制是否默认只映射显式声明的属性；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.BeanMapping` | `ignoreUnmappedSourceProperties` | 指定在未映射源属性检查中忽略的属性；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.BeanMapping` | `mappingControl` | 控制允许采用的映射方式；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.BeanMapping` | `nullValueCheckStrategy` | 配置生成代码进行 null 检查的策略；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.BeanMapping` | `nullValueMappingStrategy` | 配置映射方法源参数为 null 时返回结果的策略；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.BeanMapping` | `nullValuePropertyMappingStrategy` | 配置更新映射中源属性为 null 或不存在时的处理；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.BeanMapping` | `qualifiedBy` | 按注解限定候选映射方法；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.BeanMapping` | `qualifiedByName` | 按名称限定候选映射方法；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.BeanMapping` | `resultType` | 限定映射或工厂方法的结果类型；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.BeanMapping` | `subclassExhaustiveStrategy` | 配置子类映射未覆盖时的处理策略；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.BeanMapping` | `unmappedSourcePolicy` | 配置未映射源属性的报告策略；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.BeanMapping` | `unmappedTargetPolicy` | 配置未映射目标属性的报告策略；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Builder` | `buildMethod` | 指定构建器用于完成对象创建的方法名；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Builder` | `disableBuilder` | 控制是否禁用构建器映射；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Condition` | `appliesTo` | 指定条件检查适用的目标范围；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.DecoratedWith` | `value` | 指定装饰器类型；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.EnumMapping` | `configuration` | 提供名称转换策略所需的配置；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.EnumMapping` | `nameTransformationStrategy` | 指定枚举名称转换策略；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.EnumMapping` | `unexpectedValueMappingException` | 配置枚举值无法映射时使用的异常类型；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.InheritConfiguration` | `name` | 指定要继承的映射方法名或注解元素名；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.InheritInverseConfiguration` | `name` | 指定要继承的映射方法名或注解元素名；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.IterableMapping` | `dateFormat` | 指定日期格式转换格式；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.IterableMapping` | `elementMappingControl` | 控制集合元素允许采用的映射方式；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.IterableMapping` | `elementTargetType` | 限定集合元素的目标类型；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.IterableMapping` | `nullValueMappingStrategy` | 配置映射方法源参数为 null 时返回结果的策略；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.IterableMapping` | `numberFormat` | 指定数字格式转换格式；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.IterableMapping` | `qualifiedBy` | 按注解限定候选映射方法；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.IterableMapping` | `qualifiedByName` | 按名称限定候选映射方法；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Javadoc` | `authors` | 为生成的 Javadoc 声明作者；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Javadoc` | `deprecated` | 配置生成的 Javadoc 弃用说明；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Javadoc` | `since` | 配置生成的 Javadoc 版本信息；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Javadoc` | `value` | 指定生成 Javadoc 的主要文本；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapMapping` | `keyDateFormat` | 指定 Map 键的日期格式；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapMapping` | `keyMappingControl` | 控制 Map 键允许采用的映射方式；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapMapping` | `keyNumberFormat` | 指定 Map 键的数字格式；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapMapping` | `keyQualifiedBy` | 按注解限定 Map 键转换方法；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapMapping` | `keyQualifiedByName` | 按名称限定 Map 键转换方法；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapMapping` | `keyTargetType` | 限定 Map 键的目标类型；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapMapping` | `nullValueMappingStrategy` | 配置映射方法源参数为 null 时返回结果的策略；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapMapping` | `valueDateFormat` | 指定 Map 值的日期格式；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapMapping` | `valueMappingControl` | 控制 Map 值允许采用的映射方式；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapMapping` | `valueNumberFormat` | 指定 Map 值的数字格式；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapMapping` | `valueQualifiedBy` | 按注解限定 Map 值转换方法；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapMapping` | `valueQualifiedByName` | 按名称限定 Map 值转换方法；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapMapping` | `valueTargetType` | 限定 Map 值的目标类型；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapper` | `builder` | 配置映射时的构建器行为；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapper` | `collectionMappingStrategy` | 选择集合属性映射和目标访问策略；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapper` | `componentModel` | 指定生成 Mapper 的组件模型；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapper` | `config` | 指定复用的 Mapper 配置类型；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapper` | `disableSubMappingMethodsGeneration` | 控制是否自动生成子映射方法；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapper` | `implementationName` | 配置生成实现类的名称模板；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapper` | `implementationPackage` | 配置生成实现类的包名模板；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapper` | `imports` | 为生成实现中使用的类型添加导入；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapper` | `injectionStrategy` | 配置生成 Mapper 对依赖的注入方式；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapper` | `mappingControl` | 控制允许采用的映射方式；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapper` | `mappingInheritanceStrategy` | 配置映射配置的继承方式；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapper` | `nullValueCheckStrategy` | 配置生成代码进行 null 检查的策略；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapper` | `nullValueIterableMappingStrategy` | 配置可迭代对象映射的源参数为 null 时如何处理；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapper` | `nullValueMapMappingStrategy` | 配置 Map 映射的源参数为 null 时如何处理；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapper` | `nullValueMappingStrategy` | 配置映射方法源参数为 null 时返回结果的策略；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapper` | `nullValuePropertyMappingStrategy` | 配置更新映射中源属性为 null 或不存在时的处理；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapper` | `subclassExhaustiveStrategy` | 配置子类映射未覆盖时的处理策略；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapper` | `suppressTimestampInGenerated` | 控制生成注解中是否包含时间戳；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapper` | `typeConversionPolicy` | 配置可能损失信息的类型转换的报告级别；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapper` | `unexpectedValueMappingException` | 配置枚举值无法映射时使用的异常类型；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapper` | `unmappedSourcePolicy` | 配置未映射源属性的报告策略；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapper` | `unmappedTargetPolicy` | 配置未映射目标属性的报告策略；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapper` | `uses` | 指定可供该 Mapper 或配置使用的其他映射类型；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapperConfig` | `builder` | 配置映射时的构建器行为；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapperConfig` | `collectionMappingStrategy` | 选择集合属性映射和目标访问策略；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapperConfig` | `componentModel` | 指定生成 Mapper 的组件模型；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapperConfig` | `disableSubMappingMethodsGeneration` | 控制是否自动生成子映射方法；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapperConfig` | `implementationName` | 配置生成实现类的名称模板；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapperConfig` | `implementationPackage` | 配置生成实现类的包名模板；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapperConfig` | `imports` | 为生成实现中使用的类型添加导入；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapperConfig` | `injectionStrategy` | 配置生成 Mapper 对依赖的注入方式；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapperConfig` | `mappingControl` | 控制允许采用的映射方式；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapperConfig` | `mappingInheritanceStrategy` | 配置映射配置的继承方式；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapperConfig` | `nullValueCheckStrategy` | 配置生成代码进行 null 检查的策略；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapperConfig` | `nullValueIterableMappingStrategy` | 配置可迭代对象映射的源参数为 null 时如何处理；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapperConfig` | `nullValueMapMappingStrategy` | 配置 Map 映射的源参数为 null 时如何处理；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapperConfig` | `nullValueMappingStrategy` | 配置映射方法源参数为 null 时返回结果的策略；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapperConfig` | `nullValuePropertyMappingStrategy` | 配置更新映射中源属性为 null 或不存在时的处理；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapperConfig` | `subclassExhaustiveStrategy` | 配置子类映射未覆盖时的处理策略；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapperConfig` | `suppressTimestampInGenerated` | 控制生成注解中是否包含时间戳；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapperConfig` | `typeConversionPolicy` | 配置可能损失信息的类型转换的报告级别；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapperConfig` | `unexpectedValueMappingException` | 配置枚举值无法映射时使用的异常类型；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapperConfig` | `unmappedSourcePolicy` | 配置未映射源属性的报告策略；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapperConfig` | `unmappedTargetPolicy` | 配置未映射目标属性的报告策略；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.MapperConfig` | `uses` | 指定可供该 Mapper 或配置使用的其他映射类型；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapping` | `conditionExpression` | 指定控制属性映射是否执行的表达式；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapping` | `conditionQualifiedBy` | 按注解限定可使用的条件判断方法；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapping` | `conditionQualifiedByName` | 按名称限定可使用的条件判断方法；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapping` | `constant` | 为目标属性指定常量值；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapping` | `dateFormat` | 指定日期格式转换格式；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapping` | `defaultExpression` | 在来源为 null 时指定默认表达式；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapping` | `defaultValue` | 在来源为 null 时指定默认值；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapping` | `dependsOn` | 声明目标属性映射的先后依赖；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapping` | `expression` | 指定用于赋值的表达式；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapping` | `ignore` | 控制是否跳过目标属性映射；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapping` | `mappingControl` | 控制允许采用的映射方式；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapping` | `nullValueCheckStrategy` | 配置生成代码进行 null 检查的策略；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapping` | `nullValuePropertyMappingStrategy` | 配置更新映射中源属性为 null 或不存在时的处理；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapping` | `numberFormat` | 指定数字格式转换格式；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapping` | `qualifiedBy` | 按注解限定候选映射方法；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapping` | `qualifiedByName` | 按名称限定候选映射方法；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapping` | `resultType` | 限定映射或工厂方法的结果类型；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapping` | `source` | 指定来源属性、来源类型或来源枚举项；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mapping` | `target` | 指定目标属性、目标类型或目标枚举项；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Mappings` | `value` | 列出 Bean 属性映射配置；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.Named` | `value` | 指定限定名称供映射方法选择；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.SubclassMapping` | `qualifiedBy` | 按注解限定候选映射方法；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.SubclassMapping` | `qualifiedByName` | 按名称限定候选映射方法；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.SubclassMapping` | `source` | 指定来源属性、来源类型或来源枚举项；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.SubclassMapping` | `target` | 指定目标属性、目标类型或目标枚举项；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.SubclassMappings` | `value` | 列出子类映射配置；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.ValueMapping` | `source` | 指定来源属性、来源类型或来源枚举项；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.ValueMapping` | `target` | 指定目标属性、目标类型或目标枚举项；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.ValueMappings` | `value` | 列出枚举值映射配置；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.control.MappingControl` | `value` | 指定允许使用的映射手段；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.control.MappingControls` | `value` | 列出映射控制配置；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.factory.Mappers` | `getMapper` | 获取给定 Mapper 类型的实例；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.factory.Mappers` | `getMapperClass` | 获取给定 Mapper 的生成实现类；仅在该声明支持且项目实际需要时配置。 |
| `org.mapstruct.util.Experimental` | `value` | 提供实验性标记的字符串值；语义以源码为准；仅在该声明支持且项目实际需要时配置。 |
