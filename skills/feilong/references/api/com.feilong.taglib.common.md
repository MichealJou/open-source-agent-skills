# com.feilong.taglib.common

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.taglib.common.AbstractContainsSupport`

```java
public abstract class com.feilong.taglib.common.AbstractContainsSupport extends com.feilong.taglib.AbstractConditionalTag {
  public com.feilong.taglib.common.AbstractContainsSupport();
  public boolean condition();
  public static boolean containsByStringValue(java.util.Iterator<?>, java.lang.Object);
  public void setCollection(java.lang.Object);
  public void setValue(java.lang.Object);
}
```

## `com.feilong.taglib.common.IsContainsTag`

```java
public class com.feilong.taglib.common.IsContainsTag extends com.feilong.taglib.common.AbstractContainsSupport {
  public com.feilong.taglib.common.IsContainsTag();
}
```

## `com.feilong.taglib.common.IsInTimeTag`

```java
public class com.feilong.taglib.common.IsInTimeTag extends com.feilong.taglib.AbstractConditionalTag {
  public com.feilong.taglib.common.IsInTimeTag();
  public boolean condition();
  public void setDate(java.util.Date);
  public void setBeginDate(java.util.Date);
  public void setEndDate(java.util.Date);
  public void setBeginDateString(java.lang.String);
  public void setEndDateString(java.lang.String);
  public void setPattern(java.lang.String);
}
```

## `com.feilong.taglib.common.IsNotContainsTag`

```java
public class com.feilong.taglib.common.IsNotContainsTag extends com.feilong.taglib.common.AbstractContainsSupport {
  public com.feilong.taglib.common.IsNotContainsTag();
  public boolean condition();
}
```

## `com.feilong.taglib.common.SwitchCaseTag`

```java
public class com.feilong.taglib.common.SwitchCaseTag extends com.feilong.taglib.BaseTag {
  public com.feilong.taglib.common.SwitchCaseTag();
  public int doStartTag();
  public void setValue(java.lang.String);
}
```

## `com.feilong.taglib.common.SwitchDefaultTag`

```java
public class com.feilong.taglib.common.SwitchDefaultTag extends com.feilong.taglib.BaseTag {
  public com.feilong.taglib.common.SwitchDefaultTag();
  public int doStartTag();
}
```

## `com.feilong.taglib.common.SwitchTag`

```java
public class com.feilong.taglib.common.SwitchTag extends com.feilong.taglib.BaseTag {
  public com.feilong.taglib.common.SwitchTag();
  public int doStartTag();
  public synchronized boolean isExecuteTag();
  public synchronized void setExecuteTag();
  public void release();
  public void setValue(java.lang.String);
  public java.lang.String getValue();
}
```
