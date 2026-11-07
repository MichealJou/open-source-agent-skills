# com.google.common.reflect

版本 33.4.8-jre。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.google.common.reflect.AbstractInvocationHandler` | `Object invoke(Object proxy,Method method,@Nullable
Object @Nullable [] args)` | 【原文待译】{@inheritDoc} proxy.hashCode() delegates to AbstractInvocationHandler#hashCode proxy.toString() delegates to AbstractInvocationHandler#toString proxy.equals(argument) returns true if: proxy and argument are of the same type and AbstractInvocationHandler#equals returns true for the InvocationHandler … |
| `com.google.common.reflect.AbstractInvocationHandler` | `String toString()` | 【原文待译】By default delegates to Object#toString. The dynamic proxies' toString() will delegate to this method. Subclasses can override this method to provide custom string representation for the proxies. |
| `com.google.common.reflect.AbstractInvocationHandler` | `boolean equals(@Nullable
Object obj)` | 【原文待译】By default delegates to Object#equals so instances are only equal if they are identical. proxy.equals(argument) returns true if: proxy and argument are of the same type and this method returns true for the InvocationHandler of argument Subclasses can override this method to provide custom equality. |
| `com.google.common.reflect.AbstractInvocationHandler` | `int hashCode()` | 【原文待译】By default delegates to Object#hashCode. The dynamic proxies' hashCode() will delegate to this method. Subclasses can override this method to provide custom equality. |
| `com.google.common.reflect.ClassPath` | `ClassPath from(ClassLoader classloader)` | 【原文待译】Returns a ClassPath representing all classes and resources loadable from classloader and its ancestor class loaders. Warning: ClassPath can find classes and resources only from: URLClassLoader instances' file: URLs the {@linkplain ClassLoader#getSystemClassLoader() system class loader}. To search th… |
| `com.google.common.reflect.ClassPath` | `ImmutableSet<ClassInfo> getAllClasses()` | 【原文待译】Returns all classes loadable from the current class path. |
| `com.google.common.reflect.ClassPath` | `ImmutableSet<ClassInfo> getTopLevelClasses()` | 【原文待译】Returns all top level classes loadable from the current class path. Note that "top-level-ness" is determined heuristically by class name (see ClassInfo#isTopLevel). |
| `com.google.common.reflect.ClassPath` | `ImmutableSet<ClassInfo> getTopLevelClasses(String packageName)` | 【原文待译】Returns all top level classes whose package name is packageName. |
| `com.google.common.reflect.ClassPath` | `ImmutableSet<ClassInfo> getTopLevelClassesRecursive(String packageName)` | 【原文待译】Returns all top level classes whose package name is packageName or starts with packageName followed by a '.'. |
| `com.google.common.reflect.ClassPath` | `ImmutableSet<ResourceInfo> getResources()` | 【原文待译】Returns all resources loadable from the current class path, including the class files of all loadable classes but excluding the "META-INF/MANIFEST.MF" file. |
| `com.google.common.reflect.ClassPath$ClassInfo` | `Class<?> load()` | 【原文待译】Loads (but doesn't link or initialize) the class. |
| `com.google.common.reflect.ClassPath$ClassInfo` | `String getName()` | 【原文待译】Returns the fully qualified name of the class. Behaves identically to Class#getName() but does not require the class to be loaded. |
| `com.google.common.reflect.ClassPath$ClassInfo` | `String getPackageName()` | 【原文待译】Returns the package name of the class, without attempting to load the class. Behaves similarly to class.getPackage().Package#getName() getName() but does not require the class (or package) to be loaded. But note that this method may behave differently for a class in the default package: For such cla… |
| `com.google.common.reflect.ClassPath$ClassInfo` | `String getSimpleName()` | 【原文待译】Returns the simple name of the underlying class as given in the source code. Behaves similarly to Class#getSimpleName() but does not require the class to be loaded. But note that this class uses heuristics to identify the simple name. See a related discussion in issue 3349 . |
| `com.google.common.reflect.ClassPath$ClassInfo` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.ClassPath$ClassInfo` | `boolean isTopLevel()` | 【原文待译】Returns true if the class name "looks to be" top level (not nested), that is, it includes no '$' in the name. This method may return false for a top-level class that's intentionally named with the '$' character. If this is a concern, you could use #load and then check on the loaded Class object inst… |
| `com.google.common.reflect.ClassPath$ResourceInfo` | `ByteSource asByteSource()` | 【原文待译】Returns a ByteSource view of the resource from which its bytes can be read. |
| `com.google.common.reflect.ClassPath$ResourceInfo` | `CharSource asCharSource(Charset charset)` | 【原文待译】Returns a CharSource view of the resource from which its bytes can be read as characters decoded with the given charset. |
| `com.google.common.reflect.ClassPath$ResourceInfo` | `String getResourceName()` | 【原文待译】Returns the fully qualified name of the resource. Such as "com/mycomp/foo/bar.txt". |
| `com.google.common.reflect.ClassPath$ResourceInfo` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.ClassPath$ResourceInfo` | `URL url()` | 【原文待译】Returns the url identifying the resource. See ClassLoader#getResource |
| `com.google.common.reflect.ClassPath$ResourceInfo` | `boolean equals(@Nullable
Object obj)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.ClassPath$ResourceInfo` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.ImmutableTypeToInstanceMap` | `B put(TypeToken<? extends B> key,B value)` | 【原文待译】Guaranteed to throw an exception and leave the map unmodified. |
| `com.google.common.reflect.ImmutableTypeToInstanceMap` | `Builder<B> builder()` | 【原文待译】Returns a new builder. |
| `com.google.common.reflect.ImmutableTypeToInstanceMap` | `ImmutableTypeToInstanceMap<B> of()` | 【原文待译】Returns an empty type to instance map. |
| `com.google.common.reflect.ImmutableTypeToInstanceMap` | `T getInstance(Class<T> type)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.ImmutableTypeToInstanceMap` | `T getInstance(TypeToken<T> type)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.ImmutableTypeToInstanceMap` | `T putInstance(Class<T> type,T value)` | 【原文待译】Guaranteed to throw an exception and leave the map unmodified. |
| `com.google.common.reflect.ImmutableTypeToInstanceMap` | `T putInstance(TypeToken<T> type,T value)` | 【原文待译】Guaranteed to throw an exception and leave the map unmodified. |
| `com.google.common.reflect.ImmutableTypeToInstanceMap` | `void putAll(Map<? extends TypeToken<? extends B>, ? extends B> map)` | 【原文待译】Guaranteed to throw an exception and leave the map unmodified. |
| `com.google.common.reflect.ImmutableTypeToInstanceMap$Builder` | `Builder<B> put(Class<T> key,T value)` | 【原文待译】Associates key with value in the built map. Duplicate keys are not allowed, and will cause #build to fail. |
| `com.google.common.reflect.ImmutableTypeToInstanceMap$Builder` | `Builder<B> put(TypeToken<T> key,T value)` | 【原文待译】Associates key with value in the built map. Duplicate keys are not allowed, and will cause #build to fail. |
| `com.google.common.reflect.ImmutableTypeToInstanceMap$Builder` | `ImmutableTypeToInstanceMap<B> build()` | 【原文待译】Returns a new immutable type-to-instance map containing the entries provided to this builder. |
| `com.google.common.reflect.Invokable` | `A getAnnotation(Class<A> annotationClass)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.Invokable` | `AnnotatedType getAnnotatedReturnType()` | 【原文待译】Returns the AnnotatedType for the return type. |
| `com.google.common.reflect.Invokable` | `Annotation[] getAnnotations()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.Invokable` | `Annotation[] getDeclaredAnnotations()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.Invokable` | `Class<? super T> getDeclaringClass()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.Invokable` | `ImmutableList<Parameter> getParameters()` | 【原文待译】Returns all declared parameters of this Invokable. Note that if this is a constructor of a non-static inner class, unlike Constructor#getParameterTypes, the hidden this parameter of the enclosing class is excluded from the returned parameters. |
| `com.google.common.reflect.Invokable` | `ImmutableList<TypeToken<? extends Throwable>> getExceptionTypes()` | 【原文待译】Returns all declared exception types of this Invokable. |
| `com.google.common.reflect.Invokable` | `Invokable<?, Object> from(Method method)` | 【原文待译】Returns Invokable of method. |
| `com.google.common.reflect.Invokable` | `Invokable<T, R1> returning(Class<R1> returnType)` | 【原文待译】Explicitly specifies the return type of this Invokable. For example: {@snippet : Method factoryMethod = Person.class.getMethod("create"); Invokable factory = Invokable.of(getNameMethod).returning(Person.class); } |
| `com.google.common.reflect.Invokable` | `Invokable<T, R1> returning(TypeToken<R1> returnType)` | 【原文待译】Explicitly specifies the return type of this Invokable. |
| `com.google.common.reflect.Invokable` | `Invokable<T, T> from(Constructor<T> constructor)` | 【原文待译】Returns Invokable of constructor. |
| `com.google.common.reflect.Invokable` | `R invoke(@Nullable
T receiver,@Nullable
Object... args)` | 【原文待译】Invokes with receiver as 'this' and args passed to the underlying method and returns the return value; or calls the underlying constructor with args and returns the constructed instance. |
| `com.google.common.reflect.Invokable` | `String getName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.Invokable` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.Invokable` | `TypeToken<? extends R> getReturnType()` | 【原文待译】Returns the return type of this Invokable. |
| `com.google.common.reflect.Invokable` | `TypeToken<T> getOwnerType()` | 【原文待译】Returns the type of T. |
| `com.google.common.reflect.Invokable` | `TypeVariable<?>[] getTypeParameters()` | 【原文待译】See java.lang.reflect.GenericDeclaration#getTypeParameters(). |
| `com.google.common.reflect.Invokable` | `boolean equals(@Nullable
Object obj)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.Invokable` | `boolean isAbstract()` | 【原文待译】Returns true if the method is abstract. |
| `com.google.common.reflect.Invokable` | `boolean isAccessible()` | 【原文待译】See java.lang.reflect.AccessibleObject#isAccessible(). |
| `com.google.common.reflect.Invokable` | `boolean isAnnotationPresent(Class<? extends Annotation> annotationClass)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.Invokable` | `boolean isFinal()` | 【原文待译】Returns true if this method is final, per Modifier.isFinal(getModifiers()). Note that a method may still be effectively "final", or non-overridable when it has no final keyword. For example, it could be private, or it could be declared by a final class. To tell whether a method is overridable, use I… |
| `com.google.common.reflect.Invokable` | `boolean isNative()` | 【原文待译】Returns true if the element is native. |
| `com.google.common.reflect.Invokable` | `boolean isOverridable()` | 【原文待译】Returns true if this is an overridable method. Constructors, private, static or final methods, or methods declared by final classes are not overridable. |
| `com.google.common.reflect.Invokable` | `boolean isPackagePrivate()` | 【原文待译】Returns true if the element is package-private. |
| `com.google.common.reflect.Invokable` | `boolean isPrivate()` | 【原文待译】Returns true if the element is private. |
| `com.google.common.reflect.Invokable` | `boolean isProtected()` | 【原文待译】Returns true if the element is protected. |
| `com.google.common.reflect.Invokable` | `boolean isPublic()` | 【原文待译】Returns true if the element is public. |
| `com.google.common.reflect.Invokable` | `boolean isStatic()` | 【原文待译】Returns true if the element is static. |
| `com.google.common.reflect.Invokable` | `boolean isSynchronized()` | 【原文待译】Returns true if the method is synchronized. |
| `com.google.common.reflect.Invokable` | `boolean isSynthetic()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.Invokable` | `boolean isVarArgs()` | 【原文待译】Returns true if this was declared to take a variable number of arguments. |
| `com.google.common.reflect.Invokable` | `boolean trySetAccessible()` | 【原文待译】See java.lang.reflect.AccessibleObject#trySetAccessible(). |
| `com.google.common.reflect.Invokable` | `int getModifiers()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.Invokable` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.Invokable` | `void setAccessible(boolean flag)` | 【原文待译】See java.lang.reflect.AccessibleObject#setAccessible(boolean). |
| `com.google.common.reflect.MutableTypeToInstanceMap` | `B put(TypeToken<? extends @NonNull B> key,@ParametricNullness
B value)` | 【原文待译】Not supported. Use #putInstance instead. |
| `com.google.common.reflect.MutableTypeToInstanceMap` | `Set<Entry<TypeToken<? extends @NonNull B>, B>> entrySet()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.MutableTypeToInstanceMap` | `T getInstance(Class<T> type)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.MutableTypeToInstanceMap` | `T getInstance(TypeToken<T> type)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.MutableTypeToInstanceMap` | `T putInstance(Class<@NonNull T> type,@ParametricNullness
T value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.MutableTypeToInstanceMap` | `T putInstance(TypeToken<@NonNull T> type,@ParametricNullness
T value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.MutableTypeToInstanceMap` | `void putAll(Map<? extends TypeToken<? extends @NonNull B>, ? extends B> map)` | 【原文待译】Not supported. Use #putInstance instead. |
| `com.google.common.reflect.Parameter` | `A getAnnotation(Class<A> annotationType)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.Parameter` | `A getDeclaredAnnotation(Class<A> annotationType)` | 【原文待译】@since 18.0 |
| `com.google.common.reflect.Parameter` | `A[] getAnnotationsByType(Class<A> annotationType)` | 【原文待译】@since 18.0 |
| `com.google.common.reflect.Parameter` | `A[] getDeclaredAnnotationsByType(Class<A> annotationType)` | 【原文待译】@since 18.0 |
| `com.google.common.reflect.Parameter` | `AnnotatedType getAnnotatedType()` | 【原文待译】Returns the AnnotatedType of the parameter. |
| `com.google.common.reflect.Parameter` | `Annotation[] getAnnotations()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.Parameter` | `Annotation[] getDeclaredAnnotations()` | 【原文待译】@since 18.0 |
| `com.google.common.reflect.Parameter` | `Invokable<?, ?> getDeclaringInvokable()` | 【原文待译】Returns the Invokable that declares this parameter. |
| `com.google.common.reflect.Parameter` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.Parameter` | `TypeToken<?> getType()` | 【原文待译】Returns the type of the parameter. |
| `com.google.common.reflect.Parameter` | `boolean equals(@Nullable
Object obj)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.Parameter` | `boolean isAnnotationPresent(Class<? extends Annotation> annotationType)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.Parameter` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.Reflection` | `String getPackageName(Class<?> clazz)` | 【原文待译】Returns the package name of clazz according to the Java Language Specification (section 6.7). Unlike Class#getPackage, this method only parses the class name, without attempting to define the Package and hence load files. |
| `com.google.common.reflect.Reflection` | `String getPackageName(String classFullName)` | 【原文待译】Returns the package name of classFullName according to the Java Language Specification (section 6.7). Unlike Class#getPackage, this method only parses the class name, without attempting to define the Package and hence load files. |
| `com.google.common.reflect.Reflection` | `T newProxy(Class<T> interfaceType,InvocationHandler handler)` | 【原文待译】Returns a proxy instance that implements interfaceType by dispatching method invocations to handler. The class loader of interfaceType will be used to define the proxy class. To implement multiple interfaces or specify a class loader, use Proxy#newProxyInstance. |
| `com.google.common.reflect.Reflection` | `void initialize(Class<?>... classes)` | 【原文待译】Ensures that the given classes are initialized, as described in JLS Section 12.4.2 . WARNING: Normally it's a smell if a class needs to be explicitly initialized, because static state hurts system maintainability and testability. In cases when you have no choice while interoperating with a legacy fr… |
| `com.google.common.reflect.TypeParameter` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.TypeParameter` | `boolean equals(@Nullable
Object o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.TypeParameter` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.TypeResolver` | `Type resolveType(Type type)` | 【原文待译】Resolves all type variables in type and all downstream types and returns a corresponding type with type variables resolved. |
| `com.google.common.reflect.TypeResolver` | `TypeResolver where(Type formal,Type actual)` | 【原文待译】Returns a new TypeResolver with type variables in formal mapping to types in actual. For example, if formal is a TypeVariable T, and actual is String.class, then new TypeResolver().where(formal, actual) will {@linkplain #resolveType resolve} ParameterizedType List to List , and resolve Map to Map et… |
| `com.google.common.reflect.TypeToInstanceMap` | `T getInstance(Class<T> type)` | 【原文待译】Returns the value the specified class is mapped to, or null if no entry for this class is present. This will only return a value that was bound to this specific class, not a value that may have been bound to a subtype. getInstance(Foo.class) is equivalent to getInstance(TypeToken.of(Foo.class)). |
| `com.google.common.reflect.TypeToInstanceMap` | `T getInstance(TypeToken<T> type)` | 【原文待译】Returns the value the specified type is mapped to, or null if no entry for this type is present. This will only return a value that was bound to this specific type, not a value that may have been bound to a subtype. |
| `com.google.common.reflect.TypeToInstanceMap` | `T putInstance(Class<@NonNull T> type,@ParametricNullness
T value)` | 【原文待译】Maps the specified class to the specified value. Does not associate this value with any of the class's supertypes. putInstance(Foo.class, foo) is equivalent to putInstance(TypeToken.of(Foo.class), foo). |
| `com.google.common.reflect.TypeToInstanceMap` | `T putInstance(TypeToken<@NonNull T> type,@ParametricNullness
T value)` | 【原文待译】Maps the specified type to the specified value. Does not associate this value with any of the type's supertypes. |
| `com.google.common.reflect.TypeToken` | `Class<? super T> getRawType()` | 【原文待译】Returns the raw type of T. Formally speaking, if T is returned by java.lang.reflect.Method#getGenericReturnType, the raw type is what's returned by java.lang.reflect.Method#getReturnType of the same method object. Specifically: If T is a Class itself, T itself is returned. If T is a ParameterizedTyp… |
| `com.google.common.reflect.TypeToken` | `Invokable<T, Object> method(Method method)` | 【原文待译】Returns the Invokable for method, which must be a member of T. |
| `com.google.common.reflect.TypeToken` | `Invokable<T, T> constructor(Constructor<?> constructor)` | 【原文待译】Returns the Invokable for constructor, which must be a member of T. |
| `com.google.common.reflect.TypeToken` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.TypeToken` | `Type getType()` | 【原文待译】Returns the represented type. |
| `com.google.common.reflect.TypeToken` | `TypeSet getTypes()` | 【原文待译】Returns the set of interfaces and classes that this type is or is a subtype of. The returned types are parameterized with proper type arguments. Subtypes are always listed before supertypes. But the reverse is not true. A type isn't necessarily a subtype of all the types following. Order between typ… |
| `com.google.common.reflect.TypeToken` | `TypeToken<? extends T> getSubtype(Class<?> subclass)` | 【原文待译】Returns subtype of this with subclass as the raw class. For example, if this is Iterable and subclass is List, List is returned. |
| `com.google.common.reflect.TypeToken` | `TypeToken<? super T> getSupertype(Class<? super T> superclass)` | 【原文待译】Returns the generic form of superclass. For example, if this is ArrayList , Iterable is returned given the input Iterable.class. |
| `com.google.common.reflect.TypeToken` | `TypeToken<?> getComponentType()` | 【原文待译】Returns the array component type if this type represents an array (int[], T[], []> etc.), or else null is returned. |
| `com.google.common.reflect.TypeToken` | `TypeToken<?> of(Type type)` | 【原文待译】Returns an instance of type token that wraps type. |
| `com.google.common.reflect.TypeToken` | `TypeToken<?> resolveType(Type type)` | 【原文待译】Resolves the given type against the type context represented by this type. For example: {@snippet : new TypeToken >() {}.resolveType( List.class.getMethod("get", int.class).getGenericReturnType()) => String.class } |
| `com.google.common.reflect.TypeToken` | `TypeToken<T> of(Class<T> type)` | 【原文待译】Returns an instance of type token that wraps type. |
| `com.google.common.reflect.TypeToken` | `TypeToken<T> unwrap()` | 【原文待译】Returns the corresponding primitive type if this is a wrapper type; otherwise returns this itself. Idempotent. |
| `com.google.common.reflect.TypeToken` | `TypeToken<T> where(TypeParameter<X> typeParam,Class<X> typeArg)` | 【原文待译】Returns a new TypeToken where type variables represented by typeParam are substituted by typeArg. For example, it can be used to construct Map for any K and V type: {@snippet : static TypeToken > mapOf( Class keyType, Class valueType) { return new TypeToken >() {} .where(new TypeParameter () {}, key… |
| `com.google.common.reflect.TypeToken` | `TypeToken<T> where(TypeParameter<X> typeParam,TypeToken<X> typeArg)` | 【原文待译】Returns a new TypeToken where type variables represented by typeParam are substituted by typeArg. For example, it can be used to construct Map for any K and V type: {@snippet : static TypeToken > mapOf( TypeToken keyType, TypeToken valueType) { return new TypeToken >() {} .where(new TypeParameter ()… |
| `com.google.common.reflect.TypeToken` | `TypeToken<T> wrap()` | 【原文待译】Returns the corresponding wrapper type if this is a primitive type; otherwise returns this itself. Idempotent. |
| `com.google.common.reflect.TypeToken` | `boolean equals(@Nullable
Object o)` | 【原文待译】Returns true if o is another TypeToken that represents the same Type. |
| `com.google.common.reflect.TypeToken` | `boolean isArray()` | 【原文待译】Returns true if this type is known to be an array type, such as int[], T[], []> etc. |
| `com.google.common.reflect.TypeToken` | `boolean isPrimitive()` | 【原文待译】Returns true if this type is one of the nine primitive types (including void). |
| `com.google.common.reflect.TypeToken` | `boolean isSubtypeOf(Type supertype)` | 【原文待译】Returns true if this type is a subtype of the given type. "Subtype" is defined according to the rules for type arguments introduced with Java generics. |
| `com.google.common.reflect.TypeToken` | `boolean isSubtypeOf(TypeToken<?> type)` | 【原文待译】Returns true if this type is a subtype of the given type. "Subtype" is defined according to the rules for type arguments introduced with Java generics. |
| `com.google.common.reflect.TypeToken` | `boolean isSupertypeOf(Type type)` | 【原文待译】Returns true if this type is a supertype of the given type. "Supertype" is defined according to the rules for type arguments introduced with Java generics. |
| `com.google.common.reflect.TypeToken` | `boolean isSupertypeOf(TypeToken<?> type)` | 【原文待译】Returns true if this type is a supertype of the given type. "Supertype" is defined according to the rules for type arguments introduced with Java generics. |
| `com.google.common.reflect.TypeToken` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.reflect.TypeToken$TypeSet` | `Set<Class<? super T>> rawTypes()` | 【原文待译】Returns the raw types of the types in this set, in the same order. |
| `com.google.common.reflect.TypeToken$TypeSet` | `TypeSet classes()` | 【原文待译】Returns the types that are classes. |
| `com.google.common.reflect.TypeToken$TypeSet` | `TypeSet interfaces()` | 【原文待译】Returns the types that are interfaces implemented by this type. |
