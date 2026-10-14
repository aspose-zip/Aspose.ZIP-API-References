---
title: "事件"
second_title: "Aspose.ZIP for Java API 参考"
description: "一个事件。"
type: docs
weight: 160
url: /zh/java/com.aspose.zip/event/
---
```
public interface Event<TArgs>
```

一个事件。

`TArgs`：事件参数。

TArgs：
## 方法

| 方法 | 描述 |
| --- | --- |
| [invoke(Object sender, TArgs args)](#invoke-java.lang.Object-TArgs-) | 当事件被触发时，将调用此方法。 |
### invoke(Object sender, TArgs args) {#invoke-java.lang.Object-TArgs-}
```
public abstract void invoke(Object sender, TArgs args)
```


当事件被触发时，将调用此方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 发送者 | java.lang.Object | 触发此事件的对象。 |
| 参数 | TArgs | 自定义参数。 |

