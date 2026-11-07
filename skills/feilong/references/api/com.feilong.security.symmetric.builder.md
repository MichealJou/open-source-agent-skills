# com.feilong.security.symmetric.builder

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.security.symmetric.builder.AbstractSecretKeySpecBuilder`

```java
public abstract class com.feilong.security.symmetric.builder.AbstractSecretKeySpecBuilder implements com.feilong.security.symmetric.builder.KeyBuilder {
  public com.feilong.security.symmetric.builder.AbstractSecretKeySpecBuilder();
  public java.security.Key build(java.lang.String, java.lang.String);
}
```

## `com.feilong.security.symmetric.builder.Base64KeyBuilder`

```java
public class com.feilong.security.symmetric.builder.Base64KeyBuilder extends com.feilong.security.symmetric.builder.AbstractSecretKeySpecBuilder {
  public com.feilong.security.symmetric.builder.Base64KeyBuilder();
}
```

## `com.feilong.security.symmetric.builder.DefaultKeyBuilder`

```java
public class com.feilong.security.symmetric.builder.DefaultKeyBuilder extends com.feilong.security.symmetric.builder.AbstractSecretKeySpecBuilder {
  public com.feilong.security.symmetric.builder.DefaultKeyBuilder();
}
```

## `com.feilong.security.symmetric.builder.KeyBuilder`

```java
public interface com.feilong.security.symmetric.builder.KeyBuilder {
  public abstract java.security.Key build(java.lang.String, java.lang.String);
}
```

## `com.feilong.security.symmetric.builder.KeyGeneratorKeyBuilder`

```java
public class com.feilong.security.symmetric.builder.KeyGeneratorKeyBuilder extends com.feilong.security.symmetric.builder.AbstractSecretKeySpecBuilder {
  public com.feilong.security.symmetric.builder.KeyGeneratorKeyBuilder();
  public com.feilong.security.symmetric.builder.KeyGeneratorKeyBuilder(java.lang.String);
  public com.feilong.security.symmetric.builder.KeyGeneratorKeyBuilder(int, java.lang.String);
  public void setSecureRandomAlgorithm(java.lang.String);
  public void setKeyGeneratorKeysize(int);
}
```

## `com.feilong.security.symmetric.builder.TransformationBuilder`

```java
public class com.feilong.security.symmetric.builder.TransformationBuilder {
  public static java.lang.String build(java.lang.String, com.feilong.security.symmetric.CipherMode, com.feilong.security.symmetric.CipherPadding);
}
```
