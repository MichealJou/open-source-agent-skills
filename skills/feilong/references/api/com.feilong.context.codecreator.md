# com.feilong.context.codecreator

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.context.codecreator.CodeCreatorHelper`

```java
public class com.feilong.context.codecreator.CodeCreatorHelper {
  public static java.lang.String debugSeparator(boolean);
  public static java.lang.String debugLength(java.lang.StringBuilder, boolean);
  public static java.lang.String formatLastValue(java.lang.Long, int);
}
```

## `com.feilong.context.codecreator.DefaultGuestShoppingcartLineIdCreator`

```java
public class com.feilong.context.codecreator.DefaultGuestShoppingcartLineIdCreator implements com.feilong.context.codecreator.GuestShoppingcartLineIdCreator {
  public com.feilong.context.codecreator.DefaultGuestShoppingcartLineIdCreator();
  public long create();
}
```

## `com.feilong.context.codecreator.GuestShoppingcartLineIdCreator`

```java
public interface com.feilong.context.codecreator.GuestShoppingcartLineIdCreator {
  public abstract long create();
}
```

## `com.feilong.context.codecreator.MultiSellerOrderCodeCreator`

```java
public interface com.feilong.context.codecreator.MultiSellerOrderCodeCreator extends com.feilong.context.codecreator.OrderCodeCreator {
  public abstract java.lang.String create(java.lang.Long, java.lang.Long);
}
```

## `com.feilong.context.codecreator.SequenceTypeOrderCodeCreator`

```java
public interface com.feilong.context.codecreator.SequenceTypeOrderCodeCreator extends com.feilong.context.codecreator.OrderCodeCreator {
  public abstract java.lang.String create(long, int);
}
```

## `com.feilong.context.codecreator.SimpleMultiSellerOrderCodeCreator`

```java
public class com.feilong.context.codecreator.SimpleMultiSellerOrderCodeCreator implements com.feilong.context.codecreator.MultiSellerOrderCodeCreator {
  public com.feilong.context.codecreator.SimpleMultiSellerOrderCodeCreator();
  public java.lang.String create(java.lang.Long, java.lang.Long);
  public void setSimpleMultiSellerOrderCodeCreatorConfig(com.feilong.context.codecreator.SimpleMultiSellerOrderCodeCreatorConfig);
}
```

## `com.feilong.context.codecreator.SimpleMultiSellerOrderCodeCreatorConfig`

```java
public class com.feilong.context.codecreator.SimpleMultiSellerOrderCodeCreatorConfig {
  public com.feilong.context.codecreator.SimpleMultiSellerOrderCodeCreatorConfig();
  public java.lang.String getPrefix();
  public void setPrefix(java.lang.String);
  public int getBuyerIdLastLength();
  public void setBuyerIdLastLength(int);
  public int getShopIdLastLength();
  public void setShopIdLastLength(int);
  public int getRandomNumberLength();
  public void setRandomNumberLength(int);
  public boolean getIsDebug();
  public void setIsDebug(boolean);
}
```

## `com.feilong.context.codecreator.SimpleSequenceTypeOrderCodeCreator`

```java
public class com.feilong.context.codecreator.SimpleSequenceTypeOrderCodeCreator implements com.feilong.context.codecreator.SequenceTypeOrderCodeCreator {
  public com.feilong.context.codecreator.SimpleSequenceTypeOrderCodeCreator();
  public com.feilong.context.codecreator.SimpleSequenceTypeOrderCodeCreator(boolean);
  public java.lang.String create(long, int);
  public void setIsDebug(boolean);
}
```
