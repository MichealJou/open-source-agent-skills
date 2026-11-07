# cn.hutool.json.serialize

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.json.serialize.GlobalSerializeMapping`

```java
public class cn.hutool.json.serialize.GlobalSerializeMapping {
  public cn.hutool.json.serialize.GlobalSerializeMapping();
  public static void put(java.lang.reflect.Type, cn.hutool.json.serialize.JSONArraySerializer<?>);
  public static void put(java.lang.reflect.Type, cn.hutool.json.serialize.JSONObjectSerializer<?>);
  public static synchronized void put(java.lang.reflect.Type, cn.hutool.json.serialize.JSONDeserializer<?>);
  public static cn.hutool.json.serialize.JSONSerializer<? extends cn.hutool.json.JSON, ?> getSerializer(java.lang.reflect.Type);
  public static cn.hutool.json.serialize.JSONDeserializer<?> getDeserializer(java.lang.reflect.Type);
}
```

## `cn.hutool.json.serialize.JSONDeserializer`

```java
public interface cn.hutool.json.serialize.JSONDeserializer<T> {
  public abstract T deserialize(cn.hutool.json.JSON);
}
```

## `cn.hutool.json.serialize.JSONSerializer`

```java
public interface cn.hutool.json.serialize.JSONSerializer<T extends cn.hutool.json.JSON, V> {
  public abstract void serialize(T, V);
}
```

## `cn.hutool.json.serialize.JSONWriter`

```java
public class cn.hutool.json.serialize.JSONWriter extends java.io.Writer {
  public static cn.hutool.json.serialize.JSONWriter of(java.io.Writer, int, int, cn.hutool.json.JSONConfig);
  public cn.hutool.json.serialize.JSONWriter(java.io.Writer, int, int, cn.hutool.json.JSONConfig);
  public cn.hutool.json.serialize.JSONWriter beginObj();
  public cn.hutool.json.serialize.JSONWriter beginArray();
  public cn.hutool.json.serialize.JSONWriter end();
  public cn.hutool.json.serialize.JSONWriter writeKey(java.lang.String);
  public cn.hutool.json.serialize.JSONWriter writeValue(java.lang.Object);
  public cn.hutool.json.serialize.JSONWriter writeField(java.lang.String, java.lang.Object);
  public cn.hutool.json.serialize.JSONWriter writeField(cn.hutool.core.lang.mutable.MutablePair<java.lang.Object, java.lang.Object>, cn.hutool.core.lang.Filter<cn.hutool.core.lang.mutable.MutablePair<java.lang.Object, java.lang.Object>>);
  public void write(char[], int, int) throws java.io.IOException;
  public void flush();
  public void close() throws java.io.IOException;
}
```

## `cn.hutool.json.serialize.TemporalAccessorSerializer`

```java
public class cn.hutool.json.serialize.TemporalAccessorSerializer implements cn.hutool.json.serialize.JSONObjectSerializer<java.time.temporal.TemporalAccessor>, cn.hutool.json.serialize.JSONDeserializer<java.time.temporal.TemporalAccessor> {
  public cn.hutool.json.serialize.TemporalAccessorSerializer(java.lang.Class<? extends java.time.temporal.TemporalAccessor>);
  public void serialize(cn.hutool.json.JSONObject, java.time.temporal.TemporalAccessor);
  public java.time.temporal.TemporalAccessor deserialize(cn.hutool.json.JSON);
  public void serialize(cn.hutool.json.JSON, java.lang.Object);
  public java.lang.Object deserialize(cn.hutool.json.JSON);
}
```
