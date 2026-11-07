# com.feilong.lib.ezmorph.bean

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.ezmorph.bean.BeanMorpher`

```java
public final class com.feilong.lib.ezmorph.bean.BeanMorpher implements com.feilong.lib.ezmorph.ObjectMorpher {
  public com.feilong.lib.ezmorph.bean.BeanMorpher(java.lang.Class<?>, com.feilong.lib.ezmorph.MorpherRegistry);
  public java.lang.Object morph(java.lang.Object);
  public java.lang.Class<?> morphsTo();
  public boolean supports(java.lang.Class<?>);
}
```

## `com.feilong.lib.ezmorph.bean.MorphDynaBean`

```java
public final class com.feilong.lib.ezmorph.bean.MorphDynaBean implements org.apache.commons.beanutils.DynaBean,java.io.Serializable {
  public com.feilong.lib.ezmorph.bean.MorphDynaBean();
  public com.feilong.lib.ezmorph.bean.MorphDynaBean(com.feilong.lib.ezmorph.MorpherRegistry);
  public boolean contains(java.lang.String, java.lang.String);
  public boolean equals(java.lang.Object);
  public java.lang.Object get(java.lang.String);
  public java.lang.Object get(java.lang.String, int);
  public java.lang.Object get(java.lang.String, java.lang.String);
  public com.feilong.lib.beanutils.DynaClass getDynaClass();
  public com.feilong.lib.ezmorph.MorpherRegistry getMorpherRegistry();
  public int hashCode();
  public void remove(java.lang.String, java.lang.String);
  public void set(java.lang.String, int, java.lang.Object);
  public void set(java.lang.String, java.lang.Object);
  public void set(java.lang.String, java.lang.String, java.lang.Object);
  public synchronized void setDynaBeanClass(com.feilong.lib.ezmorph.bean.MorphDynaClass);
  public void setMorpherRegistry(com.feilong.lib.ezmorph.MorpherRegistry);
  public java.lang.String toString();
}
```

## `com.feilong.lib.ezmorph.bean.MorphDynaClass`

```java
public final class com.feilong.lib.ezmorph.bean.MorphDynaClass implements com.feilong.lib.beanutils.DynaClass,java.io.Serializable {
  public com.feilong.lib.ezmorph.bean.MorphDynaClass(java.util.Map);
  public com.feilong.lib.ezmorph.bean.MorphDynaClass(java.util.Map, boolean);
  public com.feilong.lib.ezmorph.bean.MorphDynaClass(java.lang.String, java.lang.Class<?>, java.util.Map);
  public com.feilong.lib.ezmorph.bean.MorphDynaClass(java.lang.String, java.lang.Class<?>, java.util.Map, boolean);
  public boolean equals(java.lang.Object);
  public com.feilong.lib.beanutils.DynaProperty[] getDynaProperties();
  public com.feilong.lib.beanutils.DynaProperty getDynaProperty(java.lang.String);
  public java.lang.String getName();
  public int hashCode();
  public org.apache.commons.beanutils.DynaBean newInstance() throws java.lang.IllegalAccessException, java.lang.InstantiationException;
  public java.lang.String toString();
}
```
