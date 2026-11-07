# cn.hutool.core.annotation

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.annotation.AbstractAnnotationSynthesizer` | `A synthesize(Class<A> annotationType)` | 获取合成注解 |
| `cn.hutool.core.annotation.AbstractAnnotationSynthesizer` | `Collection<SynthesizedAnnotationPostProcessor> getAnnotationPostProcessors()` | 获取合成注解后置处理器 |
| `cn.hutool.core.annotation.AbstractAnnotationSynthesizer` | `Map<Class<? extends Annotation>, SynthesizedAnnotation> getAllSynthesizedAnnotation()` | 获取全部的合成注解 |
| `cn.hutool.core.annotation.AbstractAnnotationSynthesizer` | `SynthesizedAnnotation getSynthesizedAnnotation(Class<?> annotationType)` | 获取已合成的注解 |
| `cn.hutool.core.annotation.AbstractAnnotationSynthesizer` | `SynthesizedAnnotationSelector getAnnotationSelector()` | 合成注解选择器 |
| `cn.hutool.core.annotation.AbstractAnnotationSynthesizer` | `T getSource()` | 获取合成注解来源最初来源 |
| `cn.hutool.core.annotation.AbstractLinkAnnotationPostProcessor` | `void process(SynthesizedAnnotation synthesizedAnnotation,AnnotationSynthesizer synthesizer)` | 若一个注解属性上存在Link注解，注解的Link#type()返回值在#processTypes()中存在， 且此Link指定的注解对象在当前的SynthesizedAggregateAnnotation中存在， 则从聚合器中获取类型对应的合成注解对象，与该对象中的指定属性，然后将全部关联数据交给 #processLinkedAttribute处理。 |
| `cn.hutool.core.annotation.AbstractWrappedAnnotationAttribute` | `AnnotationAttribute getLinked()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.AbstractWrappedAnnotationAttribute` | `AnnotationAttribute getNonWrappedOriginal()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.AbstractWrappedAnnotationAttribute` | `AnnotationAttribute getOriginal()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.AbstractWrappedAnnotationAttribute` | `Collection<AnnotationAttribute> getAllLinkedNonWrappedAttributes()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.AggregateAnnotation` | `Annotation[] getAnnotations()` | 获取聚合中的全部注解对象 |
| `cn.hutool.core.annotation.AggregateAnnotation` | `boolean isAnnotationPresent(Class<? extends Annotation> annotationType)` | 在聚合中是否存在的指定类型注解对象 |
| `cn.hutool.core.annotation.Alias` | `String value()` | 别名值，即使用此注解要替换成的别名名称 |
| `cn.hutool.core.annotation.AliasAnnotationPostProcessor` | `int order()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.AliasAnnotationPostProcessor` | `void process(SynthesizedAnnotation synthesizedAnnotation,AnnotationSynthesizer synthesizer)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.AliasFor` | `Class<? extends Annotation> annotation()` | 产生关联的注解类型，当不指定时，默认指注释的属性所在的类 |
| `cn.hutool.core.annotation.AliasFor` | `String attribute()` | #annotation()指定注解中关联的属性 |
| `cn.hutool.core.annotation.AliasLinkAnnotationPostProcessor` | `int order()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.AliasedAnnotationAttribute` | `Object getValue()` | 若#linked为默认值，则返回#original的值，否则返回#linked的值 |
| `cn.hutool.core.annotation.AliasedAnnotationAttribute` | `boolean isValueEquivalentToDefaultValue()` | 当#original与#linked都为默认值时返回true |
| `cn.hutool.core.annotation.AnnotationAttribute` | `Annotation getAnnotation()` | 获取注解对象 |
| `cn.hutool.core.annotation.AnnotationAttribute` | `Class<?> getAnnotationType()` | 获取声明属性的注解类 |
| `cn.hutool.core.annotation.AnnotationAttribute` | `Class<?> getAttributeType()` | 获取属性类型 |
| `cn.hutool.core.annotation.AnnotationAttribute` | `Method getAttribute()` | 获取注解属性对应的方法 |
| `cn.hutool.core.annotation.AnnotationAttribute` | `Object getValue()` | 获取注解属性 |
| `cn.hutool.core.annotation.AnnotationAttribute` | `String getAttributeName()` | 获取属性名称 |
| `cn.hutool.core.annotation.AnnotationAttribute` | `T getAnnotation(Class<T> annotationType)` | 获取属性上的注解 |
| `cn.hutool.core.annotation.AnnotationAttribute` | `boolean isValueEquivalentToDefaultValue()` | 该注解属性的值是否等于默认值 |
| `cn.hutool.core.annotation.AnnotationAttribute` | `boolean isWrapped()` | 当前注解属性是否已经被WrappedAnnotationAttribute包装 |
| `cn.hutool.core.annotation.AnnotationAttributeValueProvider` | `Object getAttributeValue(String attributeName,Class<?> attributeType)` | 获取注解属性值 |
| `cn.hutool.core.annotation.AnnotationProxy` | `Class<? extends Annotation> annotationType()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.AnnotationProxy` | `Object invoke(Object proxy,Method method,Object[] args)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.AnnotationSynthesizer` | `Collection<SynthesizedAnnotationPostProcessor> getAnnotationPostProcessors()` | 获取合成注解后置处理器 |
| `cn.hutool.core.annotation.AnnotationSynthesizer` | `Map<Class<? extends Annotation>, SynthesizedAnnotation> getAllSynthesizedAnnotation()` | 获取全部的合成注解 |
| `cn.hutool.core.annotation.AnnotationSynthesizer` | `Object getSource()` | 获取合成注解来源最初来源 |
| `cn.hutool.core.annotation.AnnotationSynthesizer` | `SynthesizedAnnotation getSynthesizedAnnotation(Class<?> annotationType)` | 获取已合成的注解 |
| `cn.hutool.core.annotation.AnnotationSynthesizer` | `SynthesizedAnnotationSelector getAnnotationSelector()` | 合成注解选择器 |
| `cn.hutool.core.annotation.AnnotationSynthesizer` | `T synthesize(Class<T> annotationType)` | 获取合成注解 |
| `cn.hutool.core.annotation.AnnotationUtil` | `A getAnnotation(AnnotatedElement annotationEle,Class<A> annotationType)` | 获取指定注解（优化版：新增L1缓存，提升高频调用性能） 支持获取直接注解、元注解、组合注解，行为与原生实现完全一致 |
| `cn.hutool.core.annotation.AnnotationUtil` | `Annotation[] getAnnotations(AnnotatedElement annotationEle,boolean isToCombination)` | 获取指定注解 |
| `cn.hutool.core.annotation.AnnotationUtil` | `Annotation[] getAnnotations(AnnotatedElement annotationEle,boolean isToCombination,Predicate<Annotation> predicate)` | 获取指定注解 |
| `cn.hutool.core.annotation.AnnotationUtil` | `CombinationAnnotationElement toCombination(AnnotatedElement annotationEle)` | 将指定的被注解的元素转换为组合注解元素 |
| `cn.hutool.core.annotation.AnnotationUtil` | `ElementType[] getTargetType(Class<? extends Annotation> annotationType)` | 获取注解类可以用来修饰哪些程序元素，如 TYPE, METHOD, CONSTRUCTOR, FIELD, PARAMETER 等 |
| `cn.hutool.core.annotation.AnnotationUtil` | `List<Annotation> scanClass(Class<?> targetClass)` | 扫描类以及类的Class层级结构中的注解，将返回除了#META_ANNOTATIONS中指定的JDK默认元注解外, 全部类/接口的Class#getAnnotations()方法返回的注解对象。 层级结构将按广度优先递归，遵循规则如下： 同一层级中，优先处理父类，然后再处理父接口； 同一个接口在不同层级出现，优先选择层级距离targetClass更近的接口； 同一个接口在相同层级出现，优先选择其子类/子接口被先解析的那个； 注解根据其声明类/接口被扫描的顺序排序，若注解都在同一个Class中被声明，则还会遵循Class#getAnnotations()的顺序。 比如： 若targetClass… |
| `cn.hutool.core.annotation.AnnotationUtil` | `List<Annotation> scanMetaAnnotation(Class<? extends Annotation> annotationType)` | 扫描注解类，以及注解类的Class层级结构中的注解，将返回除了#META_ANNOTATIONS中指定的JDK默认注解外， 按元注解对象与annotationType的距离和Class#getAnnotations()顺序排序的注解对象集合 比如： 若annotationType为 A，且A存在元注解B，B又存在元注解C和D，则有： |
| `cn.hutool.core.annotation.AnnotationUtil` | `List<Annotation> scanMethod(Method method)` | 扫描方法，以及该方法所在类的Class层级结构中的具有相同方法签名的方法， 将返回除了#META_ANNOTATIONS中指定的JDK默认元注解外, 全部匹配方法上Method#getAnnotations()方法返回的注解对象。 方法所在类的层级结构将按广度优先递归，遵循规则如下： 同一层级中，优先处理父类，然后再处理父接口； 同一个接口在不同层级出现，优先选择层级距离targetClass更近的接口； 同一个接口在相同层级出现，优先选择其子类/子接口被先解析的那个； 方法上的注解根据方法的声明类/接口被扫描的顺序排序，若注解都在同一个类的同一个方法中被声明，则还会遵循Method#getA… |
| `cn.hutool.core.annotation.AnnotationUtil` | `List<T> getAllSynthesizedAnnotations(AnnotatedElement annotatedEle,Class<T> annotationType)` | 获取元素上所有指定注解 若元素是类，则递归解析全部父类和全部父接口上的注解; 若元素是方法、属性或注解，则只解析其直接声明的注解; 注解合成规则如下： 若AnnotatedEle按顺序从上到下声明了A，B，C三个注解，且三注解存在元注解如下： |
| `cn.hutool.core.annotation.AnnotationUtil` | `Map<String, Object> getAnnotationValueMap(AnnotatedElement annotationEle,Class<? extends Annotation> annotationType)` | 获取指定注解中所有属性值 如果无指定的属性方法返回null |
| `cn.hutool.core.annotation.AnnotationUtil` | `R getAnnotationValue(AnnotatedElement annotationEle,Func1<A, R> propertyName)` | 获取指定注解属性的值 如果无指定的属性方法返回null |
| `cn.hutool.core.annotation.AnnotationUtil` | `RetentionPolicy getRetentionPolicy(Class<? extends Annotation> annotationType)` | 获取注解类的保留时间，可选值 SOURCE（源码时），CLASS（编译时），RUNTIME（运行时），默认为 CLASS |
| `cn.hutool.core.annotation.AnnotationUtil` | `SynthesizedAggregateAnnotation aggregatingFromAnnotation(Annotation... annotations)` | 对指定注解对象进行聚合 |
| `cn.hutool.core.annotation.AnnotationUtil` | `SynthesizedAggregateAnnotation aggregatingFromAnnotationWithMeta(Annotation... annotations)` | 对指定注解对象及其元注解进行聚合 |
| `cn.hutool.core.annotation.AnnotationUtil` | `T getAnnotationAlias(AnnotatedElement annotationEle,Class<T> annotationType)` | 获取别名支持后的注解（优化版：新增L2缓存，提升高频别名解析性能） |
| `cn.hutool.core.annotation.AnnotationUtil` | `T getAnnotationValue(AnnotatedElement annotationEle,Class<? extends Annotation> annotationType)` | 获取指定注解默认值 如果无指定的属性方法返回null |
| `cn.hutool.core.annotation.AnnotationUtil` | `T getAnnotationValue(AnnotatedElement annotationEle,Class<? extends Annotation> annotationType,String propertyName)` | 获取指定注解属性的值 如果无指定的属性方法返回null |
| `cn.hutool.core.annotation.AnnotationUtil` | `T getSynthesizedAnnotation(AnnotatedElement annotatedEle,Class<T> annotationType)` | 获取元素上距离指定元素最接近的合成注解（优化版：新增L2缓存，避免重复合成解析） 若元素是类，则递归解析全部父类和全部父接口上的注解; 若元素是方法、属性或注解，则只解析其直接声明的注解; 注解合成规则如下： 若AnnotatedEle按顺序从上到下声明了A，B，C三个注解，且三注解存在元注解如下： |
| `cn.hutool.core.annotation.AnnotationUtil` | `T getSynthesizedAnnotation(Class<T> annotationType,Annotation... annotations)` | 将指定注解实例与其元注解转为合成注解 |
| `cn.hutool.core.annotation.AnnotationUtil` | `T[] getAnnotations(AnnotatedElement annotationEle,boolean isToCombination,Class<T> annotationType)` | 获取指定注解 |
| `cn.hutool.core.annotation.AnnotationUtil` | `T[] getCombinationAnnotations(AnnotatedElement annotationEle,Class<T> annotationType)` | 获取组合注解 |
| `cn.hutool.core.annotation.AnnotationUtil` | `boolean hasAnnotation(AnnotatedElement annotationEle,Class<? extends Annotation> annotationType)` | 检查是否包含指定注解指定注解 |
| `cn.hutool.core.annotation.AnnotationUtil` | `boolean hasAnnotation(final AnnotatedElement annotationEle,final String annotationTypeName)` | 检查是否包含指定注解 注解类传入全名，通过Class#forName(String)加载，避免不存在的注解导致的ClassNotFoundException |
| `cn.hutool.core.annotation.AnnotationUtil` | `boolean isDocumented(Class<? extends Annotation> annotationType)` | 是否会保存到 Javadoc 文档中 |
| `cn.hutool.core.annotation.AnnotationUtil` | `boolean isInherited(Class<? extends Annotation> annotationType)` | 是否可以被继承，默认为 false |
| `cn.hutool.core.annotation.AnnotationUtil` | `boolean isJdkMetaAnnotation(Class<? extends Annotation> annotationType)` | 是否为Jdk自带的元注解。 包括： Target Retention Inherited Documented SuppressWarnings Override Deprecated |
| `cn.hutool.core.annotation.AnnotationUtil` | `boolean isNotJdkMateAnnotation(Class<? extends Annotation> annotationType)` | 是否不为Jdk自带的元注解。 包括： Target Retention Inherited Documented SuppressWarnings Override Deprecated |
| `cn.hutool.core.annotation.AnnotationUtil` | `boolean isSynthesizedAnnotation(Annotation annotation)` | 该注解对象是否为通过代理类生成的合成注解 |
| `cn.hutool.core.annotation.AnnotationUtil` | `void setValue(Annotation annotation,String annotationField,Object value)` | 设置新的注解的属性（字段）值 |
| `cn.hutool.core.annotation.CacheableAnnotationAttribute` | `Annotation getAnnotation()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.CacheableAnnotationAttribute` | `Method getAttribute()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.CacheableAnnotationAttribute` | `Object getValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.CacheableAnnotationAttribute` | `boolean isValueEquivalentToDefaultValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.CacheableSynthesizedAnnotationAttributeProcessor` | `T getAttributeValue(String attributeName,Class<T> attributeType,Collection<? extends SynthesizedAnnotation> synthesizedAnnotations)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.CombinationAnnotationElement` | `Annotation[] getAnnotations()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.CombinationAnnotationElement` | `Annotation[] getDeclaredAnnotations()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.CombinationAnnotationElement` | `CombinationAnnotationElement of(AnnotatedElement element,Predicate<Annotation> predicate)` | 创建CombinationAnnotationElement |
| `cn.hutool.core.annotation.CombinationAnnotationElement` | `T getAnnotation(Class<T> annotationClass)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.CombinationAnnotationElement` | `boolean isAnnotationPresent(Class<? extends Annotation> annotationClass)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.ForceAliasFor` | `Class<? extends Annotation> annotation()` | 产生关联的注解类型，当不指定时，默认指注释的属性所在的类 |
| `cn.hutool.core.annotation.ForceAliasFor` | `String attribute()` | #annotation()指定注解中关联的属性 |
| `cn.hutool.core.annotation.ForceAliasedAnnotationAttribute` | `Class<?> getAttributeType()` | 总是返回#linked的AnnotationAttribute#getAttributeType()的返回值 |
| `cn.hutool.core.annotation.ForceAliasedAnnotationAttribute` | `Object getValue()` | 总是返回#linked的AnnotationAttribute#getValue()的返回值 |
| `cn.hutool.core.annotation.ForceAliasedAnnotationAttribute` | `boolean isValueEquivalentToDefaultValue()` | 总是返回#linked的AnnotationAttribute#isValueEquivalentToDefaultValue()的返回值 |
| `cn.hutool.core.annotation.GenericSynthesizedAggregateAnnotation` | `Annotation[] getAnnotations()` | 获取合成注解中包含的全部注解 |
| `cn.hutool.core.annotation.GenericSynthesizedAggregateAnnotation` | `Object getAttributeValue(String attributeName,Class<?> attributeType)` | 根据指定的属性名与属性类型获取对应的属性值，若存在Alias则获取Alias#value()指定的别名属性的值 当不同层级的注解之间存在同名同类型属性时，将优先获取更接近根注解的属性 |
| `cn.hutool.core.annotation.GenericSynthesizedAggregateAnnotation` | `Object getRoot()` | 获取根对象 |
| `cn.hutool.core.annotation.GenericSynthesizedAggregateAnnotation` | `SynthesizedAnnotationAttributeProcessor getAnnotationAttributeProcessor()` | 获取合成注解属性处理器 |
| `cn.hutool.core.annotation.GenericSynthesizedAggregateAnnotation` | `T getAnnotation(Class<T> annotationType)` | 获取合成注解中包含的指定注解 |
| `cn.hutool.core.annotation.GenericSynthesizedAggregateAnnotation` | `T synthesize(Class<T> annotationType,SynthesizedAnnotation annotation)` | 若合成注解在存在指定元注解，则使用动态代理生成一个对应的注解实例 |
| `cn.hutool.core.annotation.GenericSynthesizedAggregateAnnotation` | `boolean isAnnotationPresent(Class<? extends Annotation> annotationType)` | 当前合成注解中是否存在指定元注解 |
| `cn.hutool.core.annotation.GenericSynthesizedAggregateAnnotation` | `int getHorizontalDistance()` | 获取与根对象的水平距离 |
| `cn.hutool.core.annotation.GenericSynthesizedAggregateAnnotation` | `int getVerticalDistance()` | 获取与根对象的垂直距离 |
| `cn.hutool.core.annotation.GenericSynthesizedAnnotation` | `Class<? extends Annotation> annotationType()` | 获取被合成的注解类型 |
| `cn.hutool.core.annotation.GenericSynthesizedAnnotation` | `Map<String, AnnotationAttribute> getAttributes()` | 获取该注解的全部属性 |
| `cn.hutool.core.annotation.GenericSynthesizedAnnotation` | `Object getAttributeValue(String attributeName)` | 获取属性值 |
| `cn.hutool.core.annotation.GenericSynthesizedAnnotation` | `Object getAttributeValue(String attributeName,Class<?> attributeType)` | 获取注解属性值 |
| `cn.hutool.core.annotation.GenericSynthesizedAnnotation` | `R getRoot()` | 获取该合成注解对应的根节点 |
| `cn.hutool.core.annotation.GenericSynthesizedAnnotation` | `T getAnnotation()` | 获取被合成的注解对象 |
| `cn.hutool.core.annotation.GenericSynthesizedAnnotation` | `boolean hasAttribute(String attributeName)` | 元注解是否存在该属性 |
| `cn.hutool.core.annotation.GenericSynthesizedAnnotation` | `boolean hasAttribute(String attributeName,Class<?> returnType)` | 元注解是否存在该属性，且该属性的值类型是指定类型或其子类 |
| `cn.hutool.core.annotation.GenericSynthesizedAnnotation` | `int getHorizontalDistance()` | 获取该合成注解与根对象的水平距离。 默认情况下，该距离即为当前注解与根对象之间相隔的已经被扫描到的注解数。 |
| `cn.hutool.core.annotation.GenericSynthesizedAnnotation` | `int getVerticalDistance()` | 获取该合成注解与根对象的垂直距离。 默认情况下，该距离即为当前注解与根对象之间相隔的层级数。 |
| `cn.hutool.core.annotation.GenericSynthesizedAnnotation` | `void replaceAttribute(String attributeName,UnaryOperator<AnnotationAttribute> operator)` | 替换属性值 |
| `cn.hutool.core.annotation.GenericSynthesizedAnnotation` | `void setAttribute(String attributeName,AnnotationAttribute attribute)` | 设置属性值 |
| `cn.hutool.core.annotation.Hierarchical` | `Object getRoot()` | 参照物，即坐标为(0, 0)的对象。 当对象本身即为参照物时，该方法应当返回其本身 |
| `cn.hutool.core.annotation.Hierarchical` | `int compareTo(Hierarchical o)` | 按#getVerticalDistance()和#getHorizontalDistance()排序 |
| `cn.hutool.core.annotation.Hierarchical` | `int getHorizontalDistance()` | 获取该对象与参照物的水平距离。 默认情况下，该距离即为当前对象在与参照物#getVerticalDistance()相同的情况下条， 该对象被扫描到的顺序。 |
| `cn.hutool.core.annotation.Hierarchical` | `int getVerticalDistance()` | 获取该对象与参照物的垂直距离。 默认情况下，该距离即为当前对象与参照物之间相隔的层级数。 |
| `cn.hutool.core.annotation.Hierarchical$Selector` | `T choose(T prev,T next)` | 比较两个被合成的对象，选择其中的一个并返回 |
| `cn.hutool.core.annotation.Hierarchical$Selector$FarthestAndNewestPrioritySelector` | `T choose(T oldAnnotation,T newAnnotation)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.Hierarchical$Selector$FarthestAndOldestPrioritySelector` | `T choose(T oldAnnotation,T newAnnotation)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.Hierarchical$Selector$NearestAndNewestPrioritySelector` | `T choose(T oldAnnotation,T newAnnotation)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.Hierarchical$Selector$NearestAndOldestPrioritySelector` | `T choose(T oldAnnotation,T newAnnotation)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.Link` | `Class<? extends Annotation> annotation()` | 产生关联的注解类型，当不指定时，默认指注释的属性所在的类 |
| `cn.hutool.core.annotation.Link` | `RelationType type()` | #attribute()指定属性与当前注解的属性建的关联关系类型 |
| `cn.hutool.core.annotation.Link` | `String attribute()` | #annotation()指定注解中关联的属性 |
| `cn.hutool.core.annotation.MirrorFor` | `Class<? extends Annotation> annotation()` | 产生关联的注解类型，当不指定时，默认指注释的属性所在的类 |
| `cn.hutool.core.annotation.MirrorFor` | `String attribute()` | #annotation()指定注解中关联的属性 |
| `cn.hutool.core.annotation.MirrorLinkAnnotationPostProcessor` | `int order()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.MirroredAnnotationAttribute` | `Object getValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.MirroredAnnotationAttribute` | `boolean isValueEquivalentToDefaultValue()` | 当#original与#linked都为默认值时返回true |
| `cn.hutool.core.annotation.SynthesizedAggregateAnnotation` | `Class<? extends Annotation> annotationType()` | 获取当前的注解类型 |
| `cn.hutool.core.annotation.SynthesizedAggregateAnnotation` | `Object getAttributeValue(String attributeName,Class<?> attributeType)` | 从聚合中获取指定类型的属性值 |
| `cn.hutool.core.annotation.SynthesizedAggregateAnnotation` | `SynthesizedAnnotationAttributeProcessor getAnnotationAttributeProcessor()` | 获取合成注解属性处理器 |
| `cn.hutool.core.annotation.SynthesizedAggregateAnnotation` | `T getAnnotation(Class<T> annotationType)` | 获取在聚合中存在的指定注解对象 |
| `cn.hutool.core.annotation.SynthesizedAggregateAnnotation` | `int getHorizontalDistance()` | 距离#getRoot()返回值的水平距离， 默认聚合注解即为根对象，因此返回0 |
| `cn.hutool.core.annotation.SynthesizedAggregateAnnotation` | `int getVerticalDistance()` | 距离#getRoot()返回值的垂直距离， 默认聚合注解即为根对象，因此返回0 |
| `cn.hutool.core.annotation.SynthesizedAnnotation` | `Annotation getAnnotation()` | 获取被合成的注解对象 |
| `cn.hutool.core.annotation.SynthesizedAnnotation` | `Map<String, AnnotationAttribute> getAttributes()` | 获取该注解的全部属性 |
| `cn.hutool.core.annotation.SynthesizedAnnotation` | `Object getAttributeValue(String attributeName)` | 获取属性值 |
| `cn.hutool.core.annotation.SynthesizedAnnotation` | `boolean hasAttribute(String attributeName,Class<?> returnType)` | 注解是否存在该名称相同，且类型一致的属性 |
| `cn.hutool.core.annotation.SynthesizedAnnotation` | `int getHorizontalDistance()` | 获取该合成注解与根对象的水平距离。 默认情况下，该距离即为当前注解与根对象之间相隔的已经被扫描到的注解数。 |
| `cn.hutool.core.annotation.SynthesizedAnnotation` | `int getVerticalDistance()` | 获取该合成注解与根对象的垂直距离。 默认情况下，该距离即为当前注解与根对象之间相隔的层级数。 |
| `cn.hutool.core.annotation.SynthesizedAnnotation` | `void replaceAttribute(String attributeName,UnaryOperator<AnnotationAttribute> operator)` | 替换属性值 |
| `cn.hutool.core.annotation.SynthesizedAnnotation` | `void setAttribute(String attributeName,AnnotationAttribute attribute)` | 设置属性值 |
| `cn.hutool.core.annotation.SynthesizedAnnotation` | `void setAttributes(Map<String, AnnotationAttribute> attributes)` | 设置该注解的全部属性 |
| `cn.hutool.core.annotation.SynthesizedAnnotationAttributeProcessor` | `R getAttributeValue(String attributeName,Class<R> attributeType,Collection<? extends SynthesizedAnnotation> synthesizedAnnotations)` | 从一批被合成注解中，获取指定名称与类型的属性值 |
| `cn.hutool.core.annotation.SynthesizedAnnotationPostProcessor` | `int compareTo(SynthesizedAnnotationPostProcessor o)` | 比较两个后置处理器的#order()返回值 |
| `cn.hutool.core.annotation.SynthesizedAnnotationPostProcessor` | `int order()` | 在一组后置处理器中被调用的顺序，越小越靠前 |
| `cn.hutool.core.annotation.SynthesizedAnnotationPostProcessor` | `void process(SynthesizedAnnotation synthesizedAnnotation,AnnotationSynthesizer synthesizer)` | 给定指定被合成注解与其所属的合成注解聚合器实例，经过处理后返回最终 |
| `cn.hutool.core.annotation.SynthesizedAnnotationProxy` | `Object invoke(Object proxy,Method method,Object[] args)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.SynthesizedAnnotationProxy` | `T create(Class<T> annotationType,AnnotationAttributeValueProvider annotationAttributeValueProvider,SynthesizedAnnotation annotation)` | 创建一个代理注解，生成的代理对象将是SyntheticProxyAnnotation与指定的注解类的子类。 |
| `cn.hutool.core.annotation.SynthesizedAnnotationProxy` | `T create(Class<T> annotationType,SynthesizedAnnotation annotation)` | 创建一个代理注解，生成的代理对象将是SyntheticProxyAnnotation与指定的注解类的子类。 |
| `cn.hutool.core.annotation.SynthesizedAnnotationProxy` | `boolean isProxyAnnotation(Class<?> annotationType)` | 该类是否为通过SynthesizedAnnotationProxy生成的代理类 |
| `cn.hutool.core.annotation.SynthesizedAnnotationSelector` | `T choose(T oldAnnotation,T newAnnotation)` | 比较两个被合成的注解，选择其中的一个并返回 |
| `cn.hutool.core.annotation.SynthesizedAnnotationSelector$FarthestAndNewestPrioritySelector` | `T choose(T oldAnnotation,T newAnnotation)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.SynthesizedAnnotationSelector$FarthestAndOldestPrioritySelector` | `T choose(T oldAnnotation,T newAnnotation)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.SynthesizedAnnotationSelector$NearestAndNewestPrioritySelector` | `T choose(T oldAnnotation,T newAnnotation)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.SynthesizedAnnotationSelector$NearestAndOldestPrioritySelector` | `T choose(T oldAnnotation,T newAnnotation)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.annotation.WrappedAnnotationAttribute` | `Annotation getAnnotation()` | 获取注解对象 |
| `cn.hutool.core.annotation.WrappedAnnotationAttribute` | `AnnotationAttribute getLinked()` | 获取包装#getOriginal()的AnnotationAttribute对象，该对象也可能是AnnotationAttribute |
| `cn.hutool.core.annotation.WrappedAnnotationAttribute` | `AnnotationAttribute getNonWrappedOriginal()` | 获取最初的被包装的AnnotationAttribute |
| `cn.hutool.core.annotation.WrappedAnnotationAttribute` | `AnnotationAttribute getOriginal()` | 获取被包装的AnnotationAttribute对象，该对象也可能是AnnotationAttribute |
| `cn.hutool.core.annotation.WrappedAnnotationAttribute` | `Class<?> getAttributeType()` | 获取属性类型 |
| `cn.hutool.core.annotation.WrappedAnnotationAttribute` | `Collection<AnnotationAttribute> getAllLinkedNonWrappedAttributes()` | 遍历以当前实例为根节点的树结构，获取所有未被包装的属性 |
| `cn.hutool.core.annotation.WrappedAnnotationAttribute` | `Method getAttribute()` | 获取注解属性对应的方法 |
| `cn.hutool.core.annotation.WrappedAnnotationAttribute` | `T getAnnotation(Class<T> annotationType)` | 获取属性上的注解 |
| `cn.hutool.core.annotation.WrappedAnnotationAttribute` | `boolean isValueEquivalentToDefaultValue()` | 该注解属性的值是否等于默认值 默认仅当#getOriginal()与#getLinked()返回的注解属性 都为默认值时，才返回true |
| `cn.hutool.core.annotation.WrappedAnnotationAttribute` | `boolean isWrapped()` | 当前注解属性是否已经被WrappedAnnotationAttribute包装 |
