# com.feilong.coreextension.awt

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.coreextension.awt.ClipboardUtil` | `Reader getClipboardReader()` | 获得 clipboard reader. |
| `com.feilong.coreextension.awt.ClipboardUtil` | `String getClipboardContent()` | 从剪贴板中取数据. |
| `com.feilong.coreextension.awt.ClipboardUtil` | `void setClipboardContent(CharSequence data)` | 设置剪贴板数据. |
| `com.feilong.coreextension.awt.DesktopUtil` | `void browse(String urlPattern,Object... args)` | 使用系统默认浏览器,打开url. 如果 urlPattern 是null,抛出 NullPointerException 如果 urlPattern 是blank,抛出 IllegalArgumentException |
| `com.feilong.coreextension.awt.DesktopUtil` | `void mail(String urlPattern,Object... args)` | 发送邮件. 如果 urlPattern 是null,抛出 NullPointerException 如果 urlPattern 是blank,抛出 IllegalArgumentException |
| `com.feilong.coreextension.awt.DesktopUtil` | `void open(String urlPattern,Object... args)` | 启动关联应用程序来打开文件.. 如果 urlPattern 是null,抛出 NullPointerException 如果 urlPattern 是blank,抛出 IllegalArgumentException |
| `com.feilong.coreextension.awt.DesktopUtil` | `void print(String urlPattern,Object... args)` | 打印. 如果 urlPattern 是null,抛出 NullPointerException 如果 urlPattern 是blank,抛出 IllegalArgumentException |
