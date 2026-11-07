# com.google.common.xml

版本 33.4.8-jre。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.google.common.xml.XmlEscapers` | `Escaper xmlAttributeEscaper()` | 【原文待译】Returns an Escaper instance that escapes special characters in a string so it can safely be included in XML document as an attribute value. See section 3.3.3 of the XML specification. This escaper substitutes 0xFFFD for non-whitespace control characters and the character values 0xFFFE and 0xFFFF whi… |
| `com.google.common.xml.XmlEscapers` | `Escaper xmlContentEscaper()` | 【原文待译】Returns an Escaper instance that escapes special characters in a string so it can safely be included in an XML document as element content. See section 2.4 of the XML specification. Note: Double and single quotes are not escaped, so it is not safe to use this escaper to escape attribute values. Use … |
