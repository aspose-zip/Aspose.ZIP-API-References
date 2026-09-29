---
title: "CancelEntryEventArgs"
second_title: "Aspose.ZIP for Java API 参考"
description: "可取消条目相关事件的事件参数。"
type: docs
weight: 52
url: /zh/java/com.aspose.zip/cancelentryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgs](../../com.aspose.zip/entryeventargs)
```
public class CancelEntryEventArgs extends EntryEventArgs
```

可取消条目相关事件的事件参数。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [CancelEntryEventArgs(ArchiveEntry entry)](#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-) | 初始化 [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getCancel()](#getCancel--) | 获取指示事件是否应被取消的值。 |
| [setCancel(boolean value)](#setCancel-boolean-) | 设置指示事件是否应被取消的值。 |
### CancelEntryEventArgs(ArchiveEntry entry) {#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public CancelEntryEventArgs(ArchiveEntry entry)
```


初始化 [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | 事件触发的归档条目。 |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


获取指示事件是否应被取消的值。

**Returns:**
boolean - 如果应取消事件则为 true；否则为 false。
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


设置指示事件是否应被取消的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 布尔 | 如果应取消事件则为 true；否则为 false。 |

