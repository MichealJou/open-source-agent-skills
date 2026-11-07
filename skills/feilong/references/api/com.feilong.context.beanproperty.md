# com.feilong.context.beanproperty

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.context.beanproperty.HttpTypeBeanProperty`

```java
public interface com.feilong.context.beanproperty.HttpTypeBeanProperty extends com.feilong.context.beanproperty.BeanProperty {
  public abstract java.lang.String getUri();
  public abstract void setUri(java.lang.String);
  public abstract java.lang.String getMethod();
  public abstract void setMethod(java.lang.String);
}
```

## `com.feilong.context.beanproperty.JaxWsTypeBeanProperty`

```java
public interface com.feilong.context.beanproperty.JaxWsTypeBeanProperty extends com.feilong.context.beanproperty.BeanProperty {
  public abstract java.lang.String getWsdlUrl();
  public abstract void setWsdlUrl(java.lang.String);
  public abstract java.lang.String getOperationName();
  public abstract void setOperationName(java.lang.String);
}
```

## `com.feilong.context.beanproperty.SimpleHttpTypeBeanProperty`

```java
public class com.feilong.context.beanproperty.SimpleHttpTypeBeanProperty implements com.feilong.context.beanproperty.HttpTypeBeanProperty {
  public com.feilong.context.beanproperty.SimpleHttpTypeBeanProperty();
  public com.feilong.context.beanproperty.SimpleHttpTypeBeanProperty(java.lang.String, java.lang.String);
  public java.lang.String getUri();
  public void setUri(java.lang.String);
  public java.lang.String getMethod();
  public void setMethod(java.lang.String);
}
```

## `com.feilong.context.beanproperty.SimpleJaxWsTypeBeanProperty`

```java
public class com.feilong.context.beanproperty.SimpleJaxWsTypeBeanProperty implements com.feilong.context.beanproperty.JaxWsTypeBeanProperty {
  public com.feilong.context.beanproperty.SimpleJaxWsTypeBeanProperty();
  public com.feilong.context.beanproperty.SimpleJaxWsTypeBeanProperty(java.lang.String, java.lang.String);
  public java.lang.String getWsdlUrl();
  public void setWsdlUrl(java.lang.String);
  public java.lang.String getOperationName();
  public void setOperationName(java.lang.String);
}
```
