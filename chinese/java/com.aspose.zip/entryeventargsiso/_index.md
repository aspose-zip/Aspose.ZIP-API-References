---
title: "EntryEventArgsIso"
second_title: "Aspose.ZIP for Java API 参考"
description: "条目相关事件的事件参数。"
type: docs
weight: 63
url: /zh/java/com.aspose.zip/entryeventargsiso/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgsIso extends System.EventArgs
```

条目相关事件的事件参数。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [EntryEventArgsIso(IsoEntry entry)](#EntryEventArgsIso-com.aspose.zip.IsoEntry-) | 初始化 [EntryEventArgs](../../com.aspose.zip/entryeventargs) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getEntry()](#getEntry--) | 获取触发事件的存档条目。 |
### EntryEventArgsIso(IsoEntry entry) {#EntryEventArgsIso-com.aspose.zip.IsoEntry-}
```
public EntryEventArgsIso(IsoEntry entry)
```


初始化 [EntryEventArgs](../../com.aspose.zip/entryeventargs) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| entry | [IsoEntry](../../com.aspose.zip/isoentry) | 触发事件的存档条目 |

### getEntry() {#getEntry--}
```
public final IsoEntry getEntry()
```


获取触发事件的存档条目。

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the archive entry the event is raised for
