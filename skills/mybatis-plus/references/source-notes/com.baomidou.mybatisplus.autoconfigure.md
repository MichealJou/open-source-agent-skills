# com.baomidou.mybatisplus.autoconfigure

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.autoconfigure.ConfigurationCustomizer` | `void customize(MybatisConfiguration configuration)` | 【原文待译】Customize the given a MybatisConfiguration object. |
| `com.baomidou.mybatisplus.autoconfigure.DdlApplicationRunner` | `void run(ApplicationArguments args)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.autoconfigure.DdlAutoConfiguration` | `DdlApplicationRunner ddlApplicationRunner(List<IDdl> ddlList)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.autoconfigure.IdentifierGeneratorAutoConfiguration` | `IdentifierGenerator identifierGenerator(InetUtils inetUtils)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.autoconfigure.MybatisPlusAutoConfiguration` | `MybatisPlusApplicationContextAware mybatisPlusSpringApplicationContextAware()` | 【原文待译】@deprecated 3.5.13 |
| `com.baomidou.mybatisplus.autoconfigure.MybatisPlusAutoConfiguration` | `SqlSessionFactory sqlSessionFactory(DataSource dataSource)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.autoconfigure.MybatisPlusAutoConfiguration` | `SqlSessionTemplate sqlSessionTemplate(SqlSessionFactory sqlSessionFactory)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.autoconfigure.MybatisPlusAutoConfiguration` | `void afterPropertiesSet()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.autoconfigure.MybatisPlusAutoConfiguration$AutoConfiguredMapperScannerRegistrar` | `void registerBeanDefinitions(AnnotationMetadata importingClassMetadata,BeanDefinitionRegistry registry)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.autoconfigure.MybatisPlusAutoConfiguration$AutoConfiguredMapperScannerRegistrar` | `void setBeanFactory(BeanFactory beanFactory)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.autoconfigure.MybatisPlusAutoConfiguration$AutoConfiguredMapperScannerRegistrar` | `void setEnvironment(Environment environment)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.autoconfigure.MybatisPlusAutoConfiguration$MapperScannerRegistrarNotFoundConfiguration` | `void afterPropertiesSet()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.autoconfigure.MybatisPlusInnerInterceptorAutoConfiguration` | `MybatisPlusInterceptor defaultMybatisPlusInterceptor(List<InnerInterceptor> innerInterceptorList)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.autoconfigure.MybatisPlusLanguageDriverAutoConfiguration$FreeMarkerConfiguration` | `FreeMarkerLanguageDriverConfig freeMarkerLanguageDriverConfig()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.autoconfigure.MybatisPlusLanguageDriverAutoConfiguration$ThymeleafConfiguration` | `ThymeleafLanguageDriverConfig thymeleafLanguageDriverConfig()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.autoconfigure.MybatisPlusLanguageDriverAutoConfiguration$VelocityConfiguration` | `VelocityLanguageDriverConfig velocityLanguageDriverConfig()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties` | `Resource[] resolveMapperLocations()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration` | `void applyTo(MybatisConfiguration target)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.autoconfigure.MybatisPlusPropertiesCustomizer` | `void customize(MybatisPlusProperties properties)` | 【原文待译】Customize the given a MybatisPlusProperties object. |
| `com.baomidou.mybatisplus.autoconfigure.SafetyEncryptProcessor` | `void postProcessEnvironment(ConfigurableEnvironment environment,SpringApplication application)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.autoconfigure.SpringBootVFS` | `boolean isValid()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.autoconfigure.SpringBootVFS` | `void setClassLoaderSupplier(Supplier<ClassLoader> supplier)` | 【原文待译】Set the supplier for providing ClassLoader to used. Default is a returned instance from ClassUtils#getDefaultClassLoader(). |
| `com.baomidou.mybatisplus.autoconfigure.SpringBootVFS` | `void setUrlDecodingCharset(Charset charset)` | 【原文待译】Set the charset for decoding an encoded URL string. Default is system default charset. |
| `com.baomidou.mybatisplus.autoconfigure.SqlSessionFactoryBeanCustomizer` | `void customize(MybatisSqlSessionFactoryBean factoryBean)` | 【原文待译】Customize the given a MybatisSqlSessionFactoryBean object. |
