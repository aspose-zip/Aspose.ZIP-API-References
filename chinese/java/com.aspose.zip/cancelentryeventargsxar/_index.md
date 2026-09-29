---
title: "CancelEntryEventArgsXar"
second_title: "Aspose.ZIP for Java API 参考"
description: "可取消条目相关事件的事件参数。"
type: docs
weight: 53
url: /zh/java/com.aspose.zip/cancelentryeventargsxar/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgsXar](../../com.aspose.zip/entryeventargsxar)
```
public class CancelEntryEventArgsXar extends EntryEventArgsXar
```

可取消条目相关事件的事件参数。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [CancelEntryEventArgsXar(XarEntry entry)](#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-) | 初始化 [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getCancel()](#getCancel--) | 获取指示事件是否应被取消的值。 |
| [setCancel(boolean value)](#setCancel-boolean-) | 设置指示事件是否应被取消的值。 |
### CancelEntryEventArgsXar(XarEntry entry) {#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-}
```
public CancelEntryEventArgsXar(XarEntry entry)
```


初始化 [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | 存档条目触发此事件的对象 |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


获取指示事件是否应被取消的值。

**Returns:**
boolean - 如果应取消事件则为 true；否则为 false
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


设置指示事件是否应被取消的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 布尔 | 如果应取消事件则为 true；否则为 false |

