# com.feilong.xml

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.xml.XXEUtil` | `DocumentBuilderFactory disableXXE(DocumentBuilderFactory documentBuilderFactory)` | 关闭XXE，避免漏洞攻击. XML外部实体注入漏洞(XML External Entity Injection，简称XXE)，该安全问题是由XML组件默认没有禁用外部实体引用导致。 see: https://www.owasp.org/index.php/XML_External_Entity_(XXE)_Prevention_Cheat_Sheet#JAXP_DocumentBuilderFactory.2C_SAXParserFactory_and_DOM4J Note: The above defenses require Java 7 update 67, Java 8 update … |
| `com.feilong.xml.XmlUtil` | `Map<String, String> getNodeAttributeValueAndStringValueMap(Object xml,String xpathExpression,final String nodeAttributeName)` | 获得 node attribute value and string value map. |
| `com.feilong.xml.XmlUtil` | `Map<String, String> getNodeNameAndStringValueMap(Object xml,String xpathExpression)` | 根据xpath表达式, 来获得节点的名字和string value map. 按照顺序返回 |
| `com.feilong.xml.XmlUtil` | `Map<String, String> toMap(String xml,String rootElementName)` | 将xml字符串转成 Map. |
| `com.feilong.xml.XmlUtil` | `String format(String xml)` | 【原文待译】Format. |
| `com.feilong.xml.XmlUtil` | `String toXML(Map<K, V> map,String rootElementName)` | 将 map 转成 xml string. |
| `com.feilong.xml.XmlUtil` | `String toXML(Map<K, V> map,String rootElementName,boolean isPrettyPrint)` | 将 map 转成 xml 字符串. |
| `com.feilong.xml.XmlUtil` | `String toXML(Object bean,XStreamConfig xStreamConfig)` | 将object转成xml字符串. |
| `com.feilong.xml.XmlUtil` | `T toBean(String xml,Class<T> processAnnotationsType)` | 将 xml 字符串,转成带注解的 processAnnotationsType 对象. |
| `com.feilong.xml.XmlUtil` | `T toBean(String xml,XStreamConfig xStreamConfig)` | 【原文待译】From xml. |
