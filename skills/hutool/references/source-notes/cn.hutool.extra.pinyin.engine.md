# cn.hutool.extra.pinyin.engine

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.extra.pinyin.engine.PinyinFactory` | `PinyinEngine create()` | 根据用户引入的拼音引擎jar，自动创建对应的拼音引擎对象 推荐创建的引擎单例使用，此方法每次调用会返回新的引擎 |
| `cn.hutool.extra.pinyin.engine.PinyinFactory` | `PinyinEngine get()` | 获得单例的PinyinEngine |
