# com.google.common.base

版本 33.4.8-jre。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.google.common.base.Ascii` | `String toLowerCase(CharSequence chars)` | 【原文待译】Returns a copy of the input character sequence in which all {@linkplain #isUpperCase(char) uppercase ASCII characters} have been converted to lowercase. All other characters are copied without modification. |
| `com.google.common.base.Ascii` | `String toLowerCase(String string)` | 【原文待译】Returns a copy of the input string in which all {@linkplain #isUpperCase(char) uppercase ASCII characters} have been converted to lowercase. All other characters are copied without modification. |
| `com.google.common.base.Ascii` | `String toUpperCase(CharSequence chars)` | 【原文待译】Returns a copy of the input character sequence in which all {@linkplain #isLowerCase(char) lowercase ASCII characters} have been converted to uppercase. All other characters are copied without modification. |
| `com.google.common.base.Ascii` | `String toUpperCase(String string)` | 【原文待译】Returns a copy of the input string in which all {@linkplain #isLowerCase(char) lowercase ASCII characters} have been converted to uppercase. All other characters are copied without modification. |
| `com.google.common.base.Ascii` | `String truncate(CharSequence seq,int maxLength,String truncationIndicator)` | 【原文待译】Truncates the given character sequence to the given maximum length. If the length of the sequence is greater than maxLength, the returned string will be exactly maxLength chars in length and will end with the given truncationIndicator. Otherwise, the sequence will be returned as a string with no cha… |
| `com.google.common.base.Ascii` | `boolean equalsIgnoreCase(CharSequence s1,CharSequence s2)` | 【原文待译】Indicates whether the contents of the given character sequences s1 and s2 are equal, ignoring the case of any ASCII alphabetic characters between 'a' and 'z' or 'A' and 'Z' inclusive. This method is significantly faster than String#equalsIgnoreCase and should be used in preference if at least one of… |
| `com.google.common.base.Ascii` | `boolean isLowerCase(char c)` | 【原文待译】Indicates whether c is one of the twenty-six lowercase ASCII alphabetic characters between 'a' and 'z' inclusive. All others (including non-ASCII characters) return false. |
| `com.google.common.base.Ascii` | `boolean isUpperCase(char c)` | 【原文待译】Indicates whether c is one of the twenty-six uppercase ASCII alphabetic characters between 'A' and 'Z' inclusive. All others (including non-ASCII characters) return false. |
| `com.google.common.base.Ascii` | `char toLowerCase(char c)` | 【原文待译】If the argument is an {@linkplain #isUpperCase(char) uppercase ASCII character}, returns the lowercase equivalent. Otherwise returns the argument. |
| `com.google.common.base.Ascii` | `char toUpperCase(char c)` | 【原文待译】If the argument is a {@linkplain #isLowerCase(char) lowercase ASCII character}, returns the uppercase equivalent. Otherwise returns the argument. |
| `com.google.common.base.CaseFormat` | `Converter<String, String> converterTo(CaseFormat targetFormat)` | 【原文待译】Returns a serializable Converter that converts strings from this format to targetFormat. |
| `com.google.common.base.CaseFormat` | `String to(CaseFormat format,String str)` | 【原文待译】Converts the specified String str from this format to the specified format. A "best effort" approach is taken; if str does not conform to the assumed format, then the behavior of this method is undefined but we make a reasonable effort at converting anyway. |
| `com.google.common.base.CharMatcher` | `CharMatcher and(CharMatcher other)` | 【原文待译】Returns a matcher that matches any character matched by both this matcher and other. |
| `com.google.common.base.CharMatcher` | `CharMatcher any()` | 【原文待译】Matches any character. |
| `com.google.common.base.CharMatcher` | `CharMatcher anyOf(CharSequence sequence)` | 【原文待译】Returns a char matcher that matches any BMP character present in the given character sequence. Returns a bogus matcher if the sequence contains supplementary characters. |
| `com.google.common.base.CharMatcher` | `CharMatcher ascii()` | 【原文待译】Determines whether a character is ASCII, meaning that its code point is less than 128. |
| `com.google.common.base.CharMatcher` | `CharMatcher breakingWhitespace()` | 【原文待译】Determines whether a character is a breaking whitespace (that is, a whitespace which can be interpreted as a break between words for formatting purposes). See #whitespace() for a discussion of that term. |
| `com.google.common.base.CharMatcher` | `CharMatcher digit()` | 【原文待译】Determines whether a character is a BMP digit according to Unicode . If you only care to match ASCII digits, you can use inRange('0', '9'). |
| `com.google.common.base.CharMatcher` | `CharMatcher forPredicate(Predicate<? super Character> predicate)` | 【原文待译】Returns a matcher with identical behavior to the given Character-based predicate, but which operates on primitive char instances instead. |
| `com.google.common.base.CharMatcher` | `CharMatcher inRange(char startInclusive,char endInclusive)` | 【原文待译】Returns a char matcher that matches any character in a given BMP range (both endpoints are inclusive). For example, to match any lowercase letter of the English alphabet, use CharMatcher.inRange('a', 'z'). |
| `com.google.common.base.CharMatcher` | `CharMatcher invisible()` | 【原文待译】Determines whether a character is invisible; that is, if its Unicode category is any of SPACE_SEPARATOR, LINE_SEPARATOR, PARAGRAPH_SEPARATOR, CONTROL, FORMAT, SURROGATE, and PRIVATE_USE according to ICU4J. See also the Unicode Default_Ignorable_Code_Point property (available via ICU). |
| `com.google.common.base.CharMatcher` | `CharMatcher is(char match)` | 【原文待译】Returns a char matcher that matches only one specified BMP character. |
| `com.google.common.base.CharMatcher` | `CharMatcher isNot(char match)` | 【原文待译】Returns a char matcher that matches any character except the BMP character specified. To negate another CharMatcher, use #negate(). |
| `com.google.common.base.CharMatcher` | `CharMatcher javaDigit()` | 【原文待译】Determines whether a character is a BMP digit according to {@linkplain Character#isDigit(char) Java's definition}. If you only care to match ASCII digits, you can use inRange('0', '9'). |
| `com.google.common.base.CharMatcher` | `CharMatcher javaIsoControl()` | 【原文待译】Determines whether a character is an ISO control character as specified by Character#isISOControl(char). All ISO control codes are on the BMP and thus supported by this API. |
| `com.google.common.base.CharMatcher` | `CharMatcher javaLetter()` | 【原文待译】Determines whether a character is a BMP letter according to {@linkplain Character#isLetter(char) Java's definition}. If you only care to match letters of the Latin alphabet, you can use inRange('a', 'z').or(inRange('A', 'Z')). |
| `com.google.common.base.CharMatcher` | `CharMatcher javaLetterOrDigit()` | 【原文待译】Determines whether a character is a BMP letter or digit according to {@linkplain Character#isLetterOrDigit(char) Java's definition}. |
| `com.google.common.base.CharMatcher` | `CharMatcher javaLowerCase()` | 【原文待译】Determines whether a BMP character is lower case according to {@linkplain Character#isLowerCase(char) Java's definition}. |
| `com.google.common.base.CharMatcher` | `CharMatcher javaUpperCase()` | 【原文待译】Determines whether a BMP character is upper case according to {@linkplain Character#isUpperCase(char) Java's definition}. |
| `com.google.common.base.CharMatcher` | `CharMatcher negate()` | 【原文待译】Returns a matcher that matches any character not matched by this matcher. |
| `com.google.common.base.CharMatcher` | `CharMatcher none()` | 【原文待译】Matches no characters. |
| `com.google.common.base.CharMatcher` | `CharMatcher noneOf(CharSequence sequence)` | 【原文待译】Returns a char matcher that matches any BMP character not present in the given character sequence. Returns a bogus matcher if the sequence contains supplementary characters. |
| `com.google.common.base.CharMatcher` | `CharMatcher or(CharMatcher other)` | 【原文待译】Returns a matcher that matches any character matched by either this matcher or other. |
| `com.google.common.base.CharMatcher` | `CharMatcher precomputed()` | 【原文待译】Returns a char matcher functionally equivalent to this one, but which may be faster to query than the original; your mileage may vary. Precomputation takes time and requires more memory, so it is only likely to be worthwhile if the precomputed matcher is queried very often. This method has no effect… |
| `com.google.common.base.CharMatcher` | `CharMatcher singleWidth()` | 【原文待译】Determines whether a character is single-width (not double-width). When in doubt, this matcher errs on the side of returning false (that is, it tends to assume a character is double-width). Note: as the reference file evolves, we will modify this matcher to keep it up to date. See also UAX #11 East … |
| `com.google.common.base.CharMatcher` | `CharMatcher whitespace()` | 【原文待译】Determines whether a character is whitespace according to the latest Unicode standard, as illustrated here . This is not the same definition used by other Java APIs. (See a comparison of several definitions of "whitespace" .) All Unicode White_Space characters are on the BMP and thus supported by th… |
| `com.google.common.base.CharMatcher` | `String collapseFrom(CharSequence sequence,char replacement)` | 【原文待译】Returns a string copy of the input character sequence, with each group of consecutive matching BMP characters replaced by a single replacement character. For example: {@snippet : CharMatcher.anyOf("eko").collapseFrom("bookkeeper", '-') } ... returns "b-p-r". The default implementation uses #indexIn(… |
| `com.google.common.base.CharMatcher` | `String removeFrom(CharSequence sequence)` | 【原文待译】Returns a string containing all non-matching characters of a character sequence, in order. For example: {@snippet : CharMatcher.is('a').removeFrom("bazaar") } ... returns "bzr". |
| `com.google.common.base.CharMatcher` | `String replaceFrom(CharSequence sequence,CharSequence replacement)` | 【原文待译】Returns a string copy of the input character sequence, with each matching BMP character replaced by a given replacement sequence. For example: {@snippet : CharMatcher.is('a').replaceFrom("yaha", "oo") } ... returns "yoohoo". Note: If the replacement is a fixed string with only one character, you are… |
| `com.google.common.base.CharMatcher` | `String replaceFrom(CharSequence sequence,char replacement)` | 【原文待译】Returns a string copy of the input character sequence, with each matching BMP character replaced by a given replacement character. For example: {@snippet : CharMatcher.is('a').replaceFrom("radar", 'o') } ... returns "rodor". The default implementation uses #indexIn(CharSequence) to find the first ma… |
| `com.google.common.base.CharMatcher` | `String retainFrom(CharSequence sequence)` | 【原文待译】Returns a string containing all matching BMP characters of a character sequence, in order. For example: {@snippet : CharMatcher.is('a').retainFrom("bazaar") } ... returns "aaa". |
| `com.google.common.base.CharMatcher` | `String toString()` | 【原文待译】Returns a string representation of this CharMatcher, such as CharMatcher.or(WHITESPACE, JAVA_DIGIT). |
| `com.google.common.base.CharMatcher` | `String trimAndCollapseFrom(CharSequence sequence,char replacement)` | 【原文待译】Collapses groups of matching characters exactly as #collapseFrom does, except that groups of matching BMP characters at the start or end of the sequence are removed without replacement. |
| `com.google.common.base.CharMatcher` | `String trimFrom(CharSequence sequence)` | 【原文待译】Returns a substring of the input character sequence that omits all matching BMP characters from the beginning and from the end of the string. For example: {@snippet : CharMatcher.anyOf("ab").trimFrom("abacatbab") } ... returns "cat". Note that: {@snippet : CharMatcher.inRange('\0', ' ').trimFrom(str… |
| `com.google.common.base.CharMatcher` | `String trimLeadingFrom(CharSequence sequence)` | 【原文待译】Returns a substring of the input character sequence that omits all matching BMP characters from the beginning of the string. For example: {@snippet : CharMatcher.anyOf("ab").trimLeadingFrom("abacatbab") } ... returns "catbab". |
| `com.google.common.base.CharMatcher` | `String trimTrailingFrom(CharSequence sequence)` | 【原文待译】Returns a substring of the input character sequence that omits all matching BMP characters from the end of the string. For example: {@snippet : CharMatcher.anyOf("ab").trimTrailingFrom("abacatbab") } ... returns "abacat". |
| `com.google.common.base.CharMatcher` | `boolean apply(Character character)` | 【原文待译】@deprecated Provided only to satisfy the Predicate interface; use #matches instead. |
| `com.google.common.base.CharMatcher` | `boolean matches(char c)` | 【原文待译】Determines a true or false value for the given character. |
| `com.google.common.base.CharMatcher` | `boolean matchesAllOf(CharSequence sequence)` | 【原文待译】Returns true if a character sequence contains only matching BMP characters. The default implementation iterates over the sequence, invoking #matches for each character, until this returns false or the end is reached. |
| `com.google.common.base.CharMatcher` | `boolean matchesAnyOf(CharSequence sequence)` | 【原文待译】Returns true if a character sequence contains at least one matching BMP character. Equivalent to !matchesNoneOf(sequence). The default implementation iterates over the sequence, invoking #matches for each character, until this returns true or the end is reached. |
| `com.google.common.base.CharMatcher` | `boolean matchesNoneOf(CharSequence sequence)` | 【原文待译】Returns true if a character sequence contains no matching BMP characters. Equivalent to !matchesAnyOf(sequence). The default implementation iterates over the sequence, invoking #matches for each character, until this returns true or the end is reached. |
| `com.google.common.base.CharMatcher` | `boolean test(Character character)` | 【原文待译】@deprecated Provided only to satisfy the java.util.function.Predicate interface; use #matches instead. |
| `com.google.common.base.CharMatcher` | `int countIn(CharSequence sequence)` | 【原文待译】Returns the number of matching chars found in a character sequence. Counts 2 per supplementary character, such as for #whitespace().#negate(). |
| `com.google.common.base.CharMatcher` | `int indexIn(CharSequence sequence)` | 【原文待译】Returns the index of the first matching BMP character in a character sequence, or -1 if no matching character is present. The default implementation iterates over the sequence in forward order calling #matches for each character. |
| `com.google.common.base.CharMatcher` | `int indexIn(CharSequence sequence,int start)` | 【原文待译】Returns the index of the first matching BMP character in a character sequence, starting from a given position, or -1 if no character matches after that position. The default implementation iterates over the sequence in forward order, beginning at start, calling #matches for each character. |
| `com.google.common.base.CharMatcher` | `int lastIndexIn(CharSequence sequence)` | 【原文待译】Returns the index of the last matching BMP character in a character sequence, or -1 if no matching character is present. The default implementation iterates over the sequence in reverse order calling #matches for each character. |
| `com.google.common.base.Converter` | `B apply(A a)` | 【原文待译】@deprecated Provided to satisfy the Function interface; use #convert instead. |
| `com.google.common.base.Converter` | `B convert(@Nullable
A a)` | 【原文待译】Returns a representation of a as an instance of type B. |
| `com.google.common.base.Converter` | `Converter<A, B> from(Function<? super A, ? extends B> forwardFunction,Function<? super B, ? extends A> backwardFunction)` | 【原文待译】Returns a converter based on separate forward and backward functions. This is useful if the function instances already exist, or so that you can supply lambda expressions. If those circumstances don't apply, you probably don't need to use this; subclass Converter and implement its #doForward and #do… |
| `com.google.common.base.Converter` | `Converter<A, C> andThen(Converter<B, C> secondConverter)` | 【原文待译】Returns a converter whose convert method applies secondConverter to the result of this converter. Its reverse method applies the converters in reverse order. The returned converter is serializable if this converter and secondConverter are. |
| `com.google.common.base.Converter` | `Converter<B, A> reverse()` | 【原文待译】Returns the reversed view of this converter, which converts this.convert(a) back to a value roughly equivalent to a. The returned converter is serializable if this converter is. Note: you should not override this method. It is non-final for legacy reasons. |
| `com.google.common.base.Converter` | `Converter<T, T> identity()` | 【原文待译】Returns a serializable converter that always converts or reverses an object to itself. |
| `com.google.common.base.Converter` | `Iterable<B> convertAll(Iterable<? extends A> fromIterable)` | 【原文待译】Returns an iterable that applies convert to each element of fromIterable. The conversion is done lazily. The returned iterable's iterator supports remove() if the input iterator does. After a successful remove() call, fromIterable no longer contains the corresponding element. |
| `com.google.common.base.Converter` | `boolean equals(@Nullable
Object object)` | 【原文待译】Indicates whether another object is equal to this converter. Most implementations will have no reason to override the behavior of Object#equals. However, an implementation may also choose to return true whenever object is a Converter that it considers interchangeable with this one. "Interchangeable"… |
| `com.google.common.base.Defaults` | `T defaultValue(Class<T> type)` | 【原文待译】Returns the default value of type as defined by JLS --- 0 for numbers, false for boolean and '\0' for char. For non-primitive types and void, null is returned. |
| `com.google.common.base.Enums` | `Converter<String, T> stringConverter(Class<T> enumClass)` | 【原文待译】Returns a serializable converter that converts between strings and enum values of type enumClass using Enum#valueOf(Class, String) and Enum#name(). The converter will throw an IllegalArgumentException if the argument is not the name of any enum constant in the specified enum. |
| `com.google.common.base.Enums` | `Field getField(Enum<?> enumValue)` | 【原文待译】Returns the Field in which enumValue is defined. For example, to get the Description annotation on the GOLF constant of enum Sport, use Enums.getField(Sport.GOLF).getAnnotation(Description.class). |
| `com.google.common.base.Enums` | `Optional<T> getIfPresent(Class<T> enumClass,String value)` | 【原文待译】Returns an optional enum constant for the given type, using Enum#valueOf. If the constant does not exist, Optional#absent is returned. A common use case is for parsing user input or falling back to a default enum constant. For example, Enums.getIfPresent(Country.class, countryInput).or(Country.DEFAU… |
| `com.google.common.base.Equivalence` | `Equivalence<F> onResultOf(Function<? super F, ? extends @Nullable T> function)` | 【原文待译】Returns a new equivalence relation for F which evaluates equivalence by first applying function to the argument, then evaluating using this. That is, for any pair of non-null objects x and y, equivalence.onResultOf(function).equivalent(a, b) is true if and only if equivalence.equivalent(function.app… |
| `com.google.common.base.Equivalence` | `Equivalence<Iterable<S>> pairwise()` | 【原文待译】Returns an equivalence over iterables based on the equivalence of their elements. More specifically, two iterables are considered equivalent if they both contain the same number of elements, and each pair of corresponding elements is equivalent according to this. Null iterables are equivalent to one… |
| `com.google.common.base.Equivalence` | `Equivalence<Object> equals()` | 【原文待译】Returns an equivalence that delegates to Object#equals and Object#hashCode. Equivalence#equivalent returns true if both values are null, or if neither value is null and Object#equals returns true. Equivalence#hash returns 0 if passed a null value. |
| `com.google.common.base.Equivalence` | `Equivalence<Object> identity()` | 【原文待译】Returns an equivalence that uses == to compare values and System#identityHashCode(Object) to compute the hash code. Equivalence#equivalent returns true if a == b, including in the case that a and b are both null. |
| `com.google.common.base.Equivalence` | `Predicate<@Nullable T> equivalentTo(@Nullable
T target)` | 【原文待译】Returns a predicate that evaluates to true if and only if the input is equivalent to target according to this equivalence relation. |
| `com.google.common.base.Equivalence` | `Wrapper<S> wrap(@ParametricNullness
S reference)` | 【原文待译】Returns a wrapper of reference that implements Wrapper#equals(Object) Object.equals() such that wrap(a).equals(wrap(b)) if and only if equivalent(a, b). The returned object is serializable if both this Equivalence and reference are serializable (including when reference is null). |
| `com.google.common.base.Equivalence` | `boolean equivalent(@Nullable
T a,@Nullable
T b)` | 【原文待译】Returns true if the given objects are considered equivalent. This method describes an equivalence relation on object references, meaning that for all references x, y, and z (any of which may be null): equivalent(x, x) is true ( reflexive property) equivalent(x, y) and equivalent(y, x) each return th… |
| `com.google.common.base.Equivalence` | `boolean test(@Nullable
T t,@Nullable
T u)` | 【原文待译】@deprecated Provided only to satisfy the BiPredicate interface; use #equivalent instead. |
| `com.google.common.base.Equivalence` | `int hash(@Nullable
T t)` | 【原文待译】Returns a hash code for t. The hash has the following properties: It is consistent : for any reference x, multiple invocations of hash(x} consistently return the same value provided x remains unchanged according to the definition of the equivalence. The hash need not remain consistent from one execu… |
| `com.google.common.base.Equivalence$Wrapper` | `String toString()` | 【原文待译】Returns a string representation for this equivalence wrapper. The form of this string representation is not specified. |
| `com.google.common.base.Equivalence$Wrapper` | `T get()` | 【原文待译】Returns the (possibly null) reference wrapped by this instance. |
| `com.google.common.base.Equivalence$Wrapper` | `boolean equals(@Nullable
Object obj)` | 【原文待译】Returns true if Equivalence#equivalent(Object, Object) applied to the wrapped references is true and both wrappers use the Object#equals(Object) same equivalence. |
| `com.google.common.base.Equivalence$Wrapper` | `int hashCode()` | 【原文待译】Returns the result of Equivalence#hash(Object) applied to the wrapped reference. |
| `com.google.common.base.FinalizableReference` | `void finalizeReferent()` | 【原文待译】Invoked on a background thread after the referent has been garbage collected unless security restrictions prevented starting a background thread, in which case this method is invoked when new references are created. |
| `com.google.common.base.FinalizableReferenceQueue` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.base.Function` | `T apply(@ParametricNullness
F input)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.base.Function` | `boolean equals(@Nullable
Object object)` | 【原文待译】May return true if object is a Function that behaves identically to this function. Warning: do not depend on the behavior of this method. Historically, Function instances in this library have implemented this method to recognize certain cases where distinct Function instances would in fact behave id… |
| `com.google.common.base.Functions` | `Function<@Nullable Object, E> constant(@ParametricNullness
E value)` | 【原文待译】Returns a function that ignores its input and always returns value. Java 8+ users: use the lambda expression o -> value instead. |
| `com.google.common.base.Functions` | `Function<A, C> compose(Function<B, C> g,Function<A, ? extends B> f)` | 【原文待译】Returns the composition of two functions. For f: A->B and g: B->C, composition is defined as the function h such that h(a) == g(f(a)) for each a. Java 8+ users: use g.compose(f) or (probably clearer) f.andThen(g) instead. |
| `com.google.common.base.Functions` | `Function<E, E> identity()` | 【原文待译】Returns the identity function. Discouraged: Prefer using a lambda like v -> v, which is shorter and often more readable. |
| `com.google.common.base.Functions` | `Function<F, T> forSupplier(Supplier<T> supplier)` | 【原文待译】Returns a function that ignores its input and returns the result of supplier.get(). Java 8+ users: use the lambda expression o -> supplier.get() instead. |
| `com.google.common.base.Functions` | `Function<K, V> forMap(Map<K, ? extends V> map,@ParametricNullness
V defaultValue)` | 【原文待译】Returns a function which performs a map lookup with a default value. The function created by this method returns defaultValue for all inputs that do not belong to the map's key set. See also #forMap(Map), which throws an exception in this case. Java 8+ users: you can just write the lambda expression… |
| `com.google.common.base.Functions` | `Function<K, V> forMap(Map<K, V> map)` | 【原文待译】Returns a function which performs a map lookup. The returned function throws an IllegalArgumentException if given a key that does not exist in the map. See also #forMap(Map, Object), which returns a default value in this case. Note: if map is a com.google.common.collect.BiMap BiMap (or can be one), … |
| `com.google.common.base.Functions` | `Function<Object, String> toStringFunction()` | 【原文待译】A function equivalent to the method reference Object::toString, for users not yet using Java 8. The function simply invokes toString on its argument and returns the result. It throws a NullPointerException on null input. Warning: The returned function may not be consistent with equals (as documented… |
| `com.google.common.base.Functions` | `Function<T, Boolean> forPredicate(Predicate<T> predicate)` | 【原文待译】Creates a function that returns the same boolean output as the given predicate for all inputs. The returned function is consistent with equals (as documented at Function#apply) if and only if predicate is itself consistent with equals. Java 8+ users: use the method reference predicate::test instead. |
| `com.google.common.base.Joiner` | `A appendTo(A appendable,@Nullable
Object first,@Nullable
Object second,@Nullable
Object... rest)` | 【原文待译】Appends to appendable the string representation of each of the remaining arguments. |
| `com.google.common.base.Joiner` | `A appendTo(A appendable,@Nullable
Object[] parts)` | 【原文待译】Appends the string representation of each of parts, using the previously configured separator between each, to appendable. |
| `com.google.common.base.Joiner` | `A appendTo(A appendable,Iterable<?> parts)` | 【原文待译】Appends the string representation of each of parts, using the previously configured separator between each, to appendable. |
| `com.google.common.base.Joiner` | `A appendTo(A appendable,Iterator<?> parts)` | 【原文待译】Appends the string representation of each of parts, using the previously configured separator between each, to appendable. |
| `com.google.common.base.Joiner` | `Joiner on(String separator)` | 【原文待译】Returns a joiner which automatically places separator between consecutive elements. |
| `com.google.common.base.Joiner` | `Joiner on(char separator)` | 【原文待译】Returns a joiner which automatically places separator between consecutive elements. |
| `com.google.common.base.Joiner` | `Joiner skipNulls()` | 【原文待译】Returns a joiner with the same behavior as this joiner, except automatically skipping over any provided null elements. |
| `com.google.common.base.Joiner` | `Joiner useForNull(String nullText)` | 【原文待译】Returns a joiner with the same behavior as this one, except automatically substituting nullText for any provided null elements. |
| `com.google.common.base.Joiner` | `MapJoiner withKeyValueSeparator(String keyValueSeparator)` | 【原文待译】Returns a MapJoiner using the given key-value separator, and the same configuration as this Joiner otherwise. |
| `com.google.common.base.Joiner` | `MapJoiner withKeyValueSeparator(char keyValueSeparator)` | 【原文待译】Returns a MapJoiner using the given key-value separator, and the same configuration as this Joiner otherwise. |
| `com.google.common.base.Joiner` | `String join(@Nullable
Object first,@Nullable
Object second,@Nullable
Object... rest)` | 【原文待译】Returns a string containing the string representation of each argument, using the previously configured separator between each. |
| `com.google.common.base.Joiner` | `String join(@Nullable
Object[] parts)` | 【原文待译】Returns a string containing the string representation of each of parts, using the previously configured separator between each. |
| `com.google.common.base.Joiner` | `String join(Iterable<?> parts)` | 【原文待译】Returns a string containing the string representation of each of parts, using the previously configured separator between each. |
| `com.google.common.base.Joiner` | `String join(Iterator<?> parts)` | 【原文待译】Returns a string containing the string representation of each of parts, using the previously configured separator between each. |
| `com.google.common.base.Joiner` | `StringBuilder appendTo(StringBuilder builder,@Nullable
Object first,@Nullable
Object second,@Nullable
Object... rest)` | 【原文待译】Appends to builder the string representation of each of the remaining arguments. Identical to #appendTo(Appendable, Object, Object, Object...), except that it does not throw IOException. |
| `com.google.common.base.Joiner` | `StringBuilder appendTo(StringBuilder builder,@Nullable
Object[] parts)` | 【原文待译】Appends the string representation of each of parts, using the previously configured separator between each, to builder. Identical to #appendTo(Appendable, Iterable), except that it does not throw IOException. |
| `com.google.common.base.Joiner` | `StringBuilder appendTo(StringBuilder builder,Iterable<?> parts)` | 【原文待译】Appends the string representation of each of parts, using the previously configured separator between each, to builder. Identical to #appendTo(Appendable, Iterable), except that it does not throw IOException. |
| `com.google.common.base.Joiner` | `StringBuilder appendTo(StringBuilder builder,Iterator<?> parts)` | 【原文待译】Appends the string representation of each of parts, using the previously configured separator between each, to builder. Identical to #appendTo(Appendable, Iterable), except that it does not throw IOException. |
| `com.google.common.base.Joiner$MapJoiner` | `A appendTo(A appendable,Iterable<? extends Entry<?, ?>> entries)` | 【原文待译】Appends the string representation of each entry in entries, using the previously configured separator and key-value separator, to appendable. |
| `com.google.common.base.Joiner$MapJoiner` | `A appendTo(A appendable,Iterator<? extends Entry<?, ?>> parts)` | 【原文待译】Appends the string representation of each entry in entries, using the previously configured separator and key-value separator, to appendable. |
| `com.google.common.base.Joiner$MapJoiner` | `A appendTo(A appendable,Map<?, ?> map)` | 【原文待译】Appends the string representation of each entry of map, using the previously configured separator and key-value separator, to appendable. |
| `com.google.common.base.Joiner$MapJoiner` | `MapJoiner useForNull(String nullText)` | 【原文待译】Returns a map joiner with the same behavior as this one, except automatically substituting nullText for any provided null keys or values. |
| `com.google.common.base.Joiner$MapJoiner` | `String join(Iterable<? extends Entry<?, ?>> entries)` | 【原文待译】Returns a string containing the string representation of each entry in entries, using the previously configured separator and key-value separator. |
| `com.google.common.base.Joiner$MapJoiner` | `String join(Iterator<? extends Entry<?, ?>> entries)` | 【原文待译】Returns a string containing the string representation of each entry in entries, using the previously configured separator and key-value separator. |
| `com.google.common.base.Joiner$MapJoiner` | `String join(Map<?, ?> map)` | 【原文待译】Returns a string containing the string representation of each entry of map, using the previously configured separator and key-value separator. |
| `com.google.common.base.Joiner$MapJoiner` | `StringBuilder appendTo(StringBuilder builder,Iterable<? extends Entry<?, ?>> entries)` | 【原文待译】Appends the string representation of each entry in entries, using the previously configured separator and key-value separator, to builder. Identical to #appendTo(Appendable, Iterable), except that it does not throw IOException. |
| `com.google.common.base.Joiner$MapJoiner` | `StringBuilder appendTo(StringBuilder builder,Iterator<? extends Entry<?, ?>> entries)` | 【原文待译】Appends the string representation of each entry in entries, using the previously configured separator and key-value separator, to builder. Identical to #appendTo(Appendable, Iterable), except that it does not throw IOException. |
| `com.google.common.base.Joiner$MapJoiner` | `StringBuilder appendTo(StringBuilder builder,Map<?, ?> map)` | 【原文待译】Appends the string representation of each entry of map, using the previously configured separator and key-value separator, to builder. Identical to #appendTo(Appendable, Map), except that it does not throw IOException. |
| `com.google.common.base.MoreObjects` | `T firstNonNull(@Nullable
T first,@Nullable
T second)` | 【原文待译】Returns the first of two given parameters that is not null, if either is, or otherwise throws a NullPointerException. To find the first non-null element in an iterable, use Iterables.find(iterable, Predicates.notNull()). For varargs, use Iterables.find(Arrays.asList(a, b, c, ...), Predicates.notNull… |
| `com.google.common.base.MoreObjects` | `ToStringHelper toStringHelper(Class<?> clazz)` | 【原文待译】Creates an instance of ToStringHelper in the same manner as #toStringHelper(Object), but using the simple name of clazz instead of using an instance's Object#getClass(). Note that in GWT, class names are often obfuscated. |
| `com.google.common.base.MoreObjects` | `ToStringHelper toStringHelper(Object self)` | 【原文待译】Creates an instance of ToStringHelper. This is helpful for implementing Object#toString(). Specification by example: {@snippet : // Returns "ClassName{}" MoreObjects.toStringHelper(this) .toString(); // Returns "ClassName{x=1}" MoreObjects.toStringHelper(this) .add("x", 1) .toString(); // Returns "M… |
| `com.google.common.base.MoreObjects` | `ToStringHelper toStringHelper(String className)` | 【原文待译】Creates an instance of ToStringHelper in the same manner as #toStringHelper(Object), but using className instead of using an instance's Object#getClass(). |
| `com.google.common.base.MoreObjects$ToStringHelper` | `String toString()` | 【原文待译】Returns a string in the format specified by MoreObjects#toStringHelper(Object). After calling this method, you can keep adding more properties to later call toString() again and get a more complete representation of the same object; but properties cannot be removed, so this only allows limited reuse… |
| `com.google.common.base.MoreObjects$ToStringHelper` | `ToStringHelper add(String name,@Nullable
Object value)` | 【原文待译】Adds a name/value pair to the formatted output in name=value format. If value is null, the string "null" is used, unless #omitNullValues() is called, in which case this name/value pair will not be added. |
| `com.google.common.base.MoreObjects$ToStringHelper` | `ToStringHelper add(String name,boolean value)` | 【原文待译】Adds a name/value pair to the formatted output in name=value format. |
| `com.google.common.base.MoreObjects$ToStringHelper` | `ToStringHelper add(String name,char value)` | 【原文待译】Adds a name/value pair to the formatted output in name=value format. |
| `com.google.common.base.MoreObjects$ToStringHelper` | `ToStringHelper add(String name,double value)` | 【原文待译】Adds a name/value pair to the formatted output in name=value format. |
| `com.google.common.base.MoreObjects$ToStringHelper` | `ToStringHelper add(String name,float value)` | 【原文待译】Adds a name/value pair to the formatted output in name=value format. |
| `com.google.common.base.MoreObjects$ToStringHelper` | `ToStringHelper add(String name,int value)` | 【原文待译】Adds a name/value pair to the formatted output in name=value format. |
| `com.google.common.base.MoreObjects$ToStringHelper` | `ToStringHelper add(String name,long value)` | 【原文待译】Adds a name/value pair to the formatted output in name=value format. |
| `com.google.common.base.MoreObjects$ToStringHelper` | `ToStringHelper addValue(@Nullable
Object value)` | 【原文待译】Adds an unnamed value to the formatted output. It is strongly encouraged to use #add(String, Object) instead and give value a readable name. |
| `com.google.common.base.MoreObjects$ToStringHelper` | `ToStringHelper addValue(boolean value)` | 【原文待译】Adds an unnamed value to the formatted output. It is strongly encouraged to use #add(String, boolean) instead and give value a readable name. |
| `com.google.common.base.MoreObjects$ToStringHelper` | `ToStringHelper addValue(char value)` | 【原文待译】Adds an unnamed value to the formatted output. It is strongly encouraged to use #add(String, char) instead and give value a readable name. |
| `com.google.common.base.MoreObjects$ToStringHelper` | `ToStringHelper addValue(double value)` | 【原文待译】Adds an unnamed value to the formatted output. It is strongly encouraged to use #add(String, double) instead and give value a readable name. |
| `com.google.common.base.MoreObjects$ToStringHelper` | `ToStringHelper addValue(float value)` | 【原文待译】Adds an unnamed value to the formatted output. It is strongly encouraged to use #add(String, float) instead and give value a readable name. |
| `com.google.common.base.MoreObjects$ToStringHelper` | `ToStringHelper addValue(int value)` | 【原文待译】Adds an unnamed value to the formatted output. It is strongly encouraged to use #add(String, int) instead and give value a readable name. |
| `com.google.common.base.MoreObjects$ToStringHelper` | `ToStringHelper addValue(long value)` | 【原文待译】Adds an unnamed value to the formatted output. It is strongly encouraged to use #add(String, long) instead and give value a readable name. |
| `com.google.common.base.MoreObjects$ToStringHelper` | `ToStringHelper omitEmptyValues()` | 【原文待译】Configures the ToStringHelper so #toString() will ignore properties with empty values. The order of calling this method, relative to the add()/addValue() methods, is not significant. Note: in general, code should assume that the string form returned by ToStringHelper for a given object may change. I… |
| `com.google.common.base.MoreObjects$ToStringHelper` | `ToStringHelper omitNullValues()` | 【原文待译】Configures the ToStringHelper so #toString() will ignore properties with null value. The order of calling this method, relative to the add()/addValue() methods, is not significant. |
| `com.google.common.base.Objects` | `boolean equal(@Nullable
Object a,@Nullable
Object b)` | 【原文待译】Determines whether two possibly-null objects are equal. Returns: true if a and b are both null. true if a and b are both non-null and they are equal according to Object#equals(Object). false in all other situations. This assumes that any non-null objects passed to this function conform to the equals… |
| `com.google.common.base.Objects` | `int hashCode(@Nullable
Object @Nullable ... objects)` | 【原文待译】Generates a hash code for multiple values. The hash code is generated by calling Arrays#hashCode(Object[]). Note that array arguments to this method, with the exception of a single Object array, do not get any special handling; their hash codes are based on identity and not contents. This is useful … |
| `com.google.common.base.Optional` | `Iterable<T> presentInstances(Iterable<? extends Optional<? extends T>> optionals)` | 【原文待译】Returns the value of each present instance from the supplied optionals, in order, skipping over occurrences of Optional#absent. Iterators are unmodifiable and are evaluated lazily. Comparison to java.util.Optional: this method has no equivalent in Java 8's Optional class; use optionals.stream().filt… |
| `com.google.common.base.Optional` | `Optional<T> absent()` | 【原文待译】Returns an Optional instance with no contained reference. Comparison to java.util.Optional: this method is equivalent to Java 8's Optional.empty. |
| `com.google.common.base.Optional` | `Optional<T> fromJavaUtil(java.util.@Nullable Optional<T> javaUtilOptional)` | 【原文待译】Returns the equivalent com.google.common.base.Optional value to the given java.util.Optional, or null if the argument is null. |
| `com.google.common.base.Optional` | `Optional<T> fromNullable(@Nullable
T nullableReference)` | 【原文待译】If nullableReference is non-null, returns an Optional instance containing that reference; otherwise returns Optional#absent. Comparison to java.util.Optional: this method is equivalent to Java 8's Optional.ofNullable. |
| `com.google.common.base.Optional` | `Optional<T> of(T reference)` | 【原文待译】Returns an Optional instance containing the given non-null reference. To have null treated as #absent, use #fromNullable instead. Comparison to java.util.Optional: no differences. |
| `com.google.common.base.Optional` | `Optional<T> or(Optional<? extends T> secondChoice)` | 【原文待译】Returns this Optional if it has a value present; secondChoice otherwise. Comparison to java.util.Optional: this method has no equivalent in Java 8's Optional class; write thisOptional.isPresent() ? thisOptional : secondChoice instead. |
| `com.google.common.base.Optional` | `Optional<V> transform(Function<? super T, V> function)` | 【原文待译】If the instance is present, it is transformed with the given Function; otherwise, Optional#absent is returned. Comparison to java.util.Optional: this method is similar to Java 8's Optional.map, except when function returns null. In this case this method throws an exception, whereas the Java 8+ metho… |
| `com.google.common.base.Optional` | `Set<T> asSet()` | 【原文待译】Returns an immutable singleton Set whose only element is the contained instance if it is present; an empty immutable Set otherwise. Comparison to java.util.Optional: this method has no equivalent in Java 8's Optional class. However, this common usage: {@snippet : for (Foo foo : possibleFoo.asSet()) … |
| `com.google.common.base.Optional` | `String toString()` | 【原文待译】Returns a string representation for this instance. Comparison to java.util.Optional: this class leaves the specific string representation unspecified, unlike the Java 8+ equivalent. |
| `com.google.common.base.Optional` | `T get()` | 【原文待译】Returns the contained instance, which must be present. If the instance might be absent, use #or(Object) or #orNull instead. Comparison to java.util.Optional: when the value is absent, this method throws IllegalStateException, whereas the java.util counterpart throws java.util.NoSuchElementException … |
| `com.google.common.base.Optional` | `T or(Supplier<? extends T> supplier)` | 【原文待译】Returns the contained instance if it is present; supplier.get() otherwise. Comparison to java.util.Optional: this method is similar to Java 8's Optional.orElseGet, except when supplier returns null. In this case this method throws an exception, whereas the Java 8+ method returns the null to the call… |
| `com.google.common.base.Optional` | `T or(T defaultValue)` | 【原文待译】Returns the contained instance if it is present; defaultValue otherwise. If no default value should be required because the instance is known to be present, use #get() instead. For a default value of null, use #orNull. Note about generics: The signature public T or(T defaultValue) is overly restrict… |
| `com.google.common.base.Optional` | `T orNull()` | 【原文待译】Returns the contained instance if it is present; null otherwise. If the instance is known to be present, use #get() instead. Comparison to java.util.Optional: this method is equivalent to Java 8's Optional.orElse(null). |
| `com.google.common.base.Optional` | `boolean equals(@Nullable
Object object)` | 【原文待译】Returns true if object is an Optional instance, and either the contained references are {@linkplain Object#equals equal} to each other or both are absent. Note that Optional instances of differing parameterized types can be equal. Comparison to java.util.Optional: no differences. |
| `com.google.common.base.Optional` | `boolean isPresent()` | 【原文待译】Returns true if this holder contains a (non-null) instance. Comparison to java.util.Optional: no differences. |
| `com.google.common.base.Optional` | `int hashCode()` | 【原文待译】Returns a hash code for this instance. Comparison to java.util.Optional: this class leaves the specific choice of hash code unspecified, unlike the Java 8+ equivalent. |
| `com.google.common.base.Optional` | `java.util.@Nullable Optional<T> toJavaUtil(@Nullable
Optional<T> googleOptional)` | 【原文待译】Returns the equivalent java.util.Optional value to the given com.google.common.base.Optional, or null if the argument is null. If googleOptional is known to be non-null, use googleOptional.toJavaUtil() instead. Unfortunately, the method reference Optional::toJavaUtil will not work, because it could … |
| `com.google.common.base.Optional` | `java.util.Optional<T> toJavaUtil()` | 【原文待译】Returns the equivalent java.util.Optional value to this optional. Unfortunately, the method reference Optional::toJavaUtil will not work, because it could refer to either the static or instance version of this method. Write out the lambda expression o -> o.toJavaUtil() instead. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference,@Nullable
Object errorMessage)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference,String errorMessageTemplate,@Nullable
Object @Nullable ... errorMessageArgs)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference,String errorMessageTemplate,@Nullable
Object p1)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. See #checkNotNull(Object, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference,String errorMessageTemplate,@Nullable
Object p1,@Nullable
Object p2)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. See #checkNotNull(Object, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference,String errorMessageTemplate,@Nullable
Object p1,@Nullable
Object p2,@Nullable
Object p3)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. See #checkNotNull(Object, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference,String errorMessageTemplate,@Nullable
Object p1,@Nullable
Object p2,@Nullable
Object p3,@Nullable
Object p4)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. See #checkNotNull(Object, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference,String errorMessageTemplate,@Nullable
Object p1,char p2)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. See #checkNotNull(Object, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference,String errorMessageTemplate,@Nullable
Object p1,int p2)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. See #checkNotNull(Object, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference,String errorMessageTemplate,@Nullable
Object p1,long p2)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. See #checkNotNull(Object, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference,String errorMessageTemplate,char p1)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. See #checkNotNull(Object, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference,String errorMessageTemplate,char p1,@Nullable
Object p2)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. See #checkNotNull(Object, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference,String errorMessageTemplate,char p1,char p2)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. See #checkNotNull(Object, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference,String errorMessageTemplate,char p1,int p2)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. See #checkNotNull(Object, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference,String errorMessageTemplate,char p1,long p2)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. See #checkNotNull(Object, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference,String errorMessageTemplate,int p1)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. See #checkNotNull(Object, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference,String errorMessageTemplate,int p1,@Nullable
Object p2)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. See #checkNotNull(Object, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference,String errorMessageTemplate,int p1,char p2)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. See #checkNotNull(Object, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference,String errorMessageTemplate,int p1,int p2)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. See #checkNotNull(Object, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference,String errorMessageTemplate,int p1,long p2)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. See #checkNotNull(Object, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference,String errorMessageTemplate,long p1)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. See #checkNotNull(Object, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference,String errorMessageTemplate,long p1,@Nullable
Object p2)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. See #checkNotNull(Object, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference,String errorMessageTemplate,long p1,char p2)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. See #checkNotNull(Object, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference,String errorMessageTemplate,long p1,int p2)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. See #checkNotNull(Object, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `T checkNotNull(@Nullable
T reference,String errorMessageTemplate,long p1,long p2)` | 【原文待译】Ensures that an object reference passed as a parameter to the calling method is not null. See #checkNotNull(Object, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `int checkElementIndex(int index,int size)` | 【原文待译】Ensures that index specifies a valid element in an array, list or string of size size. An element index may range from zero, inclusive, to size, exclusive. |
| `com.google.common.base.Preconditions` | `int checkElementIndex(int index,int size,String desc)` | 【原文待译】Ensures that index specifies a valid element in an array, list or string of size size. An element index may range from zero, inclusive, to size, exclusive. |
| `com.google.common.base.Preconditions` | `int checkPositionIndex(int index,int size)` | 【原文待译】Ensures that index specifies a valid position in an array, list or string of size size. A position index may range from zero to size, inclusive. |
| `com.google.common.base.Preconditions` | `int checkPositionIndex(int index,int size,String desc)` | 【原文待译】Ensures that index specifies a valid position in an array, list or string of size size. A position index may range from zero to size, inclusive. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression,@Nullable
Object errorMessage)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression,@Nullable
String errorMessageTemplate,@Nullable
Object p1,@Nullable
Object p2)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. See #checkArgument(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression,String errorMessageTemplate,@Nullable
Object @Nullable ... errorMessageArgs)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression,String errorMessageTemplate,@Nullable
Object p1)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. See #checkArgument(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression,String errorMessageTemplate,@Nullable
Object p1,@Nullable
Object p2,@Nullable
Object p3)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. See #checkArgument(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression,String errorMessageTemplate,@Nullable
Object p1,@Nullable
Object p2,@Nullable
Object p3,@Nullable
Object p4)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. See #checkArgument(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression,String errorMessageTemplate,@Nullable
Object p1,char p2)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. See #checkArgument(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression,String errorMessageTemplate,@Nullable
Object p1,int p2)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. See #checkArgument(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression,String errorMessageTemplate,@Nullable
Object p1,long p2)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. See #checkArgument(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression,String errorMessageTemplate,char p1)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. See #checkArgument(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression,String errorMessageTemplate,char p1,@Nullable
Object p2)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. See #checkArgument(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression,String errorMessageTemplate,char p1,char p2)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. See #checkArgument(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression,String errorMessageTemplate,char p1,int p2)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. See #checkArgument(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression,String errorMessageTemplate,char p1,long p2)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. See #checkArgument(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression,String errorMessageTemplate,int p1)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. See #checkArgument(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression,String errorMessageTemplate,int p1,@Nullable
Object p2)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. See #checkArgument(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression,String errorMessageTemplate,int p1,char p2)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. See #checkArgument(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression,String errorMessageTemplate,int p1,int p2)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. See #checkArgument(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression,String errorMessageTemplate,int p1,long p2)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. See #checkArgument(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression,String errorMessageTemplate,long p1)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. See #checkArgument(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression,String errorMessageTemplate,long p1,@Nullable
Object p2)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. See #checkArgument(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression,String errorMessageTemplate,long p1,char p2)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. See #checkArgument(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression,String errorMessageTemplate,long p1,int p2)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. See #checkArgument(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkArgument(boolean expression,String errorMessageTemplate,long p1,long p2)` | 【原文待译】Ensures the truth of an expression involving one or more parameters to the calling method. See #checkArgument(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkPositionIndexes(int start,int end,int size)` | 【原文待译】Ensures that start and end specify valid positions in an array, list or string of size size, and are in order. A position index may range from zero to size, inclusive. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression,@Nullable
Object errorMessage)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression,@Nullable
String errorMessageTemplate,@Nullable
Object @Nullable ... errorMessageArgs)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression,String errorMessageTemplate,@Nullable
Object p1)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. See #checkState(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression,String errorMessageTemplate,@Nullable
Object p1,@Nullable
Object p2)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. See #checkState(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression,String errorMessageTemplate,@Nullable
Object p1,@Nullable
Object p2,@Nullable
Object p3)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. See #checkState(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression,String errorMessageTemplate,@Nullable
Object p1,@Nullable
Object p2,@Nullable
Object p3,@Nullable
Object p4)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. See #checkState(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression,String errorMessageTemplate,@Nullable
Object p1,char p2)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. See #checkState(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression,String errorMessageTemplate,@Nullable
Object p1,int p2)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. See #checkState(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression,String errorMessageTemplate,@Nullable
Object p1,long p2)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. See #checkState(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression,String errorMessageTemplate,char p1)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. See #checkState(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression,String errorMessageTemplate,char p1,@Nullable
Object p2)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. See #checkState(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression,String errorMessageTemplate,char p1,char p2)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. See #checkState(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression,String errorMessageTemplate,char p1,int p2)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. See #checkState(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression,String errorMessageTemplate,char p1,long p2)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. See #checkState(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression,String errorMessageTemplate,int p1)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. See #checkState(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression,String errorMessageTemplate,int p1,@Nullable
Object p2)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. See #checkState(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression,String errorMessageTemplate,int p1,char p2)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. See #checkState(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression,String errorMessageTemplate,int p1,int p2)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. See #checkState(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression,String errorMessageTemplate,int p1,long p2)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. See #checkState(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression,String errorMessageTemplate,long p1)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. See #checkState(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression,String errorMessageTemplate,long p1,@Nullable
Object p2)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. See #checkState(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression,String errorMessageTemplate,long p1,char p2)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. See #checkState(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression,String errorMessageTemplate,long p1,int p2)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. See #checkState(boolean, String, Object...) for details. |
| `com.google.common.base.Preconditions` | `void checkState(boolean expression,String errorMessageTemplate,long p1,long p2)` | 【原文待译】Ensures the truth of an expression involving the state of the calling instance, but not involving any parameters to the calling method. See #checkState(boolean, String, Object...) for details. |
| `com.google.common.base.Predicate` | `boolean apply(@ParametricNullness
T input)` | 【原文待译】Returns the result of applying this predicate to input (Java 8+ users, see notes in the class documentation above). This method is generally expected , but not absolutely required, to have the following properties: Its execution does not cause any observable side effects. The computation is consiste… |
| `com.google.common.base.Predicate` | `boolean equals(@Nullable
Object object)` | 【原文待译】Indicates whether another object is equal to this predicate. Most implementations will have no reason to override the behavior of Object#equals. However, an implementation may also choose to return true whenever object is a Predicate that it considers interchangeable with this one. "Interchangeable"… |
| `com.google.common.base.Predicate` | `boolean test(@ParametricNullness
T input)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.base.Predicates` | `Predicate<A> compose(Predicate<B> predicate,Function<A, ? extends B> function)` | 【原文待译】Returns the composition of a function and a predicate. For every x, the generated predicate returns predicate(function(x)). |
| `com.google.common.base.Predicates` | `Predicate<CharSequence> contains(Pattern pattern)` | 【原文待译】Returns a predicate that evaluates to true if the CharSequence being tested contains any match for the given regular expression pattern. The test used is equivalent to pattern.matcher(arg).find() |
| `com.google.common.base.Predicates` | `Predicate<CharSequence> containsPattern(String pattern)` | 【原文待译】Returns a predicate that evaluates to true if the CharSequence being tested contains any match for the given regular expression pattern. The test used is equivalent to Pattern.compile(pattern).matcher(arg).find() |
| `com.google.common.base.Predicates` | `Predicate<Class<?>> subtypeOf(Class<?> clazz)` | 【原文待译】Returns a predicate that evaluates to true if the class being tested is assignable to (is a subtype of) clazz. Example: {@snippet : List > classes = Arrays.asList( Object.class, String.class, Number.class, Long.class); return Iterables.filter(classes, subtypeOf(Number.class)); } The code above retur… |
| `com.google.common.base.Predicates` | `Predicate<T> alwaysFalse()` | 【原文待译】Returns a predicate that always evaluates to false. |
| `com.google.common.base.Predicates` | `Predicate<T> alwaysTrue()` | 【原文待译】Returns a predicate that always evaluates to true. |
| `com.google.common.base.Predicates` | `Predicate<T> and(Iterable<? extends Predicate<? super T>> components)` | 【原文待译】Returns a predicate that evaluates to true if each of its components evaluates to true. The components are evaluated in order, and evaluation will be "short-circuited" as soon as a false predicate is found. It defensively copies the iterable passed in, so future changes to it won't alter the behavio… |
| `com.google.common.base.Predicates` | `Predicate<T> and(Predicate<? super T> first,Predicate<? super T> second)` | 【原文待译】Returns a predicate that evaluates to true if both of its components evaluate to true. The components are evaluated in order, and evaluation will be "short-circuited" as soon as a false predicate is found. |
| `com.google.common.base.Predicates` | `Predicate<T> and(Predicate<? super T>... components)` | 【原文待译】Returns a predicate that evaluates to true if each of its components evaluates to true. The components are evaluated in order, and evaluation will be "short-circuited" as soon as a false predicate is found. It defensively copies the array passed in, so future changes to it won't alter the behavior o… |
| `com.google.common.base.Predicates` | `Predicate<T> equalTo(@ParametricNullness
T target)` | 【原文待译】Returns a predicate that evaluates to true if the object being tested equals() the given target or both are null. |
| `com.google.common.base.Predicates` | `Predicate<T> in(Collection<? extends T> target)` | 【原文待译】Returns a predicate that evaluates to true if the object reference being tested is a member of the given collection. It does not defensively copy the collection passed in, so future changes to it will alter the behavior of the predicate. This method can technically accept any Collection , but using … |
| `com.google.common.base.Predicates` | `Predicate<T> instanceOf(Class<?> clazz)` | 【原文待译】Returns a predicate that evaluates to true if the object being tested is an instance of the given class. If the object being tested is null this predicate evaluates to false. If you want to filter an Iterable to narrow its type, consider using com.google.common.collect.Iterables#filter(Iterable, Cla… |
| `com.google.common.base.Predicates` | `Predicate<T> isNull()` | 【原文待译】Returns a predicate that evaluates to true if the object reference being tested is null. |
| `com.google.common.base.Predicates` | `Predicate<T> not(Predicate<T> predicate)` | 【原文待译】Returns a predicate that evaluates to true if the given predicate evaluates to false. |
| `com.google.common.base.Predicates` | `Predicate<T> notNull()` | 【原文待译】Returns a predicate that evaluates to true if the object reference being tested is not null. |
| `com.google.common.base.Predicates` | `Predicate<T> or(Iterable<? extends Predicate<? super T>> components)` | 【原文待译】Returns a predicate that evaluates to true if any one of its components evaluates to true. The components are evaluated in order, and evaluation will be "short-circuited" as soon as a true predicate is found. It defensively copies the iterable passed in, so future changes to it won't alter the behav… |
| `com.google.common.base.Predicates` | `Predicate<T> or(Predicate<? super T> first,Predicate<? super T> second)` | 【原文待译】Returns a predicate that evaluates to true if either of its components evaluates to true. The components are evaluated in order, and evaluation will be "short-circuited" as soon as a true predicate is found. |
| `com.google.common.base.Predicates` | `Predicate<T> or(Predicate<? super T>... components)` | 【原文待译】Returns a predicate that evaluates to true if any one of its components evaluates to true. The components are evaluated in order, and evaluation will be "short-circuited" as soon as a true predicate is found. It defensively copies the array passed in, so future changes to it won't alter the behavior… |
| `com.google.common.base.Splitter` | `Iterable<String> split(CharSequence sequence)` | 【原文待译】Splits sequence into string components and makes them available through an Iterator, which may be lazily evaluated. If you want an eagerly computed List, use #splitToList(CharSequence). Java 8+ users may prefer #splitToStream instead. |
| `com.google.common.base.Splitter` | `List<String> splitToList(CharSequence sequence)` | 【原文待译】Splits sequence into string components and returns them as an immutable list. If you want an Iterable which may be lazily evaluated, use #split(CharSequence). |
| `com.google.common.base.Splitter` | `MapSplitter withKeyValueSeparator(Splitter keyValueSplitter)` | 【原文待译】Returns a MapSplitter which splits entries based on this splitter, and splits entries into keys and values using the specified key-value splitter. Note: Any configuration option configured on this splitter, such as #trimResults, does not change the behavior of the keyValueSplitter. Example: {@snippe… |
| `com.google.common.base.Splitter` | `MapSplitter withKeyValueSeparator(String separator)` | 【原文待译】Returns a MapSplitter which splits entries based on this splitter, and splits entries into keys and values using the specified separator. |
| `com.google.common.base.Splitter` | `MapSplitter withKeyValueSeparator(char separator)` | 【原文待译】Returns a MapSplitter which splits entries based on this splitter, and splits entries into keys and values using the specified separator. |
| `com.google.common.base.Splitter` | `Splitter fixedLength(int length)` | 【原文待译】Returns a splitter that divides strings into pieces of the given length. For example, Splitter.fixedLength(2).split("abcde") returns an iterable containing ["ab", "cd", "e"]. The last piece can be smaller than length but will never be empty. Note: if #fixedLength is used in conjunction with #limit, … |
| `com.google.common.base.Splitter` | `Splitter limit(int maxItems)` | 【原文待译】Returns a splitter that behaves equivalently to this splitter but stops splitting after it reaches the limit. The limit defines the maximum number of items returned by the iterator, or the maximum size of the list returned by #splitToList. For example, Splitter.on(',').limit(3).split("a,b,c,d") retu… |
| `com.google.common.base.Splitter` | `Splitter omitEmptyStrings()` | 【原文待译】Returns a splitter that behaves equivalently to this splitter, but automatically omits empty strings from the results. For example, Splitter.on(',').omitEmptyStrings().split(",a,,,b,c,,") returns an iterable containing only ["a", "b", "c"]. If either trimResults option is also specified when creatin… |
| `com.google.common.base.Splitter` | `Splitter on(CharMatcher separatorMatcher)` | 【原文待译】Returns a splitter that considers any single character matched by the given CharMatcher to be a separator. For example, Splitter.on(CharMatcher.anyOf(";,")).split("foo,;bar,quux") returns an iterable containing ["foo", "", "bar", "quux"]. |
| `com.google.common.base.Splitter` | `Splitter on(Pattern separatorPattern)` | 【原文待译】Returns a splitter that considers any subsequence matching pattern to be a separator. For example, Splitter.on(Pattern.compile("\r?\n")).split(entireFile) splits a string into lines whether it uses DOS-style or UNIX-style line terminators. |
| `com.google.common.base.Splitter` | `Splitter on(String separator)` | 【原文待译】Returns a splitter that uses the given fixed string as a separator. For example, Splitter.on(", ").split("foo, bar,baz") returns an iterable containing ["foo", "bar,baz"]. |
| `com.google.common.base.Splitter` | `Splitter on(char separator)` | 【原文待译】Returns a splitter that uses the given single-character separator. For example, Splitter.on(',').split("foo,,bar") returns an iterable containing ["foo", "", "bar"]. |
| `com.google.common.base.Splitter` | `Splitter onPattern(String separatorPattern)` | 【原文待译】Returns a splitter that considers any subsequence matching a given pattern (regular expression) to be a separator. For example, Splitter.onPattern("\r?\n").split(entireFile) splits a string into lines whether it uses DOS-style or UNIX-style line terminators. This is equivalent to Splitter.on(Pattern… |
| `com.google.common.base.Splitter` | `Splitter trimResults()` | 【原文待译】Returns a splitter that behaves equivalently to this splitter, but automatically removes leading and trailing {@linkplain CharMatcher#whitespace whitespace} from each returned substring; equivalent to trimResults(CharMatcher.whitespace()). For example, Splitter.on(',').trimResults().split(" a, b ,c … |
| `com.google.common.base.Splitter` | `Splitter trimResults(CharMatcher trimmer)` | 【原文待译】Returns a splitter that behaves equivalently to this splitter, but removes all leading or trailing characters matching the given CharMatcher from each returned substring. For example, Splitter.on(',').trimResults(CharMatcher.is('_')).split("_a ,_b_ ,c__") returns an iterable containing ["a ", "b_ ",… |
| `com.google.common.base.Splitter` | `Stream<String> splitToStream(CharSequence sequence)` | 【原文待译】Splits sequence into string components and makes them available through an Stream, which may be lazily evaluated. If you want an eagerly computed List, use #splitToList(CharSequence). |
| `com.google.common.base.Splitter$MapSplitter` | `Map<String, String> split(CharSequence sequence)` | 【原文待译】Splits sequence into substrings, splits each substring into an entry, and returns an unmodifiable map with each of the entries. For example, Splitter.on(';').trimResults().withKeyValueSeparator("=>").split("a=>b ; c=>b") will return a mapping from "a" to "b" and "c" to "b". The returned map preserve… |
| `com.google.common.base.StandardSystemProperty` | `String key()` | 【原文待译】Returns the key used to look up this system property. |
| `com.google.common.base.StandardSystemProperty` | `String toString()` | 【原文待译】Returns a string representation of this system property. |
| `com.google.common.base.StandardSystemProperty` | `String value()` | 【原文待译】Returns the current value for this system property by delegating to System#getProperty(String). The value returned by this method is non-null except in rare circumstances: #JAVA_EXT_DIRS was deprecated in Java 8 and removed in Java 9. We have not confirmed whether it is available under older version… |
| `com.google.common.base.Stopwatch` | `Duration elapsed()` | 【原文待译】Returns the current elapsed time shown on this stopwatch as a Duration. Unlike #elapsed(TimeUnit), this method does not lose any precision due to rounding. |
| `com.google.common.base.Stopwatch` | `Stopwatch createStarted()` | 【原文待译】Creates (and starts) a new stopwatch using System#nanoTime as its time source. |
| `com.google.common.base.Stopwatch` | `Stopwatch createStarted(Ticker ticker)` | 【原文待译】Creates (and starts) a new stopwatch, using the specified time source. |
| `com.google.common.base.Stopwatch` | `Stopwatch createUnstarted()` | 【原文待译】Creates (but does not start) a new stopwatch using System#nanoTime as its time source. |
| `com.google.common.base.Stopwatch` | `Stopwatch createUnstarted(Ticker ticker)` | 【原文待译】Creates (but does not start) a new stopwatch, using the specified time source. |
| `com.google.common.base.Stopwatch` | `Stopwatch reset()` | 【原文待译】Sets the elapsed time for this stopwatch to zero, and places it in a stopped state. |
| `com.google.common.base.Stopwatch` | `Stopwatch start()` | 【原文待译】Starts the stopwatch. |
| `com.google.common.base.Stopwatch` | `Stopwatch stop()` | 【原文待译】Stops the stopwatch. Future reads will return the fixed duration that had elapsed up to this point. |
| `com.google.common.base.Stopwatch` | `String toString()` | 【原文待译】Returns a string representation of the current elapsed time. |
| `com.google.common.base.Stopwatch` | `boolean isRunning()` | 【原文待译】Returns true if #start() has been called on this stopwatch, and #stop() has not been called since the last call to start(). |
| `com.google.common.base.Stopwatch` | `long elapsed(TimeUnit desiredUnit)` | 【原文待译】Returns the current elapsed time shown on this stopwatch, expressed in the desired time unit, with any fraction rounded down. Note: the overhead of measurement can be more than a microsecond, so it is generally not useful to specify TimeUnit#NANOSECONDS precision here. It is generally not a good ide… |
| `com.google.common.base.Strings` | `String commonPrefix(CharSequence a,CharSequence b)` | 【原文待译】Returns the longest string prefix such that a.toString().startsWith(prefix) && b.toString().startsWith(prefix), taking care not to split surrogate pairs. If a and b have no common prefix, returns the empty string. |
| `com.google.common.base.Strings` | `String commonSuffix(CharSequence a,CharSequence b)` | 【原文待译】Returns the longest string suffix such that a.toString().endsWith(suffix) && b.toString().endsWith(suffix), taking care not to split surrogate pairs. If a and b have no common suffix, returns the empty string. |
| `com.google.common.base.Strings` | `String emptyToNull(@Nullable
String string)` | 【原文待译】Returns the given string if it is nonempty; null otherwise. |
| `com.google.common.base.Strings` | `String lenientFormat(@Nullable
String template,@Nullable
Object @Nullable ... args)` | 【原文待译】Returns the given template string with each occurrence of "%s" replaced with the corresponding argument value from args; or, if the placeholder and argument counts do not match, returns a best-effort form of that string. Will not throw an exception under normal conditions. Note: For most string-form… |
| `com.google.common.base.Strings` | `String nullToEmpty(@Nullable
String string)` | 【原文待译】Returns the given string if it is non-null; the empty string otherwise. |
| `com.google.common.base.Strings` | `String padEnd(String string,int minLength,char padChar)` | 【原文待译】Returns a string, of length at least minLength, consisting of string appended with as many copies of padChar as are necessary to reach that length. For example, padEnd("4.", 5, '0') returns "4.000" padEnd("2010", 3, '!') returns "2010" See java.util.Formatter for a richer set of formatting capabilit… |
| `com.google.common.base.Strings` | `String padStart(String string,int minLength,char padChar)` | 【原文待译】Returns a string, of length at least minLength, consisting of string prepended with as many copies of padChar as are necessary to reach that length. For example, padStart("7", 3, '0') returns "007" padStart("2010", 3, '0') returns "2010" See java.util.Formatter for a richer set of formatting capabil… |
| `com.google.common.base.Strings` | `String repeat(String string,int count)` | 【原文待译】Returns a string consisting of a specific number of concatenated copies of an input string. For example, repeat("hey", 3) returns the string "heyheyhey". Java 11+ users: use string.repeat(count) instead. |
| `com.google.common.base.Strings` | `boolean isNullOrEmpty(@Nullable
String string)` | 【原文待译】Returns true if the given string is null or is the empty string. Consider normalizing your string references with #nullToEmpty. If you do, you can use String#isEmpty() instead of this method, and you won't need special null-safe forms of methods like String#toUpperCase either. Or, if you'd like to n… |
| `com.google.common.base.Supplier` | `T get()` | 【原文待译】Retrieves an instance of the appropriate type. The returned object may or may not be a new instance, depending on the implementation. |
| `com.google.common.base.Suppliers` | `Function<Supplier<T>, T> supplierFunction()` | 【原文待译】Returns a function that accepts a supplier and returns the result of invoking Supplier#get on that supplier. Java 8+ users: use the method reference Supplier::get instead. |
| `com.google.common.base.Suppliers` | `Supplier<T> compose(Function<? super F, T> function,Supplier<F> supplier)` | 【原文待译】Returns a new supplier which is the composition of the provided function and supplier. In other words, the new supplier's value will be computed by retrieving the value from supplier, and then applying function to that value. Note that the resulting supplier will not call supplier or invoke function… |
| `com.google.common.base.Suppliers` | `Supplier<T> memoize(Supplier<T> delegate)` | 【原文待译】Returns a supplier which caches the instance retrieved during the first call to get() and returns that value on subsequent calls to get(). See: memoization The returned supplier is thread-safe. The delegate's get() method will be invoked at most once unless the underlying get() throws an exception. … |
| `com.google.common.base.Suppliers` | `Supplier<T> memoizeWithExpiration(Supplier<T> delegate,Duration duration)` | 【原文待译】Returns a supplier that caches the instance supplied by the delegate and removes the cached value after the specified time has passed. Subsequent calls to get() return the cached value if the expiration time has not passed. After the expiration time, a new value is retrieved, cached, and returned. S… |
| `com.google.common.base.Suppliers` | `Supplier<T> memoizeWithExpiration(Supplier<T> delegate,long duration,TimeUnit unit)` | 【原文待译】Returns a supplier that caches the instance supplied by the delegate and removes the cached value after the specified time has passed. Subsequent calls to get() return the cached value if the expiration time has not passed. After the expiration time, a new value is retrieved, cached, and returned. S… |
| `com.google.common.base.Suppliers` | `Supplier<T> ofInstance(@ParametricNullness
T instance)` | 【原文待译】Returns a supplier that always supplies instance. |
| `com.google.common.base.Suppliers` | `Supplier<T> synchronizedSupplier(Supplier<T> delegate)` | 【原文待译】Returns a supplier whose get() method synchronizes on delegate before calling it, making it thread-safe. |
| `com.google.common.base.Throwables` | `List<StackTraceElement> lazyStackTrace(Throwable throwable)` | 【原文待译】Returns the stack trace of throwable, possibly providing slower iteration over the full trace but faster iteration over parts of the trace. Here, "slower" and "faster" are defined in comparison to the normal way to access the stack trace, Throwable#getStackTrace() throwable.getStackTrace(). Note, ho… |
| `com.google.common.base.Throwables` | `List<Throwable> getCausalChain(Throwable throwable)` | 【原文待译】Gets a Throwable cause chain as a list. The first entry in the list will be throwable followed by its cause hierarchy. Note that this is a snapshot of the cause chain and will not reflect any subsequent changes to the cause chain. Here's an example of how it can be used to find specific types of exc… |
| `com.google.common.base.Throwables` | `RuntimeException propagate(Throwable throwable)` | 【原文待译】Propagates throwable as-is if it is an instance of RuntimeException or Error, or else as a last resort, wraps it in a RuntimeException and then propagates. This method always throws an exception. The RuntimeException return type allows client code to signal to the compiler that statements after the … |
| `com.google.common.base.Throwables` | `String getStackTraceAsString(Throwable throwable)` | 【原文待译】Returns a string containing the result of Throwable#toString() toString(), followed by the full, recursive stack trace of throwable. Note that you probably should not be parsing the resulting string; if you need programmatic access to the stack frames, you can call Throwable#getStackTrace(). |
| `com.google.common.base.Throwables` | `Throwable getRootCause(Throwable throwable)` | 【原文待译】Returns the innermost cause of throwable. The first throwable in a chain provides context from when the error or exception was initially detected. Example usage: |
| `com.google.common.base.Throwables` | `X getCauseAs(Throwable throwable,Class<X> expectedCauseType)` | 【原文待译】Returns throwable's cause, cast to expectedCauseType. Prefer this method instead of manually casting an exception's cause. For example, (IOException) e.getCause() throws a ClassCastException that discards the original exception e if the cause is not an IOException, but Throwables.getCauseAs(e, IOExc… |
| `com.google.common.base.Throwables` | `boolean lazyStackTraceIsLazy()` | 【原文待译】Returns whether #lazyStackTrace will use the special implementation described in its documentation. |
| `com.google.common.base.Throwables` | `void propagateIfInstanceOf(@Nullable
Throwable throwable,Class<X> declaredType)` | 【原文待译】Propagates throwable exactly as-is, if and only if it is an instance of declaredType. Example usage: |
| `com.google.common.base.Throwables` | `void propagateIfPossible(@Nullable
Throwable throwable)` | 【原文待译】Propagates throwable exactly as-is, if and only if it is an instance of RuntimeException or Error. |
| `com.google.common.base.Throwables` | `void propagateIfPossible(@Nullable
Throwable throwable,Class<X1> declaredType1,Class<X2> declaredType2)` | 【原文待译】Propagates throwable exactly as-is, if and only if it is an instance of RuntimeException, Error, declaredType1, or declaredType2. |
| `com.google.common.base.Throwables` | `void propagateIfPossible(@Nullable
Throwable throwable,Class<X> declaredType)` | 【原文待译】Propagates throwable exactly as-is, if and only if it is an instance of RuntimeException, Error, or declaredType. Discouraged in favor of calling #throwIfInstanceOf and #throwIfUnchecked. |
| `com.google.common.base.Throwables` | `void throwIfInstanceOf(Throwable throwable,Class<X> declaredType)` | 【原文待译】Throws throwable if it is an instance of declaredType. Example usage: |
| `com.google.common.base.Throwables` | `void throwIfUnchecked(Throwable throwable)` | 【原文待译】Throws throwable if it is a RuntimeException or Error. Example usage: |
| `com.google.common.base.Ticker` | `Ticker systemTicker()` | 【原文待译】A ticker that reads the current time using System#nanoTime. |
| `com.google.common.base.Ticker` | `long read()` | 【原文待译】Returns the number of nanoseconds elapsed since this ticker's fixed point of reference. |
| `com.google.common.base.Utf8` | `boolean isWellFormed(byte[] bytes)` | 【原文待译】Returns true if bytes is a well-formed UTF-8 byte sequence according to Unicode 6.0. Note that this is a stronger criterion than simply whether the bytes can be decoded. For example, some versions of the JDK decoder will accept "non-shortest form" byte sequences, but encoding never reproduces these.… |
| `com.google.common.base.Utf8` | `boolean isWellFormed(byte[] bytes,int off,int len)` | 【原文待译】Returns whether the given byte array slice is a well-formed UTF-8 byte sequence, as defined by #isWellFormed(byte[]). Note that this can be false even when isWellFormed(bytes) is true. |
| `com.google.common.base.Utf8` | `int encodedLength(CharSequence sequence)` | 【原文待译】Returns the number of bytes in the UTF-8-encoded form of sequence. For a string, this method is equivalent to string.getBytes(UTF_8).length, but is more efficient in both time and space. |
| `com.google.common.base.Verify` | `T verifyNotNull(@Nullable
T reference)` | 【原文待译】Ensures that reference is non-null, throwing a VerifyException with a default message otherwise. |
| `com.google.common.base.Verify` | `T verifyNotNull(@Nullable
T reference,String errorMessageTemplate,@Nullable
Object @Nullable ... errorMessageArgs)` | 【原文待译】Ensures that reference is non-null, throwing a VerifyException with a custom message otherwise. |
| `com.google.common.base.Verify` | `void verify(boolean expression)` | 【原文待译】Ensures that expression is true, throwing a VerifyException with no message otherwise. |
| `com.google.common.base.Verify` | `void verify(boolean expression,String errorMessageTemplate,@Nullable
Object @Nullable ... errorMessageArgs)` | 【原文待译】Ensures that expression is true, throwing a VerifyException with a custom message otherwise. |
| `com.google.common.base.Verify` | `void verify(boolean expression,String errorMessageTemplate,@Nullable
Object p1)` | 【原文待译】Ensures that expression is true, throwing a VerifyException with a custom message otherwise. See #verify(boolean, String, Object...) for details. |
| `com.google.common.base.Verify` | `void verify(boolean expression,String errorMessageTemplate,@Nullable
Object p1,@Nullable
Object p2)` | 【原文待译】Ensures that expression is true, throwing a VerifyException with a custom message otherwise. See #verify(boolean, String, Object...) for details. |
| `com.google.common.base.Verify` | `void verify(boolean expression,String errorMessageTemplate,@Nullable
Object p1,@Nullable
Object p2,@Nullable
Object p3)` | 【原文待译】Ensures that expression is true, throwing a VerifyException with a custom message otherwise. See #verify(boolean, String, Object...) for details. |
| `com.google.common.base.Verify` | `void verify(boolean expression,String errorMessageTemplate,@Nullable
Object p1,@Nullable
Object p2,@Nullable
Object p3,@Nullable
Object p4)` | 【原文待译】Ensures that expression is true, throwing a VerifyException with a custom message otherwise. See #verify(boolean, String, Object...) for details. |
| `com.google.common.base.Verify` | `void verify(boolean expression,String errorMessageTemplate,@Nullable
Object p1,char p2)` | 【原文待译】Ensures that expression is true, throwing a VerifyException with a custom message otherwise. See #verify(boolean, String, Object...) for details. |
| `com.google.common.base.Verify` | `void verify(boolean expression,String errorMessageTemplate,@Nullable
Object p1,int p2)` | 【原文待译】Ensures that expression is true, throwing a VerifyException with a custom message otherwise. See #verify(boolean, String, Object...) for details. |
| `com.google.common.base.Verify` | `void verify(boolean expression,String errorMessageTemplate,@Nullable
Object p1,long p2)` | 【原文待译】Ensures that expression is true, throwing a VerifyException with a custom message otherwise. See #verify(boolean, String, Object...) for details. |
| `com.google.common.base.Verify` | `void verify(boolean expression,String errorMessageTemplate,char p1)` | 【原文待译】Ensures that expression is true, throwing a VerifyException with a custom message otherwise. See #verify(boolean, String, Object...) for details. |
| `com.google.common.base.Verify` | `void verify(boolean expression,String errorMessageTemplate,char p1,@Nullable
Object p2)` | 【原文待译】Ensures that expression is true, throwing a VerifyException with a custom message otherwise. See #verify(boolean, String, Object...) for details. |
| `com.google.common.base.Verify` | `void verify(boolean expression,String errorMessageTemplate,char p1,char p2)` | 【原文待译】Ensures that expression is true, throwing a VerifyException with a custom message otherwise. See #verify(boolean, String, Object...) for details. |
| `com.google.common.base.Verify` | `void verify(boolean expression,String errorMessageTemplate,char p1,int p2)` | 【原文待译】Ensures that expression is true, throwing a VerifyException with a custom message otherwise. See #verify(boolean, String, Object...) for details. |
| `com.google.common.base.Verify` | `void verify(boolean expression,String errorMessageTemplate,char p1,long p2)` | 【原文待译】Ensures that expression is true, throwing a VerifyException with a custom message otherwise. See #verify(boolean, String, Object...) for details. |
| `com.google.common.base.Verify` | `void verify(boolean expression,String errorMessageTemplate,int p1)` | 【原文待译】Ensures that expression is true, throwing a VerifyException with a custom message otherwise. See #verify(boolean, String, Object...) for details. |
| `com.google.common.base.Verify` | `void verify(boolean expression,String errorMessageTemplate,int p1,@Nullable
Object p2)` | 【原文待译】Ensures that expression is true, throwing a VerifyException with a custom message otherwise. See #verify(boolean, String, Object...) for details. |
| `com.google.common.base.Verify` | `void verify(boolean expression,String errorMessageTemplate,int p1,char p2)` | 【原文待译】Ensures that expression is true, throwing a VerifyException with a custom message otherwise. See #verify(boolean, String, Object...) for details. |
| `com.google.common.base.Verify` | `void verify(boolean expression,String errorMessageTemplate,int p1,int p2)` | 【原文待译】Ensures that expression is true, throwing a VerifyException with a custom message otherwise. See #verify(boolean, String, Object...) for details. |
| `com.google.common.base.Verify` | `void verify(boolean expression,String errorMessageTemplate,int p1,long p2)` | 【原文待译】Ensures that expression is true, throwing a VerifyException with a custom message otherwise. See #verify(boolean, String, Object...) for details. |
| `com.google.common.base.Verify` | `void verify(boolean expression,String errorMessageTemplate,long p1)` | 【原文待译】Ensures that expression is true, throwing a VerifyException with a custom message otherwise. See #verify(boolean, String, Object...) for details. |
| `com.google.common.base.Verify` | `void verify(boolean expression,String errorMessageTemplate,long p1,@Nullable
Object p2)` | 【原文待译】Ensures that expression is true, throwing a VerifyException with a custom message otherwise. See #verify(boolean, String, Object...) for details. |
| `com.google.common.base.Verify` | `void verify(boolean expression,String errorMessageTemplate,long p1,char p2)` | 【原文待译】Ensures that expression is true, throwing a VerifyException with a custom message otherwise. See #verify(boolean, String, Object...) for details. |
| `com.google.common.base.Verify` | `void verify(boolean expression,String errorMessageTemplate,long p1,int p2)` | 【原文待译】Ensures that expression is true, throwing a VerifyException with a custom message otherwise. See #verify(boolean, String, Object...) for details. |
| `com.google.common.base.Verify` | `void verify(boolean expression,String errorMessageTemplate,long p1,long p2)` | 【原文待译】Ensures that expression is true, throwing a VerifyException with a custom message otherwise. See #verify(boolean, String, Object...) for details. |
