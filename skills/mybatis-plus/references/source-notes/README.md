# 固定版本方法源码说明索引

来源：[https://github.com/baomidou/mybatis-plus](https://github.com/baomidou/mybatis-plus)，Maven 源码版本 `3.5.16`；许可：Apache-2.0，见 [LICENSE](LICENSE)。这里仅对公开类中的公开方法提取源码签名和文档摘要；不包含构造器、继承展开、非公开类或内嵌第三方包。

共 1544 条方法声明；833 条摘要包含中文，75 条只有非中文摘要，其余无摘要。标记“待译”或“无源码摘要”的方法尚未完成中文说明。部分注释可能过时或省略边界，使用前核对该版本源码及调用契约。

本索引是可检索的源码参考，不自动赋予优先级。先查本技能中文选择指南和项目规范：复用已有实现；判空在语义符合且已引入时先查 Feilong，再查 Hutool；数据库和对象转换沿用现有 Service、Mapper 与权限规则。安全、网络和序列化沿用项目统一链路。

- [com.baomidou.mybatisplus.annotation](com.baomidou.mybatisplus.annotation.md)：41 个方法声明
- [com.baomidou.mybatisplus.autoconfigure](com.baomidou.mybatisplus.autoconfigure.md)：24 个方法声明
- [com.baomidou.mybatisplus.core](com.baomidou.mybatisplus.core.md)：61 个方法声明
- [com.baomidou.mybatisplus.core.assist](com.baomidou.mybatisplus.core.assist.md)：9 个方法声明
- [com.baomidou.mybatisplus.core.batch](com.baomidou.mybatisplus.core.batch.md)：30 个方法声明
- [com.baomidou.mybatisplus.core.conditions](com.baomidou.mybatisplus.core.conditions.md)：96 个方法声明
- [com.baomidou.mybatisplus.core.conditions.interfaces](com.baomidou.mybatisplus.core.conditions.interfaces.md)：111 个方法声明
- [com.baomidou.mybatisplus.core.conditions.query](com.baomidou.mybatisplus.core.conditions.query.md)：19 个方法声明
- [com.baomidou.mybatisplus.core.conditions.segments](com.baomidou.mybatisplus.core.conditions.segments.md)：8 个方法声明
- [com.baomidou.mybatisplus.core.conditions.update](com.baomidou.mybatisplus.core.conditions.update.md)：25 个方法声明
- [com.baomidou.mybatisplus.core.enums](com.baomidou.mybatisplus.core.enums.md)：5 个方法声明
- [com.baomidou.mybatisplus.core.handlers](com.baomidou.mybatisplus.core.handlers.md)：43 个方法声明
- [com.baomidou.mybatisplus.core.incrementer](com.baomidou.mybatisplus.core.incrementer.md)：11 个方法声明
- [com.baomidou.mybatisplus.core.injector](com.baomidou.mybatisplus.core.injector.md)：9 个方法声明
- [com.baomidou.mybatisplus.core.injector.methods](com.baomidou.mybatisplus.core.injector.methods.md)：18 个方法声明
- [com.baomidou.mybatisplus.core.mapper](com.baomidou.mybatisplus.core.mapper.md)：44 个方法声明
- [com.baomidou.mybatisplus.core.metadata](com.baomidou.mybatisplus.core.metadata.md)：74 个方法声明
- [com.baomidou.mybatisplus.core.override](com.baomidou.mybatisplus.core.override.md)：5 个方法声明
- [com.baomidou.mybatisplus.core.plugins](com.baomidou.mybatisplus.core.plugins.md)：16 个方法声明
- [com.baomidou.mybatisplus.core.spi](com.baomidou.mybatisplus.core.spi.md)：10 个方法声明
- [com.baomidou.mybatisplus.core.toolkit](com.baomidou.mybatisplus.core.toolkit.md)：191 个方法声明
- [com.baomidou.mybatisplus.core.toolkit.reflect](com.baomidou.mybatisplus.core.toolkit.reflect.md)：9 个方法声明
- [com.baomidou.mybatisplus.core.toolkit.sql](com.baomidou.mybatisplus.core.toolkit.sql.md)：23 个方法声明
- [com.baomidou.mybatisplus.core.toolkit.support](com.baomidou.mybatisplus.core.toolkit.support.md)：14 个方法声明
- [com.baomidou.mybatisplus.extension](com.baomidou.mybatisplus.extension.md)：5 个方法声明
- [com.baomidou.mybatisplus.extension.activerecord](com.baomidou.mybatisplus.extension.activerecord.md)：16 个方法声明
- [com.baomidou.mybatisplus.extension.conditions](com.baomidou.mybatisplus.extension.conditions.md)：72 个方法声明
- [com.baomidou.mybatisplus.extension.conditions.query](com.baomidou.mybatisplus.extension.conditions.query.md)：20 个方法声明
- [com.baomidou.mybatisplus.extension.conditions.update](com.baomidou.mybatisplus.extension.conditions.update.md)：17 个方法声明
- [com.baomidou.mybatisplus.extension.ddl](com.baomidou.mybatisplus.extension.ddl.md)：32 个方法声明
- [com.baomidou.mybatisplus.extension.ddl.history](com.baomidou.mybatisplus.extension.ddl.history.md)：24 个方法声明
- [com.baomidou.mybatisplus.extension.handlers](com.baomidou.mybatisplus.extension.handlers.md)：22 个方法声明
- [com.baomidou.mybatisplus.extension.incrementer](com.baomidou.mybatisplus.extension.incrementer.md)：18 个方法声明
- [com.baomidou.mybatisplus.extension.injector.methods](com.baomidou.mybatisplus.extension.injector.methods.md)：5 个方法声明
- [com.baomidou.mybatisplus.extension.p6spy](com.baomidou.mybatisplus.extension.p6spy.md)：6 个方法声明
- [com.baomidou.mybatisplus.extension.parser](com.baomidou.mybatisplus.extension.parser.md)：9 个方法声明
- [com.baomidou.mybatisplus.extension.parser.cache](com.baomidou.mybatisplus.extension.parser.cache.md)：22 个方法声明
- [com.baomidou.mybatisplus.extension.plugins](com.baomidou.mybatisplus.extension.plugins.md)：6 个方法声明
- [com.baomidou.mybatisplus.extension.plugins.handler](com.baomidou.mybatisplus.extension.plugins.handler.md)：8 个方法声明
- [com.baomidou.mybatisplus.extension.plugins.inner](com.baomidou.mybatisplus.extension.plugins.inner.md)：51 个方法声明
- [com.baomidou.mybatisplus.extension.plugins.pagination](com.baomidou.mybatisplus.extension.plugins.pagination.md)：42 个方法声明
- [com.baomidou.mybatisplus.extension.plugins.pagination.dialects](com.baomidou.mybatisplus.extension.plugins.pagination.dialects.md)：15 个方法声明
- [com.baomidou.mybatisplus.extension.repository](com.baomidou.mybatisplus.extension.repository.md)：65 个方法声明
- [com.baomidou.mybatisplus.extension.scripting](com.baomidou.mybatisplus.extension.scripting.md)：3 个方法声明
- [com.baomidou.mybatisplus.extension.service](com.baomidou.mybatisplus.extension.service.md)：4 个方法声明
- [com.baomidou.mybatisplus.extension.spi](com.baomidou.mybatisplus.extension.spi.md)：10 个方法声明
- [com.baomidou.mybatisplus.extension.spring](com.baomidou.mybatisplus.extension.spring.md)：41 个方法声明
- [com.baomidou.mybatisplus.extension.toolkit](com.baomidou.mybatisplus.extension.toolkit.md)：133 个方法声明
- [com.baomidou.mybatisplus.jsqlparser](com.baomidou.mybatisplus.jsqlparser.md)：2 个方法声明
