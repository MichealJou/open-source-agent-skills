# com.google.common.eventbus

版本 33.4.8-jre。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.google.common.eventbus.DeadEvent` | `Object getEvent()` | 【原文待译】Returns the wrapped, 'dead' event, which the system was unable to deliver to any registered subscriber. |
| `com.google.common.eventbus.DeadEvent` | `Object getSource()` | 【原文待译】Returns the object that originated this event ( not the object that originated the wrapped event). This is generally an EventBus. |
| `com.google.common.eventbus.DeadEvent` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.eventbus.EventBus` | `String identifier()` | 【原文待译】Returns the identifier for this event bus. |
| `com.google.common.eventbus.EventBus` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.google.common.eventbus.EventBus` | `void post(Object event)` | 【原文待译】Posts an event to all registered subscribers. This method will return successfully after the event has been posted to all subscribers, and regardless of any exceptions thrown by subscribers. If no subscribers have been subscribed for event's class, and event is not already a DeadEvent, it will be wr… |
| `com.google.common.eventbus.EventBus` | `void register(Object object)` | 【原文待译】Registers all subscriber methods on object to receive events. |
| `com.google.common.eventbus.EventBus` | `void unregister(Object object)` | 【原文待译】Unregisters all subscriber methods on a registered object. |
| `com.google.common.eventbus.SubscriberExceptionContext` | `EventBus getEventBus()` | 【原文待译】@return The EventBus that handled the event and the subscriber. Useful for broadcasting a new event based on the error. |
| `com.google.common.eventbus.SubscriberExceptionContext` | `Method getSubscriberMethod()` | 【原文待译】@return The subscribed method that threw the exception. |
| `com.google.common.eventbus.SubscriberExceptionContext` | `Object getEvent()` | 【原文待译】@return The event object that caused the subscriber to throw. |
| `com.google.common.eventbus.SubscriberExceptionContext` | `Object getSubscriber()` | 【原文待译】@return The object context that the subscriber was called on. |
| `com.google.common.eventbus.SubscriberExceptionHandler` | `void handleException(Throwable exception,SubscriberExceptionContext context)` | 【原文待译】Handles exceptions thrown by subscribers. |
