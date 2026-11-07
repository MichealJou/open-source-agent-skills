# com.feilong.lib.org.apache.http.impl.entity

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.impl.entity.DisallowIdentityContentLengthStrategy`

```java
public class com.feilong.lib.org.apache.http.impl.entity.DisallowIdentityContentLengthStrategy implements com.feilong.lib.org.apache.http.entity.ContentLengthStrategy {
  public com.feilong.lib.org.apache.http.impl.entity.DisallowIdentityContentLengthStrategy(com.feilong.lib.org.apache.http.entity.ContentLengthStrategy);
  public long determineLength(com.feilong.lib.org.apache.http.HttpMessage) throws com.feilong.lib.org.apache.http.HttpException;
}
```

## `com.feilong.lib.org.apache.http.impl.entity.LaxContentLengthStrategy`

```java
public class com.feilong.lib.org.apache.http.impl.entity.LaxContentLengthStrategy implements com.feilong.lib.org.apache.http.entity.ContentLengthStrategy {
  public com.feilong.lib.org.apache.http.impl.entity.LaxContentLengthStrategy(int);
  public com.feilong.lib.org.apache.http.impl.entity.LaxContentLengthStrategy();
  public long determineLength(com.feilong.lib.org.apache.http.HttpMessage) throws com.feilong.lib.org.apache.http.HttpException;
}
```

## `com.feilong.lib.org.apache.http.impl.entity.StrictContentLengthStrategy`

```java
public class com.feilong.lib.org.apache.http.impl.entity.StrictContentLengthStrategy implements com.feilong.lib.org.apache.http.entity.ContentLengthStrategy {
  public com.feilong.lib.org.apache.http.impl.entity.StrictContentLengthStrategy(int);
  public com.feilong.lib.org.apache.http.impl.entity.StrictContentLengthStrategy();
  public long determineLength(com.feilong.lib.org.apache.http.HttpMessage) throws com.feilong.lib.org.apache.http.HttpException;
}
```
