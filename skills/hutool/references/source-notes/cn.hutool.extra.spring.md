# cn.hutool.extra.spring

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.extra.spring.SpringUtil` | `ApplicationContext getApplicationContext()` | 获取ApplicationContext |
| `cn.hutool.extra.spring.SpringUtil` | `ConfigurableListableBeanFactory getConfigurableBeanFactory()` | 获取ConfigurableListableBeanFactory |
| `cn.hutool.extra.spring.SpringUtil` | `ListableBeanFactory getBeanFactory()` | 获取ListableBeanFactory，可能为ConfigurableListableBeanFactory 或 ApplicationContextAware |
| `cn.hutool.extra.spring.SpringUtil` | `Map<String, T> getBeansOfType(Class<T> type)` | 获取指定类型对应的所有Bean，包括子类 |
| `cn.hutool.extra.spring.SpringUtil` | `Object getBean(String name,Object... args)` | 通过name,以及Clazz返回指定的Bean |
| `cn.hutool.extra.spring.SpringUtil` | `String getActiveProfile()` | 获取当前的环境配置，当有多个环境配置时，只获取第一个 |
| `cn.hutool.extra.spring.SpringUtil` | `String getApplicationName()` | 获取应用程序名称 |
| `cn.hutool.extra.spring.SpringUtil` | `String getProperty(String key)` | 获取配置文件配置项的值 |
| `cn.hutool.extra.spring.SpringUtil` | `String getProperty(String key,String defaultValue)` | 获取配置文件配置项的值 |
| `cn.hutool.extra.spring.SpringUtil` | `String[] getActiveProfiles()` | 获取当前的环境配置，无配置返回null |
| `cn.hutool.extra.spring.SpringUtil` | `String[] getBeanNamesForType(Class<?> type)` | 获取指定类型对应的Bean名称，包括子类 |
| `cn.hutool.extra.spring.SpringUtil` | `T getBean(Class<T> clazz)` | 通过class获取Bean |
| `cn.hutool.extra.spring.SpringUtil` | `T getBean(Class<T> clazz,Object... args)` | 通过class获取Bean |
| `cn.hutool.extra.spring.SpringUtil` | `T getBean(String name)` | 通过name获取 Bean |
| `cn.hutool.extra.spring.SpringUtil` | `T getBean(String name,Class<T> clazz)` | 通过name,以及Clazz返回指定的Bean |
| `cn.hutool.extra.spring.SpringUtil` | `T getBean(TypeReference<T> reference)` | 通过类型参考返回带泛型参数的Bean |
| `cn.hutool.extra.spring.SpringUtil` | `T getProperty(String key,Class<T> targetType,T defaultValue)` | 获取配置文件配置项的值 |
| `cn.hutool.extra.spring.SpringUtil` | `void postProcessBeanFactory(ConfigurableListableBeanFactory beanFactory)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.spring.SpringUtil` | `void publishEvent(ApplicationEvent event)` | 发布事件 |
| `cn.hutool.extra.spring.SpringUtil` | `void publishEvent(Object event)` | 发布事件 Spring 4.2+ 版本事件可以不再是ApplicationEvent的子类 |
| `cn.hutool.extra.spring.SpringUtil` | `void registerBean(String beanName,T bean)` | 动态向Spring注册Bean 由org.springframework.beans.factory.BeanFactory 实现，通过工具开放API 更新: shadow 2021-07-29 17:20:44 增加自动注入，修复注册bean无法反向注入的问题 |
| `cn.hutool.extra.spring.SpringUtil` | `void setApplicationContext(ApplicationContext applicationContext)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.spring.SpringUtil` | `void unregisterBean(String beanName)` | 注销bean 将Spring中的bean注销，请谨慎使用 |
