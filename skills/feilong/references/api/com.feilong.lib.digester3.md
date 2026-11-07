# com.feilong.lib.digester3

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.digester3.AbstractMethodRule`

```java
public abstract class com.feilong.lib.digester3.AbstractMethodRule extends com.feilong.lib.digester3.Rule {
  public com.feilong.lib.digester3.AbstractMethodRule(java.lang.String);
  public com.feilong.lib.digester3.AbstractMethodRule(java.lang.String, java.lang.Class<?>);
  public com.feilong.lib.digester3.AbstractMethodRule(java.lang.String, java.lang.String);
  public boolean isExactMatch();
  public void setFireOnBegin(boolean);
  public boolean isFireOnBegin();
  public void setExactMatch(boolean);
  public void begin(java.lang.String, java.lang.String, org.xml.sax.Attributes) throws java.lang.Exception;
  public void end(java.lang.String, java.lang.String) throws java.lang.Exception;
  public final java.lang.String toString();
}
```

## `com.feilong.lib.digester3.AbstractObjectCreationFactory`

```java
public abstract class com.feilong.lib.digester3.AbstractObjectCreationFactory<T> implements com.feilong.lib.digester3.ObjectCreationFactory<T> {
  public com.feilong.lib.digester3.AbstractObjectCreationFactory();
  public abstract T createObject(org.xml.sax.Attributes) throws java.lang.Exception;
  public com.feilong.lib.digester3.Digester getDigester();
  public void setDigester(com.feilong.lib.digester3.Digester);
}
```

## `com.feilong.lib.digester3.AbstractRulesImpl`

```java
public abstract class com.feilong.lib.digester3.AbstractRulesImpl implements com.feilong.lib.digester3.Rules {
  public com.feilong.lib.digester3.AbstractRulesImpl();
  public com.feilong.lib.digester3.Digester getDigester();
  public void setDigester(com.feilong.lib.digester3.Digester);
  public java.lang.String getNamespaceURI();
  public void setNamespaceURI(java.lang.String);
  public final void add(java.lang.String, com.feilong.lib.digester3.Rule);
}
```

## `com.feilong.lib.digester3.BeanPropertySetterRule`

```java
public class com.feilong.lib.digester3.BeanPropertySetterRule extends com.feilong.lib.digester3.Rule {
  public com.feilong.lib.digester3.BeanPropertySetterRule(java.lang.String);
  public com.feilong.lib.digester3.BeanPropertySetterRule();
  public java.lang.String getPropertyName();
  public void setPropertyNameFromAttribute(java.lang.String);
  public void begin(java.lang.String, java.lang.String, org.xml.sax.Attributes) throws java.lang.Exception;
  public void body(java.lang.String, java.lang.String, java.lang.String) throws java.lang.Exception;
  public void end(java.lang.String, java.lang.String) throws java.lang.Exception;
  public void finish() throws java.lang.Exception;
  public java.lang.String toString();
}
```

## `com.feilong.lib.digester3.CallMethodRule`

```java
public class com.feilong.lib.digester3.CallMethodRule extends com.feilong.lib.digester3.Rule {
  public com.feilong.lib.digester3.CallMethodRule(java.lang.String, int);
  public com.feilong.lib.digester3.CallMethodRule(int, java.lang.String, int);
  public com.feilong.lib.digester3.CallMethodRule(java.lang.String);
  public com.feilong.lib.digester3.CallMethodRule(int, java.lang.String);
  public com.feilong.lib.digester3.CallMethodRule(java.lang.String, int, java.lang.String[]);
  public com.feilong.lib.digester3.CallMethodRule(int, java.lang.String, int, java.lang.String[]);
  public com.feilong.lib.digester3.CallMethodRule(java.lang.String, int, java.lang.Class<?>[]);
  public com.feilong.lib.digester3.CallMethodRule(int, java.lang.String, int, java.lang.Class<?>[]);
  public boolean getUseExactMatch();
  public void setUseExactMatch(boolean);
  public void setDigester(com.feilong.lib.digester3.Digester);
  public void begin(java.lang.String, java.lang.String, org.xml.sax.Attributes) throws java.lang.Exception;
  public void body(java.lang.String, java.lang.String, java.lang.String) throws java.lang.Exception;
  public void end(java.lang.String, java.lang.String) throws java.lang.Exception;
  public void finish() throws java.lang.Exception;
  public java.lang.String toString();
}
```

## `com.feilong.lib.digester3.CallParamRule`

```java
public class com.feilong.lib.digester3.CallParamRule extends com.feilong.lib.digester3.Rule {
  public com.feilong.lib.digester3.CallParamRule(int);
  public com.feilong.lib.digester3.CallParamRule(int, java.lang.String);
  public com.feilong.lib.digester3.CallParamRule(int, boolean);
  public com.feilong.lib.digester3.CallParamRule(int, int);
  public void setAttributeName(java.lang.String);
  public void begin(java.lang.String, java.lang.String, org.xml.sax.Attributes) throws java.lang.Exception;
  public void body(java.lang.String, java.lang.String, java.lang.String) throws java.lang.Exception;
  public void end(java.lang.String, java.lang.String);
  public java.lang.String toString();
}
```

## `com.feilong.lib.digester3.Digester`

```java
public class com.feilong.lib.digester3.Digester extends org.xml.sax.helpers.DefaultHandler {
  public com.feilong.lib.digester3.Digester(org.xml.sax.XMLReader);
  public java.lang.ClassLoader getClassLoader();
  public void setClassLoader(java.lang.ClassLoader);
  public int getCount();
  public javax.xml.parsers.SAXParserFactory getFactory();
  public java.lang.String getMatch();
  public java.util.Stack<java.util.List<com.feilong.lib.digester3.Rule>> getMatches();
  public boolean getNamespaceAware();
  public void setNamespaceAware(boolean);
  public boolean getXIncludeAware();
  public void setXIncludeAware(boolean);
  public void setPublicId(java.lang.String);
  public java.lang.String getPublicId();
  public java.lang.String getRuleNamespaceURI();
  public void setRuleNamespaceURI(java.lang.String);
  public javax.xml.parsers.SAXParser getParser();
  public java.lang.Object getProperty(java.lang.String) throws org.xml.sax.SAXNotRecognizedException, org.xml.sax.SAXNotSupportedException;
  public void setProperty(java.lang.String, java.lang.Object) throws org.xml.sax.SAXNotRecognizedException, org.xml.sax.SAXNotSupportedException;
  public com.feilong.lib.digester3.Rules getRules();
  public void setRules(com.feilong.lib.digester3.Rules);
  public javax.xml.validation.Schema getXMLSchema();
  public void setXMLSchema(javax.xml.validation.Schema);
  public boolean getUseContextClassLoader();
  public void setUseContextClassLoader(boolean);
  public boolean getValidating();
  public void setValidating(boolean);
  public org.xml.sax.XMLReader getXMLReader() throws org.xml.sax.SAXException;
  public com.feilong.lib.digester3.Substitutor getSubstitutor();
  public void setSubstitutor(com.feilong.lib.digester3.Substitutor);
  public org.xml.sax.ContentHandler getCustomContentHandler();
  public void setCustomContentHandler(org.xml.sax.ContentHandler);
  public java.util.Map<java.lang.String, java.lang.String> getCurrentNamespaces();
  public void setExecutorService(java.util.concurrent.ExecutorService);
  public void characters(char[], int, int) throws org.xml.sax.SAXException;
  public void endDocument() throws org.xml.sax.SAXException;
  public void endElement(java.lang.String, java.lang.String, java.lang.String) throws org.xml.sax.SAXException;
  public void endPrefixMapping(java.lang.String) throws org.xml.sax.SAXException;
  public void ignorableWhitespace(char[], int, int) throws org.xml.sax.SAXException;
  public void processingInstruction(java.lang.String, java.lang.String) throws org.xml.sax.SAXException;
  public void setDocumentLocator(org.xml.sax.Locator);
  public void skippedEntity(java.lang.String) throws org.xml.sax.SAXException;
  public void startDocument() throws org.xml.sax.SAXException;
  public void startElement(java.lang.String, java.lang.String, java.lang.String, org.xml.sax.Attributes) throws org.xml.sax.SAXException;
  public void startPrefixMapping(java.lang.String, java.lang.String) throws org.xml.sax.SAXException;
  public void notationDecl(java.lang.String, java.lang.String, java.lang.String);
  public org.xml.sax.InputSource resolveEntity(java.lang.String, java.lang.String) throws org.xml.sax.SAXException;
  public void error(org.xml.sax.SAXParseException) throws org.xml.sax.SAXException;
  public void fatalError(org.xml.sax.SAXParseException) throws org.xml.sax.SAXException;
  public void warning(org.xml.sax.SAXParseException) throws org.xml.sax.SAXException;
  public <T> T parse(org.xml.sax.InputSource) throws java.io.IOException, org.xml.sax.SAXException;
  public <T> T parse(java.io.InputStream) throws java.io.IOException, org.xml.sax.SAXException;
  public <T> java.util.concurrent.Future<T> asyncParse(java.io.InputStream);
  public void registerAll(java.util.Map<java.lang.String, java.net.URL>);
  public org.xml.sax.InputSource createInputSourceFromURL(java.net.URL) throws java.io.IOException;
  public org.xml.sax.InputSource createInputSourceFromURL(java.lang.String) throws java.io.IOException;
  public void addRule(java.lang.String, com.feilong.lib.digester3.Rule);
  public void addFactoryCreate(java.lang.String, java.lang.Class<? extends com.feilong.lib.digester3.ObjectCreationFactory<?>>, java.lang.String, boolean);
  public void addSetProperties(java.lang.String);
  public void clear();
  public <T> T peek();
  public <T> T peek(int);
  public <T> T pop();
  public <T> void push(T);
  public <T> void push(java.lang.String, T);
  public <T> T pop(java.lang.String);
  public boolean isEmpty(java.lang.String);
  public <T> T getRoot();
  public void resetRoot();
  public boolean isConfigured();
  public java.lang.Object[] peekParams();
  public java.lang.Object[] peekParams(int);
  public java.lang.Object[] popParams();
  public void pushParams(java.lang.Object...);
  public org.xml.sax.SAXException createSAXException(java.lang.String, java.lang.Exception);
  public org.xml.sax.SAXException createSAXException(java.lang.Exception);
  public org.xml.sax.SAXException createSAXException(java.lang.String);
}
```

## `com.feilong.lib.digester3.ExtendedBaseRules`

```java
public class com.feilong.lib.digester3.ExtendedBaseRules extends com.feilong.lib.digester3.RulesBase {
  public com.feilong.lib.digester3.ExtendedBaseRules();
  public java.util.List<com.feilong.lib.digester3.Rule> match(java.lang.String, java.lang.String, java.lang.String, org.xml.sax.Attributes);
}
```

## `com.feilong.lib.digester3.FactoryCreateRule`

```java
public class com.feilong.lib.digester3.FactoryCreateRule extends com.feilong.lib.digester3.Rule {
  public com.feilong.lib.digester3.FactoryCreateRule(java.lang.String);
  public com.feilong.lib.digester3.FactoryCreateRule(java.lang.Class<? extends com.feilong.lib.digester3.ObjectCreationFactory<?>>);
  public com.feilong.lib.digester3.FactoryCreateRule(java.lang.String, java.lang.String);
  public com.feilong.lib.digester3.FactoryCreateRule(java.lang.Class<? extends com.feilong.lib.digester3.ObjectCreationFactory<?>>, java.lang.String);
  public com.feilong.lib.digester3.FactoryCreateRule(com.feilong.lib.digester3.ObjectCreationFactory<?>);
  public com.feilong.lib.digester3.FactoryCreateRule(java.lang.String, boolean);
  public com.feilong.lib.digester3.FactoryCreateRule(java.lang.Class<? extends com.feilong.lib.digester3.ObjectCreationFactory<?>>, boolean);
  public com.feilong.lib.digester3.FactoryCreateRule(java.lang.String, java.lang.String, boolean);
  public com.feilong.lib.digester3.FactoryCreateRule(java.lang.Class<? extends com.feilong.lib.digester3.ObjectCreationFactory<?>>, java.lang.String, boolean);
  public com.feilong.lib.digester3.FactoryCreateRule(com.feilong.lib.digester3.ObjectCreationFactory<?>, boolean);
  public void begin(java.lang.String, java.lang.String, org.xml.sax.Attributes) throws java.lang.Exception;
  public void end(java.lang.String, java.lang.String) throws java.lang.Exception;
  public void finish() throws java.lang.Exception;
  public java.lang.String toString();
}
```

## `com.feilong.lib.digester3.NodeCreateRule`

```java
public class com.feilong.lib.digester3.NodeCreateRule extends com.feilong.lib.digester3.Rule {
  public com.feilong.lib.digester3.NodeCreateRule() throws javax.xml.parsers.ParserConfigurationException;
  public com.feilong.lib.digester3.NodeCreateRule(javax.xml.parsers.DocumentBuilder);
  public com.feilong.lib.digester3.NodeCreateRule(int) throws javax.xml.parsers.ParserConfigurationException;
  public com.feilong.lib.digester3.NodeCreateRule(int, javax.xml.parsers.DocumentBuilder);
  public void begin(java.lang.String, java.lang.String, org.xml.sax.Attributes) throws java.lang.Exception;
  public void end(java.lang.String, java.lang.String) throws java.lang.Exception;
}
```

## `com.feilong.lib.digester3.ObjectCreateRule`

```java
public class com.feilong.lib.digester3.ObjectCreateRule extends com.feilong.lib.digester3.Rule {
  public com.feilong.lib.digester3.ObjectCreateRule(java.lang.String, java.lang.Class<?>);
  public void begin(java.lang.String, java.lang.String, org.xml.sax.Attributes) throws java.lang.Exception;
  public void end(java.lang.String, java.lang.String) throws java.lang.Exception;
  public java.lang.String toString();
}
```

## `com.feilong.lib.digester3.ObjectCreationFactory`

```java
public interface com.feilong.lib.digester3.ObjectCreationFactory<T> {
  public abstract T createObject(org.xml.sax.Attributes) throws java.lang.Exception;
  public abstract com.feilong.lib.digester3.Digester getDigester();
  public abstract void setDigester(com.feilong.lib.digester3.Digester);
}
```

## `com.feilong.lib.digester3.ObjectParamRule`

```java
public class com.feilong.lib.digester3.ObjectParamRule extends com.feilong.lib.digester3.Rule {
  public com.feilong.lib.digester3.ObjectParamRule(int, java.lang.Object);
  public com.feilong.lib.digester3.ObjectParamRule(int, java.lang.String, java.lang.Object);
  public void begin(java.lang.String, java.lang.String, org.xml.sax.Attributes) throws java.lang.Exception;
  public java.lang.String toString();
}
```

## `com.feilong.lib.digester3.PathCallParamRule`

```java
public class com.feilong.lib.digester3.PathCallParamRule extends com.feilong.lib.digester3.Rule {
  public com.feilong.lib.digester3.PathCallParamRule(int);
  public void begin(java.lang.String, java.lang.String, org.xml.sax.Attributes) throws java.lang.Exception;
  public java.lang.String toString();
}
```

## `com.feilong.lib.digester3.RegexMatcher`

```java
public abstract class com.feilong.lib.digester3.RegexMatcher {
  public com.feilong.lib.digester3.RegexMatcher();
  public abstract boolean match(java.lang.String, java.lang.String);
}
```

## `com.feilong.lib.digester3.Rule`

```java
public abstract class com.feilong.lib.digester3.Rule {
  public com.feilong.lib.digester3.Rule();
  public com.feilong.lib.digester3.Digester getDigester();
  public void setDigester(com.feilong.lib.digester3.Digester);
  public java.lang.String getNamespaceURI();
  public void setNamespaceURI(java.lang.String);
  public void begin(java.lang.String, java.lang.String, org.xml.sax.Attributes) throws java.lang.Exception;
  public void body(java.lang.String, java.lang.String, java.lang.String) throws java.lang.Exception;
  public void end(java.lang.String, java.lang.String) throws java.lang.Exception;
  public void finish() throws java.lang.Exception;
}
```

## `com.feilong.lib.digester3.RuleSet`

```java
public interface com.feilong.lib.digester3.RuleSet {
  public abstract java.lang.String getNamespaceURI();
  public abstract void addRuleInstances(com.feilong.lib.digester3.Digester);
}
```

## `com.feilong.lib.digester3.Rules`

```java
public interface com.feilong.lib.digester3.Rules {
  public abstract com.feilong.lib.digester3.Digester getDigester();
  public abstract void setDigester(com.feilong.lib.digester3.Digester);
  public abstract java.lang.String getNamespaceURI();
  public abstract void setNamespaceURI(java.lang.String);
  public abstract void add(java.lang.String, com.feilong.lib.digester3.Rule);
  public abstract void clear();
  public abstract java.util.List<com.feilong.lib.digester3.Rule> match(java.lang.String, java.lang.String, java.lang.String, org.xml.sax.Attributes);
  public abstract java.util.List<com.feilong.lib.digester3.Rule> rules();
}
```

## `com.feilong.lib.digester3.RulesBase`

```java
public class com.feilong.lib.digester3.RulesBase extends com.feilong.lib.digester3.AbstractRulesImpl {
  public com.feilong.lib.digester3.RulesBase();
  public void setDigester(com.feilong.lib.digester3.Digester);
  public void clear();
  public java.util.List<com.feilong.lib.digester3.Rule> match(java.lang.String, java.lang.String, java.lang.String, org.xml.sax.Attributes);
  public java.util.List<com.feilong.lib.digester3.Rule> rules();
}
```

## `com.feilong.lib.digester3.SetNestedPropertiesRule`

```java
public class com.feilong.lib.digester3.SetNestedPropertiesRule extends com.feilong.lib.digester3.Rule {
  public com.feilong.lib.digester3.SetNestedPropertiesRule();
  public com.feilong.lib.digester3.SetNestedPropertiesRule(java.lang.String, java.lang.String);
  public com.feilong.lib.digester3.SetNestedPropertiesRule(java.lang.String[], java.lang.String[]);
  public com.feilong.lib.digester3.SetNestedPropertiesRule(java.util.Map<java.lang.String, java.lang.String>);
  public void setDigester(com.feilong.lib.digester3.Digester);
  public void setTrimData(boolean);
  public boolean getTrimData();
  public void setAllowUnknownChildElements(boolean);
  public boolean getAllowUnknownChildElements();
  public void begin(java.lang.String, java.lang.String, org.xml.sax.Attributes) throws java.lang.Exception;
  public void body(java.lang.String, java.lang.String, java.lang.String) throws java.lang.Exception;
  public void addAlias(java.lang.String, java.lang.String);
  public java.lang.String toString();
}
```

## `com.feilong.lib.digester3.SetNextRule`

```java
public class com.feilong.lib.digester3.SetNextRule extends com.feilong.lib.digester3.AbstractMethodRule {
  public com.feilong.lib.digester3.SetNextRule(java.lang.String);
  public com.feilong.lib.digester3.SetNextRule(java.lang.String, java.lang.String);
  public com.feilong.lib.digester3.SetNextRule(java.lang.String, java.lang.Class<?>);
}
```

## `com.feilong.lib.digester3.SetPropertiesRule`

```java
public class com.feilong.lib.digester3.SetPropertiesRule extends com.feilong.lib.digester3.Rule {
  public com.feilong.lib.digester3.SetPropertiesRule();
  public com.feilong.lib.digester3.SetPropertiesRule(java.lang.String, java.lang.String);
  public com.feilong.lib.digester3.SetPropertiesRule(java.lang.String[], java.lang.String[]);
  public com.feilong.lib.digester3.SetPropertiesRule(java.util.Map<java.lang.String, java.lang.String>);
  public void begin(java.lang.String, java.lang.String, org.xml.sax.Attributes) throws java.lang.Exception;
  public void addAlias(java.lang.String, java.lang.String);
  public java.lang.String toString();
  public boolean isIgnoreMissingProperty();
  public void setIgnoreMissingProperty(boolean);
}
```

## `com.feilong.lib.digester3.SetPropertyRule`

```java
public class com.feilong.lib.digester3.SetPropertyRule extends com.feilong.lib.digester3.Rule {
  public com.feilong.lib.digester3.SetPropertyRule(java.lang.String, java.lang.String);
  public void begin(java.lang.String, java.lang.String, org.xml.sax.Attributes) throws java.lang.Exception;
  public java.lang.String toString();
}
```

## `com.feilong.lib.digester3.SetRootRule`

```java
public class com.feilong.lib.digester3.SetRootRule extends com.feilong.lib.digester3.AbstractMethodRule {
  public com.feilong.lib.digester3.SetRootRule(java.lang.String);
  public com.feilong.lib.digester3.SetRootRule(java.lang.String, java.lang.String);
  public com.feilong.lib.digester3.SetRootRule(java.lang.String, java.lang.Class<?>);
}
```

## `com.feilong.lib.digester3.SetTopRule`

```java
public class com.feilong.lib.digester3.SetTopRule extends com.feilong.lib.digester3.AbstractMethodRule {
  public com.feilong.lib.digester3.SetTopRule(java.lang.String);
  public com.feilong.lib.digester3.SetTopRule(java.lang.String, java.lang.String);
  public com.feilong.lib.digester3.SetTopRule(java.lang.String, java.lang.Class<?>);
}
```

## `com.feilong.lib.digester3.Substitutor`

```java
public abstract class com.feilong.lib.digester3.Substitutor {
  public com.feilong.lib.digester3.Substitutor();
  public abstract org.xml.sax.Attributes substitute(org.xml.sax.Attributes);
  public abstract java.lang.String substitute(java.lang.String);
}
```
