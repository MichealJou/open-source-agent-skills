# com.feilong.lib.digester3.binder

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.digester3.binder.AbstractNamespaceURIBasedRulesModule`

```java
public abstract class com.feilong.lib.digester3.binder.AbstractNamespaceURIBasedRulesModule extends com.feilong.lib.digester3.binder.AbstractRulesModule {
  public com.feilong.lib.digester3.binder.AbstractNamespaceURIBasedRulesModule(java.lang.String);
}
```

## `com.feilong.lib.digester3.binder.AbstractParamTypeBuilder`

```java
public abstract class com.feilong.lib.digester3.binder.AbstractParamTypeBuilder<R extends com.feilong.lib.digester3.AbstractMethodRule> extends com.feilong.lib.digester3.binder.AbstractBackToLinkedRuleBuilder<R> {
  public final com.feilong.lib.digester3.binder.AbstractParamTypeBuilder<R> withParameterType(java.lang.Class<?>);
  public final com.feilong.lib.digester3.binder.AbstractParamTypeBuilder<R> withParameterType(java.lang.String);
  public final com.feilong.lib.digester3.binder.AbstractParamTypeBuilder<R> useExactMatch(boolean);
  public final com.feilong.lib.digester3.binder.AbstractParamTypeBuilder<R> fireOnBegin(boolean);
}
```

## `com.feilong.lib.digester3.binder.AbstractRulesModule`

```java
public abstract class com.feilong.lib.digester3.binder.AbstractRulesModule implements com.feilong.lib.digester3.binder.RulesModule {
  public com.feilong.lib.digester3.binder.AbstractRulesModule();
  public final void configure(com.feilong.lib.digester3.binder.RulesBinder);
}
```

## `com.feilong.lib.digester3.binder.AddAliasBuilder`

```java
public final class com.feilong.lib.digester3.binder.AddAliasBuilder<B> {
  public B forProperty(java.lang.String);
}
```

## `com.feilong.lib.digester3.binder.BeanPropertySetterBuilder`

```java
public final class com.feilong.lib.digester3.binder.BeanPropertySetterBuilder extends com.feilong.lib.digester3.binder.AbstractBackToLinkedRuleBuilder<com.feilong.lib.digester3.BeanPropertySetterRule> {
  public com.feilong.lib.digester3.binder.BeanPropertySetterBuilder withName(java.lang.String);
  public com.feilong.lib.digester3.binder.BeanPropertySetterBuilder extractPropertyNameFromAttribute(java.lang.String);
}
```

## `com.feilong.lib.digester3.binder.CallMethodBuilder`

```java
public final class com.feilong.lib.digester3.binder.CallMethodBuilder extends com.feilong.lib.digester3.binder.AbstractBackToLinkedRuleBuilder<com.feilong.lib.digester3.CallMethodRule> {
  public com.feilong.lib.digester3.binder.CallMethodBuilder withTargetOffset(int);
  public com.feilong.lib.digester3.binder.CallMethodBuilder withParamTypes(java.lang.String...);
  public com.feilong.lib.digester3.binder.CallMethodBuilder withParamTypes(java.lang.Class<?>...);
  public com.feilong.lib.digester3.binder.CallMethodBuilder useExactMatch(boolean);
  public com.feilong.lib.digester3.binder.CallMethodBuilder withParamCount(int);
  public com.feilong.lib.digester3.binder.CallMethodBuilder usingElementBodyAsArgument();
}
```

## `com.feilong.lib.digester3.binder.CallParamBuilder`

```java
public final class com.feilong.lib.digester3.binder.CallParamBuilder extends com.feilong.lib.digester3.binder.AbstractBackToLinkedRuleBuilder<com.feilong.lib.digester3.CallParamRule> {
  public com.feilong.lib.digester3.binder.CallParamBuilder ofIndex(int);
  public com.feilong.lib.digester3.binder.CallParamBuilder fromAttribute(java.lang.String);
  public com.feilong.lib.digester3.binder.CallParamBuilder fromStack(boolean);
  public com.feilong.lib.digester3.binder.CallParamBuilder withStackIndex(int);
}
```

## `com.feilong.lib.digester3.binder.DigesterLoader`

```java
public final class com.feilong.lib.digester3.binder.DigesterLoader {
  public static com.feilong.lib.digester3.binder.DigesterLoader newLoader(com.feilong.lib.digester3.binder.RulesModule...);
  public com.feilong.lib.digester3.binder.DigesterLoader setNamespaceAware(boolean);
  public com.feilong.lib.digester3.binder.DigesterLoader setXIncludeAware(boolean);
  public com.feilong.lib.digester3.binder.DigesterLoader setValidating(boolean);
  public boolean isValidating();
  public com.feilong.lib.digester3.binder.DigesterLoader register(java.lang.String, java.lang.String);
  public com.feilong.lib.digester3.Digester newDigester();
  public void addRules(com.feilong.lib.digester3.Digester);
  public com.feilong.lib.digester3.RuleSet createRuleSet();
}
```

## `com.feilong.lib.digester3.binder.DigesterLoadingException`

```java
public final class com.feilong.lib.digester3.binder.DigesterLoadingException extends java.lang.RuntimeException {
  public com.feilong.lib.digester3.binder.DigesterLoadingException(java.lang.String, java.lang.Throwable);
  public com.feilong.lib.digester3.binder.DigesterLoadingException(java.lang.String);
  public com.feilong.lib.digester3.binder.DigesterLoadingException(java.lang.Throwable);
}
```

## `com.feilong.lib.digester3.binder.FactoryCreateBuilder`

```java
public final class com.feilong.lib.digester3.binder.FactoryCreateBuilder extends com.feilong.lib.digester3.binder.AbstractBackToLinkedRuleBuilder<com.feilong.lib.digester3.FactoryCreateRule> {
  public com.feilong.lib.digester3.binder.FactoryCreateBuilder ofType(java.lang.String);
  public com.feilong.lib.digester3.binder.FactoryCreateBuilder ofType(java.lang.Class<? extends com.feilong.lib.digester3.ObjectCreationFactory<?>>);
  public <T> com.feilong.lib.digester3.binder.FactoryCreateBuilder usingFactory(com.feilong.lib.digester3.ObjectCreationFactory<T>);
  public com.feilong.lib.digester3.binder.FactoryCreateBuilder overriddenByAttribute(java.lang.String);
  public com.feilong.lib.digester3.binder.FactoryCreateBuilder ignoreCreateExceptions(boolean);
}
```

## `com.feilong.lib.digester3.binder.LinkedRuleBuilder`

```java
public final class com.feilong.lib.digester3.binder.LinkedRuleBuilder {
  public com.feilong.lib.digester3.binder.BeanPropertySetterBuilder setBeanProperty();
  public com.feilong.lib.digester3.binder.CallMethodBuilder callMethod(java.lang.String);
  public com.feilong.lib.digester3.binder.CallParamBuilder callParam();
  public com.feilong.lib.digester3.binder.PathCallParamBuilder callParamPath();
  public com.feilong.lib.digester3.binder.FactoryCreateBuilder factoryCreate();
  public com.feilong.lib.digester3.binder.ObjectCreateBuilder createObject();
  public <T> com.feilong.lib.digester3.binder.ObjectParamBuilder<T> objectParam(T);
  public com.feilong.lib.digester3.binder.NestedPropertiesBuilder setNestedProperties();
  public com.feilong.lib.digester3.binder.SetNextBuilder setNext(java.lang.String);
  public com.feilong.lib.digester3.binder.SetPropertiesBuilder setProperties();
  public com.feilong.lib.digester3.binder.SetPropertyBuilder setProperty(java.lang.String);
  public com.feilong.lib.digester3.binder.SetRootBuilder setRoot(java.lang.String);
  public com.feilong.lib.digester3.binder.SetTopBuilder setTop(java.lang.String);
  public com.feilong.lib.digester3.binder.NodeCreateRuleProvider createNode();
  public <R extends com.feilong.lib.digester3.Rule> com.feilong.lib.digester3.binder.ByRuleBuilder<R> addRule(R);
  public <R extends com.feilong.lib.digester3.Rule> com.feilong.lib.digester3.binder.ByRuleProviderBuilder<R> addRuleCreatedBy(com.feilong.lib.digester3.binder.RuleProvider<R>);
  public com.feilong.lib.digester3.binder.LinkedRuleBuilder withNamespaceURI(java.lang.String);
}
```

## `com.feilong.lib.digester3.binder.NestedPropertiesBuilder`

```java
public final class com.feilong.lib.digester3.binder.NestedPropertiesBuilder extends com.feilong.lib.digester3.binder.AbstractBackToLinkedRuleBuilder<com.feilong.lib.digester3.SetNestedPropertiesRule> {
  public com.feilong.lib.digester3.binder.NestedPropertiesBuilder ignoreElement(java.lang.String);
  public com.feilong.lib.digester3.binder.AddAliasBuilder<com.feilong.lib.digester3.binder.NestedPropertiesBuilder> addAlias(java.lang.String);
  public com.feilong.lib.digester3.binder.NestedPropertiesBuilder trimData(boolean);
  public com.feilong.lib.digester3.binder.NestedPropertiesBuilder allowUnknownChildElements(boolean);
}
```

## `com.feilong.lib.digester3.binder.NodeCreateRuleProvider`

```java
public final class com.feilong.lib.digester3.binder.NodeCreateRuleProvider extends com.feilong.lib.digester3.binder.AbstractBackToLinkedRuleBuilder<com.feilong.lib.digester3.NodeCreateRule> {
  public com.feilong.lib.digester3.binder.NodeCreateRuleProvider ofType(com.feilong.lib.digester3.binder.NodeCreateRuleProvider$NodeType);
  public com.feilong.lib.digester3.binder.NodeCreateRuleProvider usingDocumentBuilder(javax.xml.parsers.DocumentBuilder);
}
```

## `com.feilong.lib.digester3.binder.NodeCreateRuleProvider$NodeType`

```java
public final class com.feilong.lib.digester3.binder.NodeCreateRuleProvider$NodeType extends java.lang.Enum<com.feilong.lib.digester3.binder.NodeCreateRuleProvider$NodeType> {
  public static com.feilong.lib.digester3.binder.NodeCreateRuleProvider$NodeType[] values();
  public static com.feilong.lib.digester3.binder.NodeCreateRuleProvider$NodeType valueOf(java.lang.String);
}
```

## `com.feilong.lib.digester3.binder.ObjectCreateBuilder`

```java
public final class com.feilong.lib.digester3.binder.ObjectCreateBuilder extends com.feilong.lib.digester3.binder.AbstractBackToLinkedRuleBuilder<com.feilong.lib.digester3.ObjectCreateRule> {
  public com.feilong.lib.digester3.binder.ObjectCreateBuilder ofType(java.lang.String);
  public <T> com.feilong.lib.digester3.binder.ObjectCreateBuilder ofType(java.lang.Class<T>);
  public com.feilong.lib.digester3.binder.ObjectCreateBuilder ofTypeSpecifiedByAttribute(java.lang.String);
  public com.feilong.lib.digester3.binder.ObjectCreateBuilder usingConstructor(java.lang.String...);
  public com.feilong.lib.digester3.binder.ObjectCreateBuilder usingConstructor(java.lang.Class<?>...);
}
```

## `com.feilong.lib.digester3.binder.ObjectParamBuilder`

```java
public final class com.feilong.lib.digester3.binder.ObjectParamBuilder<T> extends com.feilong.lib.digester3.binder.AbstractBackToLinkedRuleBuilder<com.feilong.lib.digester3.ObjectParamRule> {
  public com.feilong.lib.digester3.binder.ObjectParamBuilder<T> ofIndex(int);
  public com.feilong.lib.digester3.binder.ObjectParamBuilder<T> matchingAttribute(java.lang.String);
}
```

## `com.feilong.lib.digester3.binder.PathCallParamBuilder`

```java
public final class com.feilong.lib.digester3.binder.PathCallParamBuilder extends com.feilong.lib.digester3.binder.AbstractBackToLinkedRuleBuilder<com.feilong.lib.digester3.PathCallParamRule> {
  public com.feilong.lib.digester3.binder.PathCallParamBuilder ofIndex(int);
}
```

## `com.feilong.lib.digester3.binder.RuleProvider`

```java
public interface com.feilong.lib.digester3.binder.RuleProvider<R extends com.feilong.lib.digester3.Rule> {
  public abstract R get();
}
```

## `com.feilong.lib.digester3.binder.RulesBinder`

```java
public interface com.feilong.lib.digester3.binder.RulesBinder {
  public abstract java.lang.ClassLoader getContextClassLoader();
  public abstract void addError(java.lang.String, java.lang.Object...);
  public abstract void addError(java.lang.Throwable);
  public abstract void install(com.feilong.lib.digester3.binder.RulesModule);
  public abstract com.feilong.lib.digester3.binder.LinkedRuleBuilder forPattern(java.lang.String);
}
```

## `com.feilong.lib.digester3.binder.RulesModule`

```java
public interface com.feilong.lib.digester3.binder.RulesModule {
  public abstract void configure(com.feilong.lib.digester3.binder.RulesBinder);
}
```

## `com.feilong.lib.digester3.binder.SetPropertiesBuilder`

```java
public final class com.feilong.lib.digester3.binder.SetPropertiesBuilder extends com.feilong.lib.digester3.binder.AbstractBackToLinkedRuleBuilder<com.feilong.lib.digester3.SetPropertiesRule> {
  public com.feilong.lib.digester3.binder.AddAliasBuilder<com.feilong.lib.digester3.binder.SetPropertiesBuilder> addAlias(java.lang.String);
  public com.feilong.lib.digester3.binder.SetPropertiesBuilder ignoreAttribute(java.lang.String);
  public com.feilong.lib.digester3.binder.SetPropertiesBuilder ignoreMissingProperty(boolean);
}
```

## `com.feilong.lib.digester3.binder.SetPropertyBuilder`

```java
public final class com.feilong.lib.digester3.binder.SetPropertyBuilder extends com.feilong.lib.digester3.binder.AbstractBackToLinkedRuleBuilder<com.feilong.lib.digester3.SetPropertyRule> {
  public com.feilong.lib.digester3.binder.SetPropertyBuilder extractingValueFromAttribute(java.lang.String);
}
```
