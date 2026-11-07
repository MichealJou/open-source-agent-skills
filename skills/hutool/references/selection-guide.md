# hutool 方法用途与选择

核对版本：5.8.46。本文只标明已核对的方法；同名重载的签名、空值与异常以该版本源码为准。

## 字符串

`StrUtil` 继承 `CharSequenceUtil`。先满足业务语义：通用判空先查 Feilong；需要区分空串和空白时使用下列方法。

| 方法 | 中文用途与场景 | 选择与边界 |
| --- | --- | --- |
| `isEmpty` / `isNotEmpty` | 判断 null 或长度为零 / 其反向；空格必须保留时使用 | 空格不是空串；避免用 Feilong 文本判空替换。 |
| `isBlank` / `isNotBlank` | 判断 null、空串、空白 / 其反向 | Feilong 适用时先用 Feilong；特殊空白语义按版本核对。 |
| `hasBlank` / `isAllBlank` | 多个文本任一为空白 / 全部为空白 | 空参数行为需查具体实现；勿假定与其他库一致。 |
| `hasEmpty` / `isAllEmpty` | 多个文本任一为空串 / 全部为空串 | 空白文本与空串不同。 |
| `nullToEmpty` / `emptyToNull` | 将 null 转空串 / 空串转 null | 改变数据含义；仅在接口契约明确允许时使用。 |
| `nullToDefault` / `emptyToDefault` / `blankToDefault` | 分别在 null、空串、空白时提供默认文本 | 三者触发条件不同，不能混用。 |
| `trim` / `trimToEmpty` / `trimToNull` | 去除边缘空白，并按方法决定空值结果 | 不要擅自清理密码、签名、ID 等协议原值。 |
| `startWith` / `endWith` | 判断文本前缀 / 后缀 | 忽略大小写版本按需求选择；核对 null 行为。 |

## 集合、日期、Bean

| 方法 | 中文用途与场景 | 选择与边界 |
| --- | --- | --- |
| `CollUtil.isEmpty` / `isNotEmpty` | 判断集合为空及反向 | Feilong 已引入且语义符合时先查 Feilong；数据库查询不能因此移到内存。 |
| `CollUtil.join` | 将集合元素按分隔符拼接 | 核对 null 元素、转义及协议格式；复杂序列化使用统一设施。 |
| `DateUtil.format` / `formatDate` / `formatDateTime` | 按指定格式 / 常用日期或日期时间格式输出 | 时间格式、时区和精度以接口约定为准。 |
| `DateUtil.parseDate` / `parseLocalDateTime` | 按对应方法支持的输入解析日期 / 本地日期时间 | 输入格式和时区先核对，不应静默修正接口数据。 |
| `DateUtil.betweenDay` | 计算两个日期之间的天数 | 参数 `true` 在该版本先归一到日开始；核对先后、时区和业务口径。 |
| `BeanUtil.copyProperties` | 属性复制；已有项目模式适合时使用 | Entity/DTO 等优先已有 Mapper；非深拷贝，核对覆盖、null 和嵌套对象。 |

完整重载分别查看 [文本](api/cn.hutool.core.text.md)、[日期](api/cn.hutool.core.date.md)、[集合](api/cn.hutool.core.collection.md) 和 [Bean](api/cn.hutool.core.bean.md) 索引。
