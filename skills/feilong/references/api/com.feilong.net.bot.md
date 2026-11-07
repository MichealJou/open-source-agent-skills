# com.feilong.net.bot

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.net.bot.AbstractBot`

```java
public abstract class com.feilong.net.bot.AbstractBot implements com.feilong.net.bot.Bot {
  public com.feilong.net.bot.AbstractBot();
  public boolean sendMessage(java.lang.String);
  public boolean sendMessage(java.lang.String, com.feilong.net.bot.message.MessageParams);
  public boolean getIsCatchException();
  public void setIsCatchException(boolean);
  public boolean getIsThrowException();
  public void setIsThrowException(boolean);
  public boolean getIsAsync();
  public void setIsAsync(boolean);
}
```

## `com.feilong.net.bot.Bot`

```java
public interface com.feilong.net.bot.Bot {
  public abstract boolean sendMessage(java.lang.String);
  public abstract boolean sendMessage(java.lang.String, com.feilong.net.bot.message.MessageParams);
  public abstract java.lang.String getKey();
}
```

## `com.feilong.net.bot.CombinationConfig`

```java
public class com.feilong.net.bot.CombinationConfig {
  public com.feilong.net.bot.CombinationConfig();
  public com.feilong.net.bot.CombinationConfig(org.slf4j.Logger, com.feilong.net.bot.Bot, boolean);
  public com.feilong.net.bot.CombinationConfig(org.slf4j.Logger, com.feilong.net.bot.Bot, java.lang.String, boolean);
  public com.feilong.net.bot.CombinationConfig(org.slf4j.Logger, com.feilong.net.bot.Bot, java.lang.String, boolean, boolean);
  public org.slf4j.Logger getLogger();
  public void setLogger(org.slf4j.Logger);
  public com.feilong.net.bot.Bot getBot();
  public void setBot(com.feilong.net.bot.Bot);
  public java.lang.String getSignName();
  public void setSignName(java.lang.String);
  public boolean getIsPrintLog();
  public boolean getIsSendBotMessage();
  public void setIsPrintLog(boolean);
  public void setIsSendBotMessage(boolean);
}
```

## `com.feilong.net.bot.LogAndBotCombination`

```java
public class com.feilong.net.bot.LogAndBotCombination {
  public com.feilong.net.bot.LogAndBotCombination();
  public static void debug(org.slf4j.Logger, com.feilong.net.bot.Bot, java.lang.String, java.lang.Object...);
  public static void info(org.slf4j.Logger, com.feilong.net.bot.Bot, java.lang.String, java.lang.Object...);
  public static void warn(org.slf4j.Logger, com.feilong.net.bot.Bot, java.lang.String, java.lang.Object...);
  public static void error(org.slf4j.Logger, com.feilong.net.bot.Bot, java.lang.String, java.lang.Object...);
  public static void debug(com.feilong.net.bot.CombinationConfig, java.lang.String, java.lang.Object...);
  public static void info(com.feilong.net.bot.CombinationConfig, java.lang.String, java.lang.Object...);
  public static void warn(com.feilong.net.bot.CombinationConfig, java.lang.String, java.lang.Object...);
  public static void error(com.feilong.net.bot.CombinationConfig, java.lang.String, java.lang.Object...);
  public static void debugWithSignName(org.slf4j.Logger, com.feilong.net.bot.Bot, java.lang.String, java.lang.String, java.lang.Object...);
  public static void infoWithSignName(org.slf4j.Logger, com.feilong.net.bot.Bot, java.lang.String, java.lang.String, java.lang.Object...);
  public static void warnWithSignName(org.slf4j.Logger, com.feilong.net.bot.Bot, java.lang.String, java.lang.String, java.lang.Object...);
  public static void errorWithSignName(org.slf4j.Logger, com.feilong.net.bot.Bot, java.lang.String, java.lang.String, java.lang.Object...);
}
```

## `com.feilong.net.bot.MarkdownHelper`

```java
public class com.feilong.net.bot.MarkdownHelper {
  public static java.lang.String font(java.lang.String, java.lang.String);
  public static java.lang.String link(java.lang.String, java.lang.String);
  public static java.lang.String b(java.lang.String);
  public static java.lang.String newLine();
}
```

## `com.feilong.net.bot.MarkdownStringCreator`

```java
public class com.feilong.net.bot.MarkdownStringCreator {
  public static java.lang.String createListString(java.lang.String, java.util.Map<java.lang.String, java.lang.String>);
}
```
