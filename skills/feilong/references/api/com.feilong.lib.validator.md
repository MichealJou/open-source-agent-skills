# com.feilong.lib.validator

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.validator.DomainValidator`

```java
public class com.feilong.lib.validator.DomainValidator implements java.io.Serializable {
  public static synchronized com.feilong.lib.validator.DomainValidator getInstance();
  public static synchronized com.feilong.lib.validator.DomainValidator getInstance(boolean);
  public boolean isValid(java.lang.String);
  public boolean isValidTld(java.lang.String);
  public boolean isValidInfrastructureTld(java.lang.String);
  public boolean isValidGenericTld(java.lang.String);
  public boolean isValidCountryCodeTld(java.lang.String);
  public boolean isValidLocalTld(java.lang.String);
  public static synchronized void updateTLDOverride(com.feilong.lib.validator.DomainValidator$ArrayType, java.lang.String[]);
  public static java.lang.String[] getTLDEntries(com.feilong.lib.validator.DomainValidator$ArrayType);
}
```

## `com.feilong.lib.validator.DomainValidator$ArrayType`

```java
public final class com.feilong.lib.validator.DomainValidator$ArrayType extends java.lang.Enum<com.feilong.lib.validator.DomainValidator$ArrayType> {
  public static com.feilong.lib.validator.DomainValidator$ArrayType[] values();
  public static com.feilong.lib.validator.DomainValidator$ArrayType valueOf(java.lang.String);
}
```

## `com.feilong.lib.validator.EmailValidator`

```java
public class com.feilong.lib.validator.EmailValidator implements java.io.Serializable {
  public static com.feilong.lib.validator.EmailValidator getInstance();
  public static com.feilong.lib.validator.EmailValidator getInstance(boolean, boolean);
  public static com.feilong.lib.validator.EmailValidator getInstance(boolean);
  public boolean isValid(java.lang.String);
}
```

## `com.feilong.lib.validator.InetAddressValidator`

```java
public class com.feilong.lib.validator.InetAddressValidator implements java.io.Serializable {
  public com.feilong.lib.validator.InetAddressValidator();
  public static com.feilong.lib.validator.InetAddressValidator getInstance();
  public boolean isValid(java.lang.String);
  public boolean isValidInet4Address(java.lang.String);
  public boolean isValidInet6Address(java.lang.String);
}
```

## `com.feilong.lib.validator.RegexValidator`

```java
public class com.feilong.lib.validator.RegexValidator implements java.io.Serializable {
  public com.feilong.lib.validator.RegexValidator(java.lang.String);
  public com.feilong.lib.validator.RegexValidator(java.lang.String[], boolean);
  public boolean isValid(java.lang.String);
  public java.lang.String[] match(java.lang.String);
  public java.lang.String toString();
}
```
