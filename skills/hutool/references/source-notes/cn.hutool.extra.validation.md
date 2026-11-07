# cn.hutool.extra.validation

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.extra.validation.BeanValidationResult` | `BeanValidationResult addErrorMessage(ErrorMessage errorMessage)` | 增加错误信息 |
| `cn.hutool.extra.validation.BeanValidationResult` | `BeanValidationResult setErrorMessages(List<ErrorMessage> errorMessages)` | 设置错误信息列表 |
| `cn.hutool.extra.validation.BeanValidationResult` | `BeanValidationResult setSuccess(boolean success)` | 设置是否通过 |
| `cn.hutool.extra.validation.BeanValidationResult` | `List<ErrorMessage> getErrorMessages()` | 获取错误信息列表 |
| `cn.hutool.extra.validation.BeanValidationResult` | `boolean isSuccess()` | 是否验证通过 |
| `cn.hutool.extra.validation.BeanValidationResult$ErrorMessage` | `Object getValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.validation.BeanValidationResult$ErrorMessage` | `String getMessage()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.validation.BeanValidationResult$ErrorMessage` | `String getPropertyName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.validation.BeanValidationResult$ErrorMessage` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.validation.BeanValidationResult$ErrorMessage` | `void setMessage(String message)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.validation.BeanValidationResult$ErrorMessage` | `void setPropertyName(String propertyName)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.validation.BeanValidationResult$ErrorMessage` | `void setValue(Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.validation.ValidationUtil` | `BeanValidationResult warpValidate(T bean,Class<?>... groups)` | 校验对象 |
| `cn.hutool.extra.validation.ValidationUtil` | `BeanValidationResult warpValidateProperty(T bean,String propertyName,Class<?>... groups)` | 校验bean的某一个属性 |
| `cn.hutool.extra.validation.ValidationUtil` | `Set<ConstraintViolation<T>> validate(T bean,Class<?>... groups)` | 校验对象 |
| `cn.hutool.extra.validation.ValidationUtil` | `Set<ConstraintViolation<T>> validateProperty(T bean,String propertyName,Class<?>... groups)` | 校验bean的某一个属性 |
| `cn.hutool.extra.validation.ValidationUtil` | `Validator getValidator()` | 获取原生Validator 对象 |
