# com.feilong.context.signer

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.context.signer.SHA1Signer`

```java
public class com.feilong.context.signer.SHA1Signer implements com.feilong.context.signer.Signer {
  public com.feilong.context.signer.SHA1Signer();
  public com.feilong.context.signer.SHA1Signer(java.lang.String);
  public com.feilong.context.signer.SHA1Signer(java.lang.String, java.lang.String);
  public java.lang.String sign(java.lang.CharSequence...);
  public void setKey(java.lang.String);
  public void setCharsetName(java.lang.String);
}
```

## `com.feilong.context.signer.Signer`

```java
public interface com.feilong.context.signer.Signer {
  public abstract java.lang.String sign(java.lang.CharSequence...);
}
```
