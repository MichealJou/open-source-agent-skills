# 开源库技能

[常用技能与项目启用](常用技能与项目启用.md)提供按任务和项目选择的清单。

每个 `skills/<名称>/` 是可独立安装的技能目录。内容以对应开源项目资料为基础，实际使用时以项目依赖版本、现有规范和用户要求为准。

当前包含 15 个技能：Feilong、Hutool、MyBatis-Plus、Guava、MapStruct、VueUse、Vue 3、Vue Router、Pinia、Android Compose 性能、Android ANR、Sa-Token、Spring 事务、Spring 配置和 Spring 测试。

手动安装时，将所需目录复制到目标工具支持的技能目录；例如 Codex 用户级目录通常为 `~/.codex/skills/`。安装前检查是否同名，避免覆盖已有技能；安装后按客户端要求重新加载或开启新会话。

此目录不包含凭证，不会自动安装依赖、修改代码或连接数据库。

使用时，先选择任务涉及的库并读取对应 `SKILL.md` 的“什么时候用，怎么用”；示例是选型参考，项目依赖版本和项目规范优先。每个技能目录可独立复制。

各技能的 `references/API-INDEX.md` 提供按依赖版本生成的公开 API 签名索引；按包或名称查找，再结合对应官方文档确认用途、参数和边界。索引是声明清单，并非对每个方法的人工作用解释。

工具能力重叠时，先按项目约定和业务语义选择：Feilong 已引入且适用时，判空、判非空、判零及内部断言先查 Feilong；不适用时查 Hutool，再考虑其他已有能力。详细边界分别见 Feilong、Hutool、Guava 技能。

部分技能提供 `references/selection-guide.md` 或 `references/中文指南.md`，用于按场景选择方法；尚未覆盖的内容以该技能的源码、文档及实际依赖版本核对。

新增可独立使用：Vue 3、Vue Router、Pinia、Android Compose 性能、Android ANR 和 Sa-Token。每项保留上游原文、许可证和固定提交；MyBatis-Plus 与 VueUse 另有按需查阅的上游参考。上游建议以当前项目规范及实际版本为准。

另收录 Spring 事务、配置和测试技能，均有独立中文入口和上游许可。

11 个带上游资料的技能已补充 `references/中文指南.md`，并保留指向英文原文的链接。中文指南覆盖核心场景，并非所有方法或上游文件的完整翻译；其余内容继续以对应版本源码和英文原文为准。

## English

Each directory in `skills/` is independently installable. Chinese guides describe selected use cases, method choices and priority rules; upstream reference materials remain available in their original language with license and source details. Project rules and the installed dependency version take precedence. The guides are not yet complete translations or explanations of every public method.

Feilong、Hutool、MyBatis-Plus、Guava、MapStruct 的 `references/source-notes/README.md` 按源码中的公开声明和重载列出注释摘要及许可证；没有中文说明的条目明确标记为待译或无摘要。MapStruct 另有 `references/MapStruct方法中文.md` 逐项说明源码中提取到的公开方法和注解属性。源码摘要不等同逐项校验过的使用场景。
