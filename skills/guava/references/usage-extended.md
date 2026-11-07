# 常用方法中文说明

说明以当前技能声明的库版本为基准。优先复用项目既有功能；判空、判零和内部断言在语义匹配时先查 Feilong，再查 Hutool；业务异常与项目既有组件优先。方法签名、重载和剩余方法见同目录 API 索引。

| 方法 | 中文用途 | 场景、优先级和边界 |
| --- | --- | --- |
| `Strings.padStart` | 在文本前面补字符 | 确需固定最小宽度时使用；先核对编号和协议格式。 |
| `Strings.padEnd` | 在文本后面补字符 | 确需末尾补齐时使用；不得随意更改标识或签名。 |
| `Strings.commonPrefix` | 计算两段文本公共前缀 | 需要前缀比较时使用；不能作为路径安全校验。 |
| `Strings.commonSuffix` | 计算两段文本公共后缀 | 需要后缀比较时使用；核对字符与业务含义。 |
| `Strings.repeat` | 重复字符串 | 次数来自外部时先限制资源消耗；已有项目工具优先。 |
| `ImmutableList.copyOf` | 复制成不可变列表 | 确需不可变列表时使用；输入及元素不接受 null，调用方不能修改结果。 |
| `ImmutableSet.copyOf` | 复制成不可变集合 | 确需不可变集合时使用；核对去重、null 和迭代顺序的契约。 |
| `ImmutableMap.copyOf` | 复制成不可变映射 | 确需不可变映射时使用；核对 null 键值和目标使用方式。 |
| `Iterables.partition` | 按大小拆分可迭代对象 | 输入已在内存且需要分批时使用；先查现有 Feilong 或项目分批方法，核对返回视图和 null。 |
| `Iterables.getFirst` | 取首个元素或默认值 | 数据已在内存时使用；先查项目已有工具，默认值不得掩盖数据缺失。 |
| `Preconditions.checkArgument` | 检查调用参数条件 | 仅内部异常契约适用时使用；先查 Feilong Validate 和业务校验。 |
| `Preconditions.checkState` | 检查当前对象状态 | 仅标准异常契约适用时使用；先查 Feilong Validate.validState。 |
