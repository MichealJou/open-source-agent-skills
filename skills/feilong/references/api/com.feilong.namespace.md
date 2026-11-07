# com.feilong.namespace

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.namespace.BeanDefinitionParserUtil`

```java
public class com.feilong.namespace.BeanDefinitionParserUtil {
  public static void addPropertyValue(org.w3c.dom.Element, org.springframework.beans.factory.support.BeanDefinitionBuilder, java.lang.String, boolean);
  public static void addPropertyValue(org.w3c.dom.Element, org.springframework.beans.factory.support.RootBeanDefinition, java.lang.String, boolean);
  public static void addPropertyValue(org.w3c.dom.Element, org.springframework.beans.factory.support.BeanDefinitionBuilder, java.lang.String...);
}
```

## `com.feilong.namespace.FeilongNamespaceHandler`

```java
public class com.feilong.namespace.FeilongNamespaceHandler extends org.springframework.beans.factory.xml.NamespaceHandlerSupport {
  public com.feilong.namespace.FeilongNamespaceHandler();
  public void init();
}
```

## `com.feilong.namespace.RuntimeBeanReferenceBuilder`

```java
public class com.feilong.namespace.RuntimeBeanReferenceBuilder {
  public static org.springframework.beans.factory.config.RuntimeBeanReference build(org.springframework.beans.factory.xml.ParserContext, org.springframework.beans.factory.support.BeanDefinitionBuilder);
}
```
