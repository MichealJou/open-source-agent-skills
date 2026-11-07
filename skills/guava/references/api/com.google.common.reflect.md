# com.google.common.reflect

版本：33.4.8-jre。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.google.common.reflect.AbstractInvocationHandler`

```java
public abstract class com.google.common.reflect.AbstractInvocationHandler implements java.lang.reflect.InvocationHandler {
  public com.google.common.reflect.AbstractInvocationHandler();
  public final java.lang.Object invoke(java.lang.Object, java.lang.reflect.Method, java.lang.Object[]) throws java.lang.Throwable;
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `com.google.common.reflect.ClassPath`

```java
public final class com.google.common.reflect.ClassPath {
  public static com.google.common.reflect.ClassPath from(java.lang.ClassLoader) throws java.io.IOException;
  public com.google.common.collect.ImmutableSet<com.google.common.reflect.ClassPath$ResourceInfo> getResources();
  public com.google.common.collect.ImmutableSet<com.google.common.reflect.ClassPath$ClassInfo> getAllClasses();
  public com.google.common.collect.ImmutableSet<com.google.common.reflect.ClassPath$ClassInfo> getTopLevelClasses();
  public com.google.common.collect.ImmutableSet<com.google.common.reflect.ClassPath$ClassInfo> getTopLevelClasses(java.lang.String);
  public com.google.common.collect.ImmutableSet<com.google.common.reflect.ClassPath$ClassInfo> getTopLevelClassesRecursive(java.lang.String);
}
```

## `com.google.common.reflect.ClassPath$ClassInfo`

```java
public final class com.google.common.reflect.ClassPath$ClassInfo extends com.google.common.reflect.ClassPath$ResourceInfo {
  public java.lang.String getPackageName();
  public java.lang.String getSimpleName();
  public java.lang.String getName();
  public boolean isTopLevel();
  public java.lang.Class<?> load();
  public java.lang.String toString();
}
```

## `com.google.common.reflect.ClassPath$ResourceInfo`

```java
public class com.google.common.reflect.ClassPath$ResourceInfo {
  public final java.net.URL url();
  public final com.google.common.io.ByteSource asByteSource();
  public final com.google.common.io.CharSource asCharSource(java.nio.charset.Charset);
  public final java.lang.String getResourceName();
  public int hashCode();
  public boolean equals(java.lang.Object);
  public java.lang.String toString();
}
```

## `com.google.common.reflect.ImmutableTypeToInstanceMap`

```java
public final class com.google.common.reflect.ImmutableTypeToInstanceMap<B> extends com.google.common.collect.ForwardingMap<com.google.common.reflect.TypeToken<? extends B>, B> implements com.google.common.reflect.TypeToInstanceMap<B> {
  public static <B> com.google.common.reflect.ImmutableTypeToInstanceMap<B> of();
  public static <B> com.google.common.reflect.ImmutableTypeToInstanceMap$Builder<B> builder();
  public <T extends B> T getInstance(com.google.common.reflect.TypeToken<T>);
  public <T extends B> T getInstance(java.lang.Class<T>);
  public <T extends B> T putInstance(com.google.common.reflect.TypeToken<T>, T);
  public <T extends B> T putInstance(java.lang.Class<T>, T);
  public B put(com.google.common.reflect.TypeToken<? extends B>, B);
  public void putAll(java.util.Map<? extends com.google.common.reflect.TypeToken<? extends B>, ? extends B>);
  public java.lang.Object put(java.lang.Object, java.lang.Object);
}
```

## `com.google.common.reflect.ImmutableTypeToInstanceMap$Builder`

```java
public final class com.google.common.reflect.ImmutableTypeToInstanceMap$Builder<B> {
  public <T extends B> com.google.common.reflect.ImmutableTypeToInstanceMap$Builder<B> put(java.lang.Class<T>, T);
  public <T extends B> com.google.common.reflect.ImmutableTypeToInstanceMap$Builder<B> put(com.google.common.reflect.TypeToken<T>, T);
  public com.google.common.reflect.ImmutableTypeToInstanceMap<B> build();
}
```

## `com.google.common.reflect.Invokable`

```java
public abstract class com.google.common.reflect.Invokable<T, R> implements java.lang.reflect.AnnotatedElement, java.lang.reflect.Member {
  public static com.google.common.reflect.Invokable<?, java.lang.Object> from(java.lang.reflect.Method);
  public static <T> com.google.common.reflect.Invokable<T, T> from(java.lang.reflect.Constructor<T>);
  public final boolean isAnnotationPresent(java.lang.Class<? extends java.lang.annotation.Annotation>);
  public final <A extends java.lang.annotation.Annotation> A getAnnotation(java.lang.Class<A>);
  public final java.lang.annotation.Annotation[] getAnnotations();
  public final java.lang.annotation.Annotation[] getDeclaredAnnotations();
  public abstract java.lang.reflect.TypeVariable<?>[] getTypeParameters();
  public final void setAccessible(boolean);
  public final boolean trySetAccessible();
  public final boolean isAccessible();
  public final java.lang.String getName();
  public final int getModifiers();
  public final boolean isSynthetic();
  public final boolean isPublic();
  public final boolean isProtected();
  public final boolean isPackagePrivate();
  public final boolean isPrivate();
  public final boolean isStatic();
  public final boolean isFinal();
  public final boolean isAbstract();
  public final boolean isNative();
  public final boolean isSynchronized();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
  public abstract boolean isOverridable();
  public abstract boolean isVarArgs();
  public final R invoke(T, java.lang.Object...) throws java.lang.reflect.InvocationTargetException, java.lang.IllegalAccessException;
  public final com.google.common.reflect.TypeToken<? extends R> getReturnType();
  public final com.google.common.collect.ImmutableList<com.google.common.reflect.Parameter> getParameters();
  public final com.google.common.collect.ImmutableList<com.google.common.reflect.TypeToken<? extends java.lang.Throwable>> getExceptionTypes();
  public final <R1 extends R> com.google.common.reflect.Invokable<T, R1> returning(java.lang.Class<R1>);
  public final <R1 extends R> com.google.common.reflect.Invokable<T, R1> returning(com.google.common.reflect.TypeToken<R1>);
  public final java.lang.Class<? super T> getDeclaringClass();
  public com.google.common.reflect.TypeToken<T> getOwnerType();
  public abstract java.lang.reflect.AnnotatedType getAnnotatedReturnType();
}
```

## `com.google.common.reflect.MutableTypeToInstanceMap`

```java
public final class com.google.common.reflect.MutableTypeToInstanceMap<B> extends com.google.common.collect.ForwardingMap<com.google.common.reflect.TypeToken<? extends B>, B> implements com.google.common.reflect.TypeToInstanceMap<B> {
  public com.google.common.reflect.MutableTypeToInstanceMap();
  public <T extends B> T getInstance(java.lang.Class<T>);
  public <T extends B> T getInstance(com.google.common.reflect.TypeToken<T>);
  public <T extends B> T putInstance(java.lang.Class<T>, T);
  public <T extends B> T putInstance(com.google.common.reflect.TypeToken<T>, T);
  public B put(com.google.common.reflect.TypeToken<? extends B>, B);
  public void putAll(java.util.Map<? extends com.google.common.reflect.TypeToken<? extends B>, ? extends B>);
  public java.util.Set<java.util.Map$Entry<com.google.common.reflect.TypeToken<? extends B>, B>> entrySet();
  public java.lang.Object put(java.lang.Object, java.lang.Object);
}
```

## `com.google.common.reflect.Parameter`

```java
public final class com.google.common.reflect.Parameter implements java.lang.reflect.AnnotatedElement {
  public com.google.common.reflect.TypeToken<?> getType();
  public com.google.common.reflect.Invokable<?, ?> getDeclaringInvokable();
  public boolean isAnnotationPresent(java.lang.Class<? extends java.lang.annotation.Annotation>);
  public <A extends java.lang.annotation.Annotation> A getAnnotation(java.lang.Class<A>);
  public java.lang.annotation.Annotation[] getAnnotations();
  public <A extends java.lang.annotation.Annotation> A[] getAnnotationsByType(java.lang.Class<A>);
  public java.lang.annotation.Annotation[] getDeclaredAnnotations();
  public <A extends java.lang.annotation.Annotation> A getDeclaredAnnotation(java.lang.Class<A>);
  public <A extends java.lang.annotation.Annotation> A[] getDeclaredAnnotationsByType(java.lang.Class<A>);
  public java.lang.reflect.AnnotatedType getAnnotatedType();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `com.google.common.reflect.Reflection`

```java
public final class com.google.common.reflect.Reflection {
  public static java.lang.String getPackageName(java.lang.Class<?>);
  public static java.lang.String getPackageName(java.lang.String);
  public static void initialize(java.lang.Class<?>...);
  public static <T> T newProxy(java.lang.Class<T>, java.lang.reflect.InvocationHandler);
}
```

## `com.google.common.reflect.TypeParameter`

```java
public abstract class com.google.common.reflect.TypeParameter<T> extends com.google.common.reflect.TypeCapture<T> {
  public final int hashCode();
  public final boolean equals(java.lang.Object);
  public java.lang.String toString();
}
```

## `com.google.common.reflect.TypeResolver`

```java
public final class com.google.common.reflect.TypeResolver {
  public com.google.common.reflect.TypeResolver();
  public com.google.common.reflect.TypeResolver where(java.lang.reflect.Type, java.lang.reflect.Type);
  public java.lang.reflect.Type resolveType(java.lang.reflect.Type);
}
```

## `com.google.common.reflect.TypeToInstanceMap`

```java
public interface com.google.common.reflect.TypeToInstanceMap<B> extends java.util.Map<com.google.common.reflect.TypeToken<? extends B>, B> {
  public abstract <T extends B> T getInstance(java.lang.Class<T>);
  public abstract <T extends B> T getInstance(com.google.common.reflect.TypeToken<T>);
  public abstract <T extends B> T putInstance(java.lang.Class<T>, T);
  public abstract <T extends B> T putInstance(com.google.common.reflect.TypeToken<T>, T);
}
```

## `com.google.common.reflect.TypeToken`

```java
public abstract class com.google.common.reflect.TypeToken<T> extends com.google.common.reflect.TypeCapture<T> implements java.io.Serializable {
  public static <T> com.google.common.reflect.TypeToken<T> of(java.lang.Class<T>);
  public static com.google.common.reflect.TypeToken<?> of(java.lang.reflect.Type);
  public final java.lang.Class<? super T> getRawType();
  public final java.lang.reflect.Type getType();
  public final <X> com.google.common.reflect.TypeToken<T> where(com.google.common.reflect.TypeParameter<X>, com.google.common.reflect.TypeToken<X>);
  public final <X> com.google.common.reflect.TypeToken<T> where(com.google.common.reflect.TypeParameter<X>, java.lang.Class<X>);
  public final com.google.common.reflect.TypeToken<?> resolveType(java.lang.reflect.Type);
  public final com.google.common.reflect.TypeToken<T>.TypeSet getTypes();
  public final com.google.common.reflect.TypeToken<? super T> getSupertype(java.lang.Class<? super T>);
  public final com.google.common.reflect.TypeToken<? extends T> getSubtype(java.lang.Class<?>);
  public final boolean isSupertypeOf(com.google.common.reflect.TypeToken<?>);
  public final boolean isSupertypeOf(java.lang.reflect.Type);
  public final boolean isSubtypeOf(com.google.common.reflect.TypeToken<?>);
  public final boolean isSubtypeOf(java.lang.reflect.Type);
  public final boolean isArray();
  public final boolean isPrimitive();
  public final com.google.common.reflect.TypeToken<T> wrap();
  public final com.google.common.reflect.TypeToken<T> unwrap();
  public final com.google.common.reflect.TypeToken<?> getComponentType();
  public final com.google.common.reflect.Invokable<T, java.lang.Object> method(java.lang.reflect.Method);
  public final com.google.common.reflect.Invokable<T, T> constructor(java.lang.reflect.Constructor<?>);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `com.google.common.reflect.TypeToken$TypeSet`

```java
public class com.google.common.reflect.TypeToken$TypeSet extends com.google.common.collect.ForwardingSet<com.google.common.reflect.TypeToken<? super T>> implements java.io.Serializable {
  public com.google.common.reflect.TypeToken<T>.TypeSet interfaces();
  public com.google.common.reflect.TypeToken<T>.TypeSet classes();
  public java.util.Set<java.lang.Class<? super T>> rawTypes();
}
```
