# cn.hutool.json.xml

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.json.xml.JSONXMLParser`

```java
public class cn.hutool.json.xml.JSONXMLParser {
  public cn.hutool.json.xml.JSONXMLParser();
  public static void parseJSONObject(cn.hutool.json.JSONObject, java.lang.String, boolean) throws cn.hutool.json.JSONException;
  public static void parseJSONObject(cn.hutool.json.JSONObject, java.lang.String, cn.hutool.json.xml.ParseConfig) throws cn.hutool.json.JSONException;
}
```

## `cn.hutool.json.xml.JSONXMLSerializer`

```java
public class cn.hutool.json.xml.JSONXMLSerializer {
  public cn.hutool.json.xml.JSONXMLSerializer();
  public static java.lang.String toXml(java.lang.Object) throws cn.hutool.json.JSONException;
  public static java.lang.String toXml(java.lang.Object, java.lang.String) throws cn.hutool.json.JSONException;
  public static java.lang.String toXml(java.lang.Object, java.lang.String, java.lang.String...) throws cn.hutool.json.JSONException;
}
```

## `cn.hutool.json.xml.ParseConfig`

```java
public class cn.hutool.json.xml.ParseConfig implements java.io.Serializable {
  public cn.hutool.json.xml.ParseConfig();
  public static cn.hutool.json.xml.ParseConfig of();
  public boolean isKeepStrings();
  public cn.hutool.json.xml.ParseConfig setKeepStrings(boolean);
  public int getMaxNestingDepth();
  public cn.hutool.json.xml.ParseConfig setMaxNestingDepth(int);
}
```
