# com.baomidou.mybatisplus.jsqlparser

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.jsqlparser.JsqlParserThreadPool` | `ExecutorService getDefaultThreadPoolExecutor()` | 获取默认解析线程池(固定大小) |
| `com.baomidou.mybatisplus.jsqlparser.JsqlParserThreadPool` | `void addShutdownHook(ExecutorService executorService)` | 注册Jvm退出钩子 |
