# cn.hutool.extra.validation

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.validation.BeanValidationResult`

```java
public class cn.hutool.extra.validation.BeanValidationResult {
  public cn.hutool.extra.validation.BeanValidationResult(boolean);
  public boolean isSuccess();
  public cn.hutool.extra.validation.BeanValidationResult setSuccess(boolean);
  public java.util.List<cn.hutool.extra.validation.BeanValidationResult$ErrorMessage> getErrorMessages();
  public cn.hutool.extra.validation.BeanValidationResult setErrorMessages(java.util.List<cn.hutool.extra.validation.BeanValidationResult$ErrorMessage>);
  public cn.hutool.extra.validation.BeanValidationResult addErrorMessage(cn.hutool.extra.validation.BeanValidationResult$ErrorMessage);
}
```

## `cn.hutool.extra.validation.BeanValidationResult$ErrorMessage`

```java
public class cn.hutool.extra.validation.BeanValidationResult$ErrorMessage {
  public cn.hutool.extra.validation.BeanValidationResult$ErrorMessage();
  public java.lang.String getPropertyName();
  public void setPropertyName(java.lang.String);
  public java.lang.String getMessage();
  public void setMessage(java.lang.String);
  public java.lang.Object getValue();
  public void setValue(java.lang.Object);
  public java.lang.String toString();
}
```

## `cn.hutool.extra.validation.ValidationUtil`

```java
public class cn.hutool.extra.validation.ValidationUtil {
  public cn.hutool.extra.validation.ValidationUtil();
  public static jakarta.validation.Validator getValidator();
  public static <T> java.util.Set<jakarta.validation.ConstraintViolation<T>> validate(T, java.lang.Class<?>...);
  public static <T> java.util.Set<jakarta.validation.ConstraintViolation<T>> validateProperty(T, java.lang.String, java.lang.Class<?>...);
  public static <T> cn.hutool.extra.validation.BeanValidationResult warpValidate(T, java.lang.Class<?>...);
  public static <T> cn.hutool.extra.validation.BeanValidationResult warpValidateProperty(T, java.lang.String, java.lang.Class<?>...);
}
```
