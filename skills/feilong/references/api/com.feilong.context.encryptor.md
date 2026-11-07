# com.feilong.context.encryptor

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.context.encryptor.Encryptor`

```java
public interface com.feilong.context.encryptor.Encryptor<T extends com.feilong.context.encryptor.Encryptorable> {
  public abstract java.lang.String encrypt(T);
  public abstract T decrypt(java.lang.String, java.lang.Class<T>);
}
```

## `com.feilong.context.encryptor.SymmetricJsonHexEncryptor`

```java
public class com.feilong.context.encryptor.SymmetricJsonHexEncryptor<T extends com.feilong.context.encryptor.Encryptorable> implements com.feilong.context.encryptor.Encryptor<T> {
  public com.feilong.context.encryptor.SymmetricJsonHexEncryptor();
  public java.lang.String encrypt(T);
  public T decrypt(java.lang.String, java.lang.Class<T>);
  public void setSymmetricType(com.feilong.security.symmetric.SymmetricType);
  public void setKey(java.lang.String);
  public void setCharsetName(java.lang.String);
}
```
