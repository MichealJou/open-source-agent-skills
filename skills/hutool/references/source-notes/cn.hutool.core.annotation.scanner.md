# cn.hutool.core.annotation.scanner

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.annotation.scanner.AbstractTypeAnnotationScanner` | `T addConverters(UnaryOperator<Class<?>> converter)` | 添加转换器 |
| `cn.hutool.core.annotation.scanner.AbstractTypeAnnotationScanner` | `T addExcludeTypes(Class<?>... excludeTypes)` | 添加不扫描的类型，该类型及其树结构将直接不被查找 |
| `cn.hutool.core.annotation.scanner.AbstractTypeAnnotationScanner` | `T setFilter(Predicate<Class<?>> filter)` | 设置过滤器，若类型无法通过该过滤器，则该类型及其树结构将直接不被查找 |
| `cn.hutool.core.annotation.scanner.AbstractTypeAnnotationScanner` | `boolean isIncludeInterfaces()` | 是否允许扫描父接口 |
| `cn.hutool.core.annotation.scanner.AbstractTypeAnnotationScanner` | `boolean isIncludeSuperClass()` | 是否允许扫描父类 |
| `cn.hutool.core.annotation.scanner.AbstractTypeAnnotationScanner` | `void scan(BiConsumer<Integer, Annotation> consumer,AnnotatedElement annotatedEle,Predicate<Annotation> filter)` | 则根据广度优先递归扫描类的层级结构，并对层级结构中类/接口声明的层级索引和它们声明的注解对象进行处理 |
| `cn.hutool.core.annotation.scanner.AbstractTypeAnnotationScanner$JdkProxyClassConverter` | `Class<?> apply(Class<?> sourceClass)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.scanner.AnnotationScanner` | `List<Annotation> getAnnotations(AnnotatedElement annotatedEle)` | 获取注解元素上的全部注解。调用该方法前，需要确保调用#support(AnnotatedElement)返回为true |
| `cn.hutool.core.annotation.scanner.AnnotationScanner` | `List<Annotation> getAnnotationsIfSupport(AnnotatedElement annotatedEle)` | 若#support(AnnotatedElement)返回true， 则调用并返回#getAnnotations(AnnotatedElement)结果， 否则返回Collections#emptyList() |
| `cn.hutool.core.annotation.scanner.AnnotationScanner` | `List<Annotation> scanByAllSupported(AnnotatedElement annotatedEle,AnnotationScanner... scanners)` | 根据指定的扫描器，扫描元素上可能存在的注解 |
| `cn.hutool.core.annotation.scanner.AnnotationScanner` | `List<Annotation> scanByAnySupported(AnnotatedElement annotatedEle,AnnotationScanner... scanners)` | 给定一组扫描器，使用第一个支持处理该类型元素的扫描器获取元素上可能存在的注解 |
| `cn.hutool.core.annotation.scanner.AnnotationScanner` | `boolean support(AnnotatedElement annotatedEle)` | 判断是否支持扫描该注解元素 |
| `cn.hutool.core.annotation.scanner.AnnotationScanner` | `void scan(BiConsumer<Integer, Annotation> consumer,AnnotatedElement annotatedEle,Predicate<Annotation> filter)` | 扫描注解元素的层级结构（若存在），然后对获取到的注解和注解对应的层级索引进行处理。 调用该方法前，需要确保调用#support(AnnotatedElement)返回为true |
| `cn.hutool.core.annotation.scanner.AnnotationScanner` | `void scanIfSupport(BiConsumer<Integer, Annotation> consumer,AnnotatedElement annotatedEle,Predicate<Annotation> filter)` | 若#support(AnnotatedElement)返回true，则调用#scan(BiConsumer, AnnotatedElement, Predicate) |
| `cn.hutool.core.annotation.scanner.ElementAnnotationScanner` | `boolean support(AnnotatedElement annotatedEle)` | 判断是否支持扫描该注解元素，仅当注解元素不为空时返回true |
| `cn.hutool.core.annotation.scanner.ElementAnnotationScanner` | `void scan(BiConsumer<Integer, Annotation> consumer,AnnotatedElement annotatedEle,Predicate<Annotation> filter)` | 扫描AnnotatedElement上直接声明的注解，调用前需要确保调用#support(AnnotatedElement)返回为true |
| `cn.hutool.core.annotation.scanner.EmptyAnnotationScanner` | `List<Annotation> getAnnotations(AnnotatedElement annotatedEle)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.scanner.EmptyAnnotationScanner` | `boolean support(AnnotatedElement annotatedEle)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.scanner.EmptyAnnotationScanner` | `void scan(BiConsumer<Integer, Annotation> consumer,AnnotatedElement annotatedEle,Predicate<Annotation> filter)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.scanner.FieldAnnotationScanner` | `boolean support(AnnotatedElement annotatedEle)` | 判断是否支持扫描该注解元素，仅当注解元素是Field时返回true |
| `cn.hutool.core.annotation.scanner.FieldAnnotationScanner` | `void scan(BiConsumer<Integer, Annotation> consumer,AnnotatedElement annotatedEle,Predicate<Annotation> filter)` | 扫描Field上直接声明的注解，调用前需要确保调用#support(AnnotatedElement)返回为true |
| `cn.hutool.core.annotation.scanner.GenericAnnotationScanner` | `boolean support(AnnotatedElement annotatedEle)` | 通用注解扫描器支持扫描所有类型的AnnotatedElement |
| `cn.hutool.core.annotation.scanner.GenericAnnotationScanner` | `void scan(BiConsumer<Integer, Annotation> consumer,AnnotatedElement annotatedEle,Predicate<Annotation> filter)` | 扫描注解元素的层级结构（若存在），然后对获取到的注解和注解对应的层级索引进行处理 |
| `cn.hutool.core.annotation.scanner.MetaAnnotationScanner` | `List<Annotation> getAnnotations(AnnotatedElement annotatedEle)` | 获取注解元素上的全部注解。调用该方法前，需要确保调用#support(AnnotatedElement)返回为true |
| `cn.hutool.core.annotation.scanner.MetaAnnotationScanner` | `boolean support(AnnotatedElement annotatedEle)` | 判断是否支持扫描该注解元素，仅当注解元素是Annotation接口的子类Class时返回true |
| `cn.hutool.core.annotation.scanner.MetaAnnotationScanner` | `void scan(BiConsumer<Integer, Annotation> consumer,AnnotatedElement annotatedEle,Predicate<Annotation> filter)` | 按广度优先扫描指定注解上的元注解，对扫描到的注解与层级索引进行操作 |
| `cn.hutool.core.annotation.scanner.MethodAnnotationScanner` | `MethodAnnotationScanner setScanSameSignatureMethod(boolean scanSuperMethodIfOverride)` | 设置是否扫描类层级结构中具有相同方法签名的方法 |
| `cn.hutool.core.annotation.scanner.MethodAnnotationScanner` | `boolean support(AnnotatedElement annotatedEle)` | 判断是否支持扫描该注解元素，仅当注解元素是Method时返回true |
| `cn.hutool.core.annotation.scanner.TypeAnnotationScanner` | `TypeAnnotationScanner setIncludeInterfaces(boolean includeInterfaces)` | 是否允许扫描父接口 |
| `cn.hutool.core.annotation.scanner.TypeAnnotationScanner` | `TypeAnnotationScanner setIncludeSuperClass(boolean includeSuperClass)` | 是否允许扫描父类 |
| `cn.hutool.core.annotation.scanner.TypeAnnotationScanner` | `boolean support(AnnotatedElement annotatedEle)` | 判断是否支持扫描该注解元素，仅当注解元素是Class接时返回true |
| `cn.hutool.core.annotation.scanner.TypeAnnotationScanner$JdkProxyClassConverter` | `Class<?> apply(Class<?> sourceClass)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
