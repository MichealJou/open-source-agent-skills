# com.feilong.lib.org.apache.http.params

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.params.AbstractHttpParams`

```java
public abstract class com.feilong.lib.org.apache.http.params.AbstractHttpParams implements com.feilong.lib.org.apache.http.params.HttpParams,com.feilong.lib.org.apache.http.params.HttpParamsNames {
  public long getLongParameter(java.lang.String, long);
  public com.feilong.lib.org.apache.http.params.HttpParams setLongParameter(java.lang.String, long);
  public int getIntParameter(java.lang.String, int);
  public com.feilong.lib.org.apache.http.params.HttpParams setIntParameter(java.lang.String, int);
  public double getDoubleParameter(java.lang.String, double);
  public com.feilong.lib.org.apache.http.params.HttpParams setDoubleParameter(java.lang.String, double);
  public boolean getBooleanParameter(java.lang.String, boolean);
  public com.feilong.lib.org.apache.http.params.HttpParams setBooleanParameter(java.lang.String, boolean);
  public boolean isParameterTrue(java.lang.String);
  public boolean isParameterFalse(java.lang.String);
  public java.util.Set<java.lang.String> getNames();
}
```

## `com.feilong.lib.org.apache.http.params.BasicHttpParams`

```java
public class com.feilong.lib.org.apache.http.params.BasicHttpParams extends com.feilong.lib.org.apache.http.params.AbstractHttpParams implements java.io.Serializable,java.lang.Cloneable {
  public com.feilong.lib.org.apache.http.params.BasicHttpParams();
  public java.lang.Object getParameter(java.lang.String);
  public com.feilong.lib.org.apache.http.params.HttpParams setParameter(java.lang.String, java.lang.Object);
  public boolean removeParameter(java.lang.String);
  public void setParameters(java.lang.String[], java.lang.Object);
  public boolean isParameterSet(java.lang.String);
  public boolean isParameterSetLocally(java.lang.String);
  public void clear();
  public com.feilong.lib.org.apache.http.params.HttpParams copy();
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
  public void copyParams(com.feilong.lib.org.apache.http.params.HttpParams);
  public java.util.Set<java.lang.String> getNames();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.params.HttpParams`

```java
public interface com.feilong.lib.org.apache.http.params.HttpParams {
  public abstract java.lang.Object getParameter(java.lang.String);
  public abstract com.feilong.lib.org.apache.http.params.HttpParams setParameter(java.lang.String, java.lang.Object);
  public abstract com.feilong.lib.org.apache.http.params.HttpParams copy();
  public abstract boolean removeParameter(java.lang.String);
  public abstract long getLongParameter(java.lang.String, long);
  public abstract com.feilong.lib.org.apache.http.params.HttpParams setLongParameter(java.lang.String, long);
  public abstract int getIntParameter(java.lang.String, int);
  public abstract com.feilong.lib.org.apache.http.params.HttpParams setIntParameter(java.lang.String, int);
  public abstract double getDoubleParameter(java.lang.String, double);
  public abstract com.feilong.lib.org.apache.http.params.HttpParams setDoubleParameter(java.lang.String, double);
  public abstract boolean getBooleanParameter(java.lang.String, boolean);
  public abstract com.feilong.lib.org.apache.http.params.HttpParams setBooleanParameter(java.lang.String, boolean);
  public abstract boolean isParameterTrue(java.lang.String);
  public abstract boolean isParameterFalse(java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.params.HttpParamsNames`

```java
public interface com.feilong.lib.org.apache.http.params.HttpParamsNames {
  public abstract java.util.Set<java.lang.String> getNames();
}
```
