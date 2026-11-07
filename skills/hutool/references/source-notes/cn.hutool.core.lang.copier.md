# cn.hutool.core.lang.copier

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.lang.copier.Copier` | `T copy()` | 执行拷贝 |
| `cn.hutool.core.lang.copier.SrcToDestCopier` | `C setCopyFilter(Filter<T> copyFilter)` | 设置过滤器 |
| `cn.hutool.core.lang.copier.SrcToDestCopier` | `C setDest(T dest)` | 设置目标 |
| `cn.hutool.core.lang.copier.SrcToDestCopier` | `C setSrc(T src)` | 设置源 |
| `cn.hutool.core.lang.copier.SrcToDestCopier` | `Filter<T> getCopyFilter()` | 获得过滤器 |
| `cn.hutool.core.lang.copier.SrcToDestCopier` | `T getDest()` | 获得目标 |
| `cn.hutool.core.lang.copier.SrcToDestCopier` | `T getSrc()` | 获取源 |
