# com.feilong.lib.io.output

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.io.output.StringBuilderWriter`

```java
public class com.feilong.lib.io.output.StringBuilderWriter extends java.io.Writer implements java.io.Serializable {
  public com.feilong.lib.io.output.StringBuilderWriter();
  public com.feilong.lib.io.output.StringBuilderWriter(int);
  public java.io.Writer append(char);
  public java.io.Writer append(java.lang.CharSequence);
  public java.io.Writer append(java.lang.CharSequence, int, int);
  public void close();
  public void flush();
  public void write(java.lang.String);
  public void write(char[], int, int);
  public java.lang.StringBuilder getBuilder();
  public java.lang.String toString();
  public java.lang.Appendable append(char) throws java.io.IOException;
  public java.lang.Appendable append(java.lang.CharSequence, int, int) throws java.io.IOException;
  public java.lang.Appendable append(java.lang.CharSequence) throws java.io.IOException;
}
```
