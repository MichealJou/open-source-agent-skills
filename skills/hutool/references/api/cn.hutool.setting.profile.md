# cn.hutool.setting.profile

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.setting.profile.GlobalProfile`

```java
public class cn.hutool.setting.profile.GlobalProfile {
  public static cn.hutool.setting.profile.Profile setProfile(java.lang.String);
  public static cn.hutool.setting.Setting getSetting(java.lang.String);
}
```

## `cn.hutool.setting.profile.Profile`

```java
public class cn.hutool.setting.profile.Profile implements java.io.Serializable {
  public cn.hutool.setting.profile.Profile();
  public cn.hutool.setting.profile.Profile(java.lang.String);
  public cn.hutool.setting.profile.Profile(java.lang.String, java.nio.charset.Charset, boolean);
  public cn.hutool.setting.Setting getSetting(java.lang.String);
  public cn.hutool.setting.profile.Profile setProfile(java.lang.String);
  public cn.hutool.setting.profile.Profile setCharset(java.nio.charset.Charset);
  public cn.hutool.setting.profile.Profile setUseVar(boolean);
  public cn.hutool.setting.profile.Profile clear();
}
```
