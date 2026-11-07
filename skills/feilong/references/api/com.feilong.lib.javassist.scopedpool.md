# com.feilong.lib.javassist.scopedpool

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.javassist.scopedpool.ScopedClassPool`

```java
public class com.feilong.lib.javassist.scopedpool.ScopedClassPool extends com.feilong.lib.javassist.ClassPool {
  public java.lang.ClassLoader getClassLoader();
  public void close();
  public boolean isUnloadedClassLoader();
  public void lockInCache(com.feilong.lib.javassist.CtClass);
  public synchronized com.feilong.lib.javassist.CtClass getLocally(java.lang.String) throws com.feilong.lib.javassist.NotFoundException;
  public java.lang.Class<?> toClass(com.feilong.lib.javassist.CtClass, java.lang.ClassLoader, java.security.ProtectionDomain) throws com.feilong.lib.javassist.CannotCompileException;
}
```

## `com.feilong.lib.javassist.scopedpool.ScopedClassPoolFactory`

```java
public interface com.feilong.lib.javassist.scopedpool.ScopedClassPoolFactory {
  public abstract com.feilong.lib.javassist.scopedpool.ScopedClassPool create(java.lang.ClassLoader, com.feilong.lib.javassist.ClassPool, com.feilong.lib.javassist.scopedpool.ScopedClassPoolRepository);
  public abstract com.feilong.lib.javassist.scopedpool.ScopedClassPool create(com.feilong.lib.javassist.ClassPool, com.feilong.lib.javassist.scopedpool.ScopedClassPoolRepository);
}
```

## `com.feilong.lib.javassist.scopedpool.ScopedClassPoolFactoryImpl`

```java
public class com.feilong.lib.javassist.scopedpool.ScopedClassPoolFactoryImpl implements com.feilong.lib.javassist.scopedpool.ScopedClassPoolFactory {
  public com.feilong.lib.javassist.scopedpool.ScopedClassPoolFactoryImpl();
  public com.feilong.lib.javassist.scopedpool.ScopedClassPool create(java.lang.ClassLoader, com.feilong.lib.javassist.ClassPool, com.feilong.lib.javassist.scopedpool.ScopedClassPoolRepository);
  public com.feilong.lib.javassist.scopedpool.ScopedClassPool create(com.feilong.lib.javassist.ClassPool, com.feilong.lib.javassist.scopedpool.ScopedClassPoolRepository);
}
```

## `com.feilong.lib.javassist.scopedpool.ScopedClassPoolRepository`

```java
public interface com.feilong.lib.javassist.scopedpool.ScopedClassPoolRepository {
  public abstract void setClassPoolFactory(com.feilong.lib.javassist.scopedpool.ScopedClassPoolFactory);
  public abstract com.feilong.lib.javassist.scopedpool.ScopedClassPoolFactory getClassPoolFactory();
  public abstract boolean isPrune();
  public abstract void setPrune(boolean);
  public abstract com.feilong.lib.javassist.scopedpool.ScopedClassPool createScopedClassPool(java.lang.ClassLoader, com.feilong.lib.javassist.ClassPool);
  public abstract com.feilong.lib.javassist.ClassPool findClassPool(java.lang.ClassLoader);
  public abstract com.feilong.lib.javassist.ClassPool registerClassLoader(java.lang.ClassLoader);
  public abstract java.util.Map<java.lang.ClassLoader, com.feilong.lib.javassist.scopedpool.ScopedClassPool> getRegisteredCLs();
  public abstract void clearUnregisteredClassLoaders();
  public abstract void unregisterClassLoader(java.lang.ClassLoader);
}
```

## `com.feilong.lib.javassist.scopedpool.ScopedClassPoolRepositoryImpl`

```java
public class com.feilong.lib.javassist.scopedpool.ScopedClassPoolRepositoryImpl implements com.feilong.lib.javassist.scopedpool.ScopedClassPoolRepository {
  public static com.feilong.lib.javassist.scopedpool.ScopedClassPoolRepository getInstance();
  public boolean isPrune();
  public void setPrune(boolean);
  public com.feilong.lib.javassist.scopedpool.ScopedClassPool createScopedClassPool(java.lang.ClassLoader, com.feilong.lib.javassist.ClassPool);
  public com.feilong.lib.javassist.ClassPool findClassPool(java.lang.ClassLoader);
  public com.feilong.lib.javassist.ClassPool registerClassLoader(java.lang.ClassLoader);
  public java.util.Map<java.lang.ClassLoader, com.feilong.lib.javassist.scopedpool.ScopedClassPool> getRegisteredCLs();
  public void clearUnregisteredClassLoaders();
  public void unregisterClassLoader(java.lang.ClassLoader);
  public void insertDelegate(com.feilong.lib.javassist.scopedpool.ScopedClassPoolRepository);
  public void setClassPoolFactory(com.feilong.lib.javassist.scopedpool.ScopedClassPoolFactory);
  public com.feilong.lib.javassist.scopedpool.ScopedClassPoolFactory getClassPoolFactory();
}
```

## `com.feilong.lib.javassist.scopedpool.SoftValueHashMap`

```java
public class com.feilong.lib.javassist.scopedpool.SoftValueHashMap<K, V> implements java.util.Map<K, V> {
  public java.util.Set<java.util.Map$Entry<K, V>> entrySet();
  public com.feilong.lib.javassist.scopedpool.SoftValueHashMap(int, float);
  public com.feilong.lib.javassist.scopedpool.SoftValueHashMap(int);
  public com.feilong.lib.javassist.scopedpool.SoftValueHashMap();
  public com.feilong.lib.javassist.scopedpool.SoftValueHashMap(java.util.Map<K, V>);
  public int size();
  public boolean isEmpty();
  public boolean containsKey(java.lang.Object);
  public V get(java.lang.Object);
  public V put(K, V);
  public V remove(java.lang.Object);
  public void clear();
  public boolean containsValue(java.lang.Object);
  public java.util.Set<K> keySet();
  public void putAll(java.util.Map<? extends K, ? extends V>);
  public java.util.Collection<V> values();
}
```
