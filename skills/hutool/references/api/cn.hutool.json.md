# cn.hutool.json

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.json.InternalJSONUtil`

```java
public final class cn.hutool.json.InternalJSONUtil {
  public static java.lang.Object stringToValue(java.lang.String);
}
```

## `cn.hutool.json.JSON`

```java
public interface cn.hutool.json.JSON extends java.lang.Cloneable,java.io.Serializable,cn.hutool.core.bean.copier.IJSONTypeConverter {
  public abstract cn.hutool.json.JSONConfig getConfig();
  public abstract java.lang.Object getByPath(java.lang.String);
  public abstract void putByPath(java.lang.String, java.lang.Object);
  public abstract <T> T getByPath(java.lang.String, java.lang.Class<T>);
  public abstract <T> T getByPath(java.lang.String, cn.hutool.core.lang.TypeReference<T>);
  public default java.lang.String toStringPretty() throws cn.hutool.json.JSONException;
  public default java.lang.String toJSONString(int) throws cn.hutool.json.JSONException;
  public default java.io.Writer write(java.io.Writer) throws cn.hutool.json.JSONException;
  public abstract java.io.Writer write(java.io.Writer, int, int) throws cn.hutool.json.JSONException;
  public default <T> T toBean(java.lang.Class<T>);
  public default <T> T toBean(cn.hutool.core.lang.TypeReference<T>);
  public default <T> T toBean(java.lang.reflect.Type);
  public default <T> T toBean(java.lang.reflect.Type, boolean);
}
```

## `cn.hutool.json.JSONArray`

```java
public class cn.hutool.json.JSONArray implements cn.hutool.json.JSON, cn.hutool.json.JSONGetter<java.lang.Integer>, java.util.List<java.lang.Object>, java.util.RandomAccess {
  public cn.hutool.json.JSONArray();
  public cn.hutool.json.JSONArray(int);
  public cn.hutool.json.JSONArray(cn.hutool.json.JSONConfig);
  public cn.hutool.json.JSONArray(int, cn.hutool.json.JSONConfig);
  public cn.hutool.json.JSONArray(java.lang.Object) throws cn.hutool.json.JSONException;
  public cn.hutool.json.JSONArray(java.lang.Object, boolean) throws cn.hutool.json.JSONException;
  public cn.hutool.json.JSONArray(java.lang.Object, cn.hutool.json.JSONConfig) throws cn.hutool.json.JSONException;
  public cn.hutool.json.JSONArray(java.lang.Object, cn.hutool.json.JSONConfig, cn.hutool.core.lang.Filter<cn.hutool.core.lang.mutable.Mutable<java.lang.Object>>) throws cn.hutool.json.JSONException;
  public cn.hutool.json.JSONConfig getConfig();
  public cn.hutool.json.JSONArray setDateFormat(java.lang.String);
  public java.lang.String join(java.lang.String) throws cn.hutool.json.JSONException;
  public java.lang.Object get(int);
  public java.lang.Object getObj(java.lang.Integer, java.lang.Object);
  public java.lang.Object getByPath(java.lang.String);
  public <T> T getByPath(java.lang.String, java.lang.Class<T>);
  public <T> T getByPath(java.lang.String, cn.hutool.core.lang.TypeReference<T>);
  public void putByPath(java.lang.String, java.lang.Object);
  public cn.hutool.json.JSONArray put(java.lang.Object);
  public cn.hutool.json.JSONArray set(java.lang.Object);
  public cn.hutool.json.JSONArray put(int, java.lang.Object) throws cn.hutool.json.JSONException;
  public cn.hutool.json.JSONObject toJSONObject(cn.hutool.json.JSONArray) throws cn.hutool.json.JSONException;
  public int hashCode();
  public boolean equals(java.lang.Object);
  public java.util.Iterator<java.lang.Object> iterator();
  public java.lang.Iterable<cn.hutool.json.JSONObject> jsonIter();
  public int size();
  public boolean isEmpty();
  public boolean contains(java.lang.Object);
  public java.lang.Object[] toArray();
  public <T> T[] toArray(T[]);
  public boolean add(java.lang.Object);
  public java.lang.Object remove(int);
  public boolean remove(java.lang.Object);
  public boolean containsAll(java.util.Collection<?>);
  public boolean addAll(java.util.Collection<?>);
  public boolean addAll(int, java.util.Collection<?>);
  public boolean removeAll(java.util.Collection<?>);
  public boolean retainAll(java.util.Collection<?>);
  public void clear();
  public java.lang.Object set(int, java.lang.Object);
  public java.lang.Object set(int, java.lang.Object, cn.hutool.core.lang.Filter<cn.hutool.core.lang.mutable.MutablePair<java.lang.Integer, java.lang.Object>>);
  public void add(int, java.lang.Object);
  public int indexOf(java.lang.Object);
  public int lastIndexOf(java.lang.Object);
  public java.util.ListIterator<java.lang.Object> listIterator();
  public java.util.ListIterator<java.lang.Object> listIterator(int);
  public java.util.List<java.lang.Object> subList(int, int);
  public java.lang.Object toArray(java.lang.Class<?>);
  public <T> java.util.List<T> toList(java.lang.Class<T>);
  public java.lang.String toString();
  public java.lang.String toJSONString(int, cn.hutool.core.lang.Filter<cn.hutool.core.lang.mutable.MutablePair<java.lang.Object, java.lang.Object>>);
  public java.io.Writer write(java.io.Writer, int, int) throws cn.hutool.json.JSONException;
  public java.io.Writer write(java.io.Writer, int, int, cn.hutool.core.lang.Filter<cn.hutool.core.lang.mutable.MutablePair<java.lang.Object, java.lang.Object>>) throws cn.hutool.json.JSONException;
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
  public java.lang.Object getObj(java.lang.Object, java.lang.Object);
}
```

## `cn.hutool.json.JSONBeanParser`

```java
public interface cn.hutool.json.JSONBeanParser<T> {
  public abstract void parse(T);
}
```

## `cn.hutool.json.JSONConfig`

```java
public class cn.hutool.json.JSONConfig implements java.io.Serializable {
  public cn.hutool.json.JSONConfig();
  public static cn.hutool.json.JSONConfig create();
  public boolean isOrder();
  public cn.hutool.json.JSONConfig setOrder(boolean);
  public java.util.Comparator<java.lang.String> getKeyComparator();
  public cn.hutool.json.JSONConfig setNatureKeyComparator();
  public cn.hutool.json.JSONConfig setKeyComparator(java.util.Comparator<java.lang.String>);
  public boolean isIgnoreError();
  public cn.hutool.json.JSONConfig setIgnoreError(boolean);
  public boolean isIgnoreCase();
  public cn.hutool.json.JSONConfig setIgnoreCase(boolean);
  public java.lang.String getDateFormat();
  public cn.hutool.json.JSONConfig setDateFormat(java.lang.String);
  public boolean isIgnoreNullValue();
  public cn.hutool.json.JSONConfig setIgnoreNullValue(boolean);
  public boolean isTransientSupport();
  public cn.hutool.json.JSONConfig setTransientSupport(boolean);
  public boolean isStripTrailingZeros();
  public cn.hutool.json.JSONConfig setStripTrailingZeros(boolean);
  public boolean isCheckDuplicate();
  public cn.hutool.json.JSONConfig setCheckDuplicate(boolean);
  public boolean isWriteLongAsString();
  public cn.hutool.json.JSONConfig setWriteLongAsString(boolean);
}
```

## `cn.hutool.json.JSONConverter`

```java
public class cn.hutool.json.JSONConverter implements cn.hutool.core.convert.Converter<cn.hutool.json.JSON> {
  public cn.hutool.json.JSONConverter();
  public cn.hutool.json.JSON convert(java.lang.Object, cn.hutool.json.JSON) throws java.lang.IllegalArgumentException;
  public java.lang.Object convert(java.lang.Object, java.lang.Object) throws java.lang.IllegalArgumentException;
}
```

## `cn.hutool.json.JSONException`

```java
public class cn.hutool.json.JSONException extends java.lang.RuntimeException {
  public cn.hutool.json.JSONException(java.lang.Throwable);
  public cn.hutool.json.JSONException(java.lang.String);
  public cn.hutool.json.JSONException(java.lang.String, java.lang.Object...);
  public cn.hutool.json.JSONException(java.lang.String, java.lang.Throwable);
  public cn.hutool.json.JSONException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.json.JSONException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.json.JSONGetter`

```java
public interface cn.hutool.json.JSONGetter<K> extends cn.hutool.core.getter.OptNullBasicTypeFromObjectGetter<K> {
  public abstract cn.hutool.json.JSONConfig getConfig();
  public default boolean isNull(K);
  public default java.lang.String getStrEscaped(K);
  public default java.lang.String getStrEscaped(K, java.lang.String);
  public default cn.hutool.json.JSONArray getJSONArray(K);
  public default cn.hutool.json.JSONObject getJSONObject(K);
  public default <T> T getBean(K, java.lang.Class<T>);
  public default <T> java.util.List<T> getBeanList(K, java.lang.Class<T>);
  public default java.util.Date getDate(K, java.util.Date);
  public default java.time.LocalDateTime getLocalDateTime(K, java.time.LocalDateTime);
  public default byte[] getBytes(K);
  public default <T> T get(K, java.lang.Class<T>) throws cn.hutool.core.convert.ConvertException;
  public default <T> T get(K, java.lang.Class<T>, boolean) throws cn.hutool.core.convert.ConvertException;
}
```

## `cn.hutool.json.JSONNull`

```java
public class cn.hutool.json.JSONNull implements java.io.Serializable {
  public cn.hutool.json.JSONNull();
  public boolean equals(java.lang.Object);
  public java.lang.String toString();
}
```

## `cn.hutool.json.JSONObject`

```java
public class cn.hutool.json.JSONObject extends cn.hutool.core.map.MapWrapper<java.lang.String, java.lang.Object> implements cn.hutool.json.JSON, cn.hutool.json.JSONGetter<java.lang.String> {
  public cn.hutool.json.JSONObject();
  public cn.hutool.json.JSONObject(boolean);
  public cn.hutool.json.JSONObject(int, boolean);
  public cn.hutool.json.JSONObject(int, boolean, boolean);
  public cn.hutool.json.JSONObject(cn.hutool.json.JSONConfig);
  public cn.hutool.json.JSONObject(int, cn.hutool.json.JSONConfig);
  public cn.hutool.json.JSONObject(java.lang.Object);
  public cn.hutool.json.JSONObject(java.lang.Object, boolean);
  public cn.hutool.json.JSONObject(java.lang.Object, boolean, boolean);
  public cn.hutool.json.JSONObject(java.lang.Object, cn.hutool.json.JSONConfig);
  public cn.hutool.json.JSONObject(java.lang.Object, cn.hutool.json.JSONConfig, cn.hutool.core.lang.Filter<cn.hutool.core.lang.mutable.MutablePair<java.lang.String, java.lang.Object>>);
  public cn.hutool.json.JSONObject(java.lang.Object, java.lang.String...);
  public cn.hutool.json.JSONObject(java.lang.CharSequence, boolean) throws cn.hutool.json.JSONException;
  public cn.hutool.json.JSONConfig getConfig();
  public cn.hutool.json.JSONObject setDateFormat(java.lang.String);
  public cn.hutool.json.JSONArray toJSONArray(java.util.Collection<java.lang.String>) throws cn.hutool.json.JSONException;
  public java.lang.Object getObj(java.lang.String, java.lang.Object);
  public java.lang.Object getByPath(java.lang.String);
  public <T> T getByPath(java.lang.String, java.lang.Class<T>);
  public <T> T getByPath(java.lang.String, cn.hutool.core.lang.TypeReference<T>);
  public void putByPath(java.lang.String, java.lang.Object);
  public cn.hutool.json.JSONObject put(java.lang.String, java.lang.Object) throws cn.hutool.json.JSONException;
  public cn.hutool.json.JSONObject set(java.lang.String, java.lang.Object) throws cn.hutool.json.JSONException;
  public cn.hutool.json.JSONObject set(java.lang.String, java.lang.Object, cn.hutool.core.lang.Filter<cn.hutool.core.lang.mutable.MutablePair<java.lang.String, java.lang.Object>>, boolean) throws cn.hutool.json.JSONException;
  public cn.hutool.json.JSONObject putOnce(java.lang.String, java.lang.Object) throws cn.hutool.json.JSONException;
  public cn.hutool.json.JSONObject setOnce(java.lang.String, java.lang.Object, cn.hutool.core.lang.Filter<cn.hutool.core.lang.mutable.MutablePair<java.lang.String, java.lang.Object>>) throws cn.hutool.json.JSONException;
  public cn.hutool.json.JSONObject putOpt(java.lang.String, java.lang.Object) throws cn.hutool.json.JSONException;
  public void putAll(java.util.Map<? extends java.lang.String, ?>);
  public cn.hutool.json.JSONObject accumulate(java.lang.String, java.lang.Object) throws cn.hutool.json.JSONException;
  public cn.hutool.json.JSONObject append(java.lang.String, java.lang.Object) throws cn.hutool.json.JSONException;
  public cn.hutool.json.JSONObject increment(java.lang.String) throws cn.hutool.json.JSONException;
  public java.lang.String toString();
  public java.lang.String toJSONString(int, cn.hutool.core.lang.Filter<cn.hutool.core.lang.mutable.MutablePair<java.lang.Object, java.lang.Object>>);
  public java.io.Writer write(java.io.Writer, int, int) throws cn.hutool.json.JSONException;
  public java.io.Writer write(java.io.Writer, int, int, cn.hutool.core.lang.Filter<cn.hutool.core.lang.mutable.MutablePair<java.lang.Object, java.lang.Object>>) throws cn.hutool.json.JSONException;
  public cn.hutool.json.JSONObject clone() throws java.lang.CloneNotSupportedException;
  public cn.hutool.core.map.MapWrapper clone() throws java.lang.CloneNotSupportedException;
  public java.lang.Object put(java.lang.Object, java.lang.Object);
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
  public java.lang.Object getObj(java.lang.Object, java.lang.Object);
}
```

## `cn.hutool.json.JSONObjectIter`

```java
public class cn.hutool.json.JSONObjectIter implements java.lang.Iterable<cn.hutool.json.JSONObject> {
  public cn.hutool.json.JSONObjectIter(java.util.Iterator<java.lang.Object>);
  public java.util.Iterator<cn.hutool.json.JSONObject> iterator();
}
```

## `cn.hutool.json.JSONParser`

```java
public class cn.hutool.json.JSONParser {
  public static cn.hutool.json.JSONParser of(cn.hutool.json.JSONTokener);
  public cn.hutool.json.JSONParser(cn.hutool.json.JSONTokener);
  public void parseTo(cn.hutool.json.JSONObject, cn.hutool.core.lang.Filter<cn.hutool.core.lang.mutable.MutablePair<java.lang.String, java.lang.Object>>);
  public void parseTo(cn.hutool.json.JSONArray, cn.hutool.core.lang.Filter<cn.hutool.core.lang.mutable.Mutable<java.lang.Object>>);
}
```

## `cn.hutool.json.JSONStrFormatter`

```java
public class cn.hutool.json.JSONStrFormatter {
  public cn.hutool.json.JSONStrFormatter();
  public static java.lang.String format(java.lang.String);
}
```

## `cn.hutool.json.JSONString`

```java
public interface cn.hutool.json.JSONString {
  public abstract java.lang.String toJSONString();
}
```

## `cn.hutool.json.JSONSupport`

```java
public class cn.hutool.json.JSONSupport implements cn.hutool.json.JSONString, cn.hutool.json.JSONBeanParser<cn.hutool.json.JSON> {
  public cn.hutool.json.JSONSupport();
  public void parse(java.lang.String);
  public void parse(cn.hutool.json.JSON);
  public cn.hutool.json.JSONObject toJSON();
  public java.lang.String toJSONString();
  public java.lang.String toPrettyString();
  public java.lang.String toString();
  public void parse(java.lang.Object);
}
```

## `cn.hutool.json.JSONTokener`

```java
public class cn.hutool.json.JSONTokener {
  public cn.hutool.json.JSONTokener(java.io.Reader, cn.hutool.json.JSONConfig);
  public cn.hutool.json.JSONTokener(java.io.InputStream, cn.hutool.json.JSONConfig) throws cn.hutool.json.JSONException;
  public cn.hutool.json.JSONTokener(java.lang.CharSequence, cn.hutool.json.JSONConfig);
  public void back() throws cn.hutool.json.JSONException;
  public boolean end();
  public boolean more() throws cn.hutool.json.JSONException;
  public char next() throws cn.hutool.json.JSONException;
  public char next(char) throws cn.hutool.json.JSONException;
  public java.lang.String next(int) throws cn.hutool.json.JSONException;
  public char nextClean() throws cn.hutool.json.JSONException;
  public java.lang.String nextString(char) throws cn.hutool.json.JSONException;
  public java.lang.String nextTo(char) throws cn.hutool.json.JSONException;
  public java.lang.String nextTo(java.lang.String) throws cn.hutool.json.JSONException;
  public java.lang.String nextStringValue();
  public java.lang.Object nextValue() throws cn.hutool.json.JSONException;
  public char skipTo(char) throws cn.hutool.json.JSONException;
  public cn.hutool.json.JSONException syntaxError(java.lang.String);
  public cn.hutool.json.JSONArray toJSONArray();
  public java.lang.String toString();
}
```

## `cn.hutool.json.JSONUtil`

```java
public class cn.hutool.json.JSONUtil {
  public cn.hutool.json.JSONUtil();
  public static cn.hutool.json.JSONObject createObj();
  public static cn.hutool.json.JSONObject createObj(cn.hutool.json.JSONConfig);
  public static cn.hutool.json.JSONArray createArray();
  public static cn.hutool.json.JSONArray createArray(cn.hutool.json.JSONConfig);
  public static cn.hutool.json.JSONObject parseObj(java.lang.String);
  public static cn.hutool.json.JSONObject parseObj(java.lang.Object);
  public static cn.hutool.json.JSONObject parseObj(java.lang.Object, cn.hutool.json.JSONConfig);
  public static cn.hutool.json.JSONObject parseObj(java.lang.Object, boolean);
  public static cn.hutool.json.JSONObject parseObj(java.lang.Object, boolean, boolean);
  public static cn.hutool.json.JSONArray parseArray(java.lang.String);
  public static cn.hutool.json.JSONArray parseArray(java.lang.Object);
  public static cn.hutool.json.JSONArray parseArray(java.lang.Object, cn.hutool.json.JSONConfig);
  public static cn.hutool.json.JSONArray parseArray(java.lang.Object, boolean);
  public static cn.hutool.json.JSON parse(java.lang.Object);
  public static cn.hutool.json.JSON parse(java.lang.Object, cn.hutool.json.JSONConfig);
  public static cn.hutool.json.JSONObject parseFromXml(java.lang.String);
  public static cn.hutool.json.JSON readJSON(java.io.File, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public static cn.hutool.json.JSONObject readJSONObject(java.io.File, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public static cn.hutool.json.JSONArray readJSONArray(java.io.File, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String toJsonStr(cn.hutool.json.JSON, int);
  public static java.lang.String toJsonStr(cn.hutool.json.JSON);
  public static void toJsonStr(cn.hutool.json.JSON, java.io.Writer);
  public static java.lang.String toJsonPrettyStr(cn.hutool.json.JSON);
  public static java.lang.String toJsonStr(java.lang.Object);
  public static java.lang.String toJsonStr(java.lang.Object, cn.hutool.json.JSONConfig);
  public static void toJsonStr(java.lang.Object, java.io.Writer);
  public static java.lang.String toJsonPrettyStr(java.lang.Object);
  public static java.lang.String toXmlStr(cn.hutool.json.JSON);
  public static <T> T toBean(java.lang.String, java.lang.Class<T>);
  public static <T> T toBean(java.lang.String, cn.hutool.json.JSONConfig, java.lang.Class<T>);
  public static <T> T toBean(cn.hutool.json.JSONObject, java.lang.Class<T>);
  public static <T> T toBean(java.lang.String, cn.hutool.core.lang.TypeReference<T>, boolean);
  public static <T> T toBean(java.lang.String, java.lang.reflect.Type, boolean);
  public static <T> T toBean(cn.hutool.json.JSON, cn.hutool.core.lang.TypeReference<T>, boolean);
  public static <T> T toBean(cn.hutool.json.JSON, java.lang.reflect.Type, boolean);
  public static <T> java.util.List<T> toList(java.lang.String, java.lang.Class<T>);
  public static <T> java.util.List<T> toList(cn.hutool.json.JSONArray, java.lang.Class<T>);
  public static java.lang.Object getByPath(cn.hutool.json.JSON, java.lang.String);
  public static <T> T getByPath(cn.hutool.json.JSON, java.lang.String, T);
  public static void putByPath(cn.hutool.json.JSON, java.lang.String, java.lang.Object);
  public static java.lang.String quote(java.lang.String);
  public static java.lang.String quote(java.lang.String, boolean);
  public static java.io.Writer quote(java.lang.String, java.io.Writer) throws java.io.IOException;
  public static java.io.Writer quote(java.lang.String, java.io.Writer, boolean) throws java.io.IOException;
  public static java.lang.String escape(java.lang.String);
  public static java.lang.Object wrap(java.lang.Object, cn.hutool.json.JSONConfig);
  public static java.lang.String formatJsonStr(java.lang.String);
  public static boolean isJson(java.lang.String);
  public static boolean isTypeJSON(java.lang.String);
  public static boolean isJsonObj(java.lang.String);
  public static boolean isTypeJSONObject(java.lang.String);
  public static boolean isJsonArray(java.lang.String);
  public static boolean isTypeJSONArray(java.lang.String);
  public static boolean isNull(java.lang.Object);
  public static cn.hutool.json.JSONObject xmlToJson(java.lang.String);
  public static void putSerializer(java.lang.reflect.Type, cn.hutool.json.serialize.JSONArraySerializer<?>);
  public static void putSerializer(java.lang.reflect.Type, cn.hutool.json.serialize.JSONObjectSerializer<?>);
  public static void putDeserializer(java.lang.reflect.Type, cn.hutool.json.serialize.JSONDeserializer<?>);
}
```

## `cn.hutool.json.ObjectMapper`

```java
public class cn.hutool.json.ObjectMapper {
  public static cn.hutool.json.ObjectMapper of(java.lang.Object);
  public cn.hutool.json.ObjectMapper(java.lang.Object);
  public void map(cn.hutool.json.JSONObject, cn.hutool.core.lang.Filter<cn.hutool.core.lang.mutable.MutablePair<java.lang.String, java.lang.Object>>);
  public void map(cn.hutool.json.JSONArray, cn.hutool.core.lang.Filter<cn.hutool.core.lang.mutable.Mutable<java.lang.Object>>) throws cn.hutool.json.JSONException;
}
```

## `cn.hutool.json.XML`

```java
public class cn.hutool.json.XML {
  public cn.hutool.json.XML();
  public static cn.hutool.json.JSONObject toJSONObject(java.lang.String) throws cn.hutool.json.JSONException;
  public static cn.hutool.json.JSONObject toJSONObject(java.lang.String, boolean) throws cn.hutool.json.JSONException;
  public static cn.hutool.json.JSONObject toJSONObject(java.lang.String, cn.hutool.json.xml.ParseConfig) throws cn.hutool.json.JSONException;
  public static cn.hutool.json.JSONObject toJSONObject(cn.hutool.json.JSONObject, java.lang.String, boolean) throws cn.hutool.json.JSONException;
  public static cn.hutool.json.JSONObject toJSONObject(cn.hutool.json.JSONObject, java.lang.String, cn.hutool.json.xml.ParseConfig) throws cn.hutool.json.JSONException;
  public static java.lang.String toXml(java.lang.Object) throws cn.hutool.json.JSONException;
  public static java.lang.String toXml(java.lang.Object, java.lang.String) throws cn.hutool.json.JSONException;
  public static java.lang.String toXml(java.lang.Object, java.lang.String, java.lang.String...) throws cn.hutool.json.JSONException;
}
```

## `cn.hutool.json.XMLTokener`

```java
public class cn.hutool.json.XMLTokener extends cn.hutool.json.JSONTokener {
  public cn.hutool.json.XMLTokener(java.lang.CharSequence, cn.hutool.json.JSONConfig);
  public java.lang.String nextCDATA() throws cn.hutool.json.JSONException;
  public java.lang.Object nextContent() throws cn.hutool.json.JSONException;
  public java.lang.Object nextEntity(char) throws cn.hutool.json.JSONException;
  public java.lang.Object nextMeta() throws cn.hutool.json.JSONException;
  public java.lang.Object nextToken() throws cn.hutool.json.JSONException;
  public boolean skipPast(java.lang.String) throws cn.hutool.json.JSONException;
}
```
