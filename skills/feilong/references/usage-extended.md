# 常用方法中文说明

说明以当前技能声明的库版本为基准。优先复用项目既有功能；判空、判零和内部断言在语义匹配时先查 Feilong，再查 Hutool；业务异常与项目既有组件优先。方法签名、重载和剩余方法见同目录 API 索引。

| 方法 | 中文用途 | 场景、优先级和边界 |
| --- | --- | --- |
| `StringUtil.format` | 按模板格式化文本 | 项目需要该版本模板语义时使用；核对占位符和 null，不替换日志框架。 |
| `StringUtil.split` | 拆分文本 | 输出需要按分隔符拆分时使用；核对空文本、连续分隔符与结果类型。 |
| `StringUtil.substring` | 截取字符串 | 项目已有方法适用时使用；先核对下标、负值和越界行为。 |
| `StringUtil.replace` | 替换文本内容 | 核对重载、替换次数及特殊字符；不要修改外部协议原值。 |
| `CollectionsUtil.containsAny` | 判断集合是否含有给定候选元素 | 核对 null、相等性及候选集合为空的行为；不用于替代数据库过滤。 |
| `CollectionsUtil.partition` | 将集合按大小分组 | 确需分批处理时使用；核对批大小、顺序、返回集合和空值。 |
| `CollectionsUtil.getPropertyValueList` | 从对象集合提取指定属性列表 | 已有项目模式适用且属性路径可信时使用；核对反射、null 与输出类型。 |
| `CollectionsUtil.group` | 按条件或属性对集合分组 | 数据已在内存且规模有界时使用；核对键、null 和顺序。 |
| `MapUtil.getOrDefault` | 读取映射值或默认值 | 需默认值时核对键不存在与值为 null 的区别，避免误改业务含义。 |
| `MapUtil.putIfValueNotNull` | 仅在值非 null 时放入映射 | 构建可选字段时使用；明确是否允许 null 和覆盖既有值。 |
