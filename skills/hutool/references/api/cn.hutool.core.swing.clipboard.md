# cn.hutool.core.swing.clipboard

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.swing.clipboard.ClipboardListener`

```java
public interface cn.hutool.core.swing.clipboard.ClipboardListener {
  public abstract java.awt.datatransfer.Transferable onChange(java.awt.datatransfer.Clipboard, java.awt.datatransfer.Transferable);
}
```

## `cn.hutool.core.swing.clipboard.ClipboardMonitor`

```java
public final class cn.hutool.core.swing.clipboard.ClipboardMonitor extends java.lang.Enum<cn.hutool.core.swing.clipboard.ClipboardMonitor> implements java.awt.datatransfer.ClipboardOwner, java.lang.Runnable, java.io.Closeable {
  public static cn.hutool.core.swing.clipboard.ClipboardMonitor[] values();
  public static cn.hutool.core.swing.clipboard.ClipboardMonitor valueOf(java.lang.String);
  public cn.hutool.core.swing.clipboard.ClipboardMonitor setTryCount(int);
  public cn.hutool.core.swing.clipboard.ClipboardMonitor setDelay(long);
  public cn.hutool.core.swing.clipboard.ClipboardMonitor addListener(cn.hutool.core.swing.clipboard.ClipboardListener);
  public cn.hutool.core.swing.clipboard.ClipboardMonitor removeListener(cn.hutool.core.swing.clipboard.ClipboardListener);
  public cn.hutool.core.swing.clipboard.ClipboardMonitor clearListener();
  public void lostOwnership(java.awt.datatransfer.Clipboard, java.awt.datatransfer.Transferable);
  public synchronized void run();
  public void listen(boolean);
  public void close();
}
```

## `cn.hutool.core.swing.clipboard.ClipboardUtil`

```java
public class cn.hutool.core.swing.clipboard.ClipboardUtil {
  public cn.hutool.core.swing.clipboard.ClipboardUtil();
  public static java.awt.datatransfer.Clipboard getClipboard();
  public static void set(java.awt.datatransfer.Transferable);
  public static void set(java.awt.datatransfer.Transferable, java.awt.datatransfer.ClipboardOwner);
  public static java.lang.Object get(java.awt.datatransfer.DataFlavor);
  public static java.lang.Object get(java.awt.datatransfer.Transferable, java.awt.datatransfer.DataFlavor);
  public static void setStr(java.lang.String);
  public static java.lang.String getStr();
  public static java.lang.String getStr(java.awt.datatransfer.Transferable);
  public static void setImage(java.awt.Image);
  public static java.awt.Image getImage();
  public static java.awt.Image getImage(java.awt.datatransfer.Transferable);
  public static void listen(cn.hutool.core.swing.clipboard.ClipboardListener);
  public static void listen(cn.hutool.core.swing.clipboard.ClipboardListener, boolean);
  public static void listen(int, long, cn.hutool.core.swing.clipboard.ClipboardListener, boolean);
}
```

## `cn.hutool.core.swing.clipboard.ImageSelection`

```java
public class cn.hutool.core.swing.clipboard.ImageSelection implements java.awt.datatransfer.Transferable,java.io.Serializable {
  public cn.hutool.core.swing.clipboard.ImageSelection(java.awt.Image);
  public java.awt.datatransfer.DataFlavor[] getTransferDataFlavors();
  public boolean isDataFlavorSupported(java.awt.datatransfer.DataFlavor);
  public java.lang.Object getTransferData(java.awt.datatransfer.DataFlavor) throws java.awt.datatransfer.UnsupportedFlavorException;
}
```

## `cn.hutool.core.swing.clipboard.StrClipboardListener`

```java
public abstract class cn.hutool.core.swing.clipboard.StrClipboardListener implements cn.hutool.core.swing.clipboard.ClipboardListener,java.io.Serializable {
  public cn.hutool.core.swing.clipboard.StrClipboardListener();
  public java.awt.datatransfer.Transferable onChange(java.awt.datatransfer.Clipboard, java.awt.datatransfer.Transferable);
  public abstract java.awt.datatransfer.Transferable onChange(java.awt.datatransfer.Clipboard, java.lang.String);
}
```
