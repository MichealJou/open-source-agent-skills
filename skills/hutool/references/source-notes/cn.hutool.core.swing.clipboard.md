# cn.hutool.core.swing.clipboard

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.swing.clipboard.ClipboardListener` | `Transferable onChange(Clipboard clipboard,Transferable contents)` | 剪贴板变动触发的事件方法 在此事件中对剪贴板设置值无效，如若修改，需返回修改内容 |
| `cn.hutool.core.swing.clipboard.ClipboardMonitor` | `ClipboardMonitor addListener(ClipboardListener listener)` | 设置 监听事件处理 |
| `cn.hutool.core.swing.clipboard.ClipboardMonitor` | `ClipboardMonitor clearListener()` | 清空监听 |
| `cn.hutool.core.swing.clipboard.ClipboardMonitor` | `ClipboardMonitor removeListener(ClipboardListener listener)` | 去除指定监听 |
| `cn.hutool.core.swing.clipboard.ClipboardMonitor` | `ClipboardMonitor setDelay(long delay)` | 设置重试等待 |
| `cn.hutool.core.swing.clipboard.ClipboardMonitor` | `ClipboardMonitor setTryCount(int tryCount)` | 设置重试次数 |
| `cn.hutool.core.swing.clipboard.ClipboardMonitor` | `void close()` | 关闭（停止）监听 |
| `cn.hutool.core.swing.clipboard.ClipboardMonitor` | `void listen(boolean sync)` | 开始监听 |
| `cn.hutool.core.swing.clipboard.ClipboardMonitor` | `void lostOwnership(Clipboard clipboard,Transferable contents)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.swing.clipboard.ClipboardMonitor` | `void run()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.swing.clipboard.ClipboardUtil` | `Clipboard getClipboard()` | 获取系统剪贴板 |
| `cn.hutool.core.swing.clipboard.ClipboardUtil` | `Image getImage()` | 从剪贴板获取图片 |
| `cn.hutool.core.swing.clipboard.ClipboardUtil` | `Image getImage(Transferable content)` | 从剪贴板的Transferable获取图片 |
| `cn.hutool.core.swing.clipboard.ClipboardUtil` | `Object get(DataFlavor flavor)` | 获取剪贴板内容 |
| `cn.hutool.core.swing.clipboard.ClipboardUtil` | `Object get(Transferable content,DataFlavor flavor)` | 获取剪贴板内容 |
| `cn.hutool.core.swing.clipboard.ClipboardUtil` | `String getStr()` | 从剪贴板获取文本 |
| `cn.hutool.core.swing.clipboard.ClipboardUtil` | `String getStr(Transferable content)` | 从剪贴板的Transferable获取文本 |
| `cn.hutool.core.swing.clipboard.ClipboardUtil` | `void listen(ClipboardListener listener)` | 监听剪贴板修改事件 |
| `cn.hutool.core.swing.clipboard.ClipboardUtil` | `void listen(ClipboardListener listener,boolean sync)` | 监听剪贴板修改事件 |
| `cn.hutool.core.swing.clipboard.ClipboardUtil` | `void listen(int tryCount,long delay,ClipboardListener listener,boolean sync)` | 监听剪贴板修改事件 |
| `cn.hutool.core.swing.clipboard.ClipboardUtil` | `void set(Transferable contents)` | 设置内容到剪贴板 |
| `cn.hutool.core.swing.clipboard.ClipboardUtil` | `void set(Transferable contents,ClipboardOwner owner)` | 设置内容到剪贴板 |
| `cn.hutool.core.swing.clipboard.ClipboardUtil` | `void setImage(Image image)` | 设置图片到剪贴板 |
| `cn.hutool.core.swing.clipboard.ClipboardUtil` | `void setStr(String text)` | 设置字符串文本到剪贴板 |
| `cn.hutool.core.swing.clipboard.ImageSelection` | `DataFlavor[] getTransferDataFlavors()` | 获取元数据类型信息 |
| `cn.hutool.core.swing.clipboard.ImageSelection` | `Object getTransferData(DataFlavor flavor)` | 获取图片 |
| `cn.hutool.core.swing.clipboard.ImageSelection` | `boolean isDataFlavorSupported(DataFlavor flavor)` | 是否支持指定元数据类型 |
| `cn.hutool.core.swing.clipboard.StrClipboardListener` | `Transferable onChange(Clipboard clipboard,String contents)` | 剪贴板变动触发的事件方法 在此事件中对剪贴板设置值无效，如若修改，需返回修改内容 |
| `cn.hutool.core.swing.clipboard.StrClipboardListener` | `Transferable onChange(Clipboard clipboard,Transferable contents)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
