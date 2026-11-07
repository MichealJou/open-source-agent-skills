# cn.hutool.extra.spring

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.spring.SpringUtil`

```java
public class cn.hutool.extra.spring.SpringUtil implements org.springframework.beans.factory.config.BeanFactoryPostProcessor,org.springframework.context.ApplicationContextAware {
  public cn.hutool.extra.spring.SpringUtil();
  public void postProcessBeanFactory(org.springframework.beans.factory.config.ConfigurableListableBeanFactory) throws org.springframework.beans.BeansException;
  public void setApplicationContext(org.springframework.context.ApplicationContext);
  public static org.springframework.context.ApplicationContext getApplicationContext();
  public static org.springframework.beans.factory.ListableBeanFactory getBeanFactory();
  public static org.springframework.beans.factory.config.ConfigurableListableBeanFactory getConfigurableBeanFactory() throws cn.hutool.core.exceptions.UtilException;
  public static <T> T getBean(java.lang.String);
  public static <T> T getBean(java.lang.Class<T>);
  public static <T> T getBean(java.lang.Class<T>, java.lang.Object...);
  public static <T> T getBean(java.lang.String, java.lang.Class<T>);
  public static java.lang.Object getBean(java.lang.String, java.lang.Object...);
  public static <T> T getBean(cn.hutool.core.lang.TypeReference<T>);
  public static <T> java.util.Map<java.lang.String, T> getBeansOfType(java.lang.Class<T>);
  public static java.lang.String[] getBeanNamesForType(java.lang.Class<?>);
  public static java.lang.String getProperty(java.lang.String);
  public static java.lang.String getProperty(java.lang.String, java.lang.String);
  public static <T> T getProperty(java.lang.String, java.lang.Class<T>, T);
  public static java.lang.String getApplicationName();
  public static java.lang.String[] getActiveProfiles();
  public static java.lang.String getActiveProfile();
  public static <T> void registerBean(java.lang.String, T);
  public static void unregisterBean(java.lang.String);
  public static void publishEvent(org.springframework.context.ApplicationEvent);
  public static void publishEvent(java.lang.Object);
}
```
