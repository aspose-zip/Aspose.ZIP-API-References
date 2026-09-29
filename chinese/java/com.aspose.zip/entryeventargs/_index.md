---
title: "EntryEventArgs"
second_title: "Aspose.ZIP for Java API 参考"
description: "条目相关事件的事件参数。"
type: docs
weight: 62
url: /zh/java/com.aspose.zip/entryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgs extends System.EventArgs
```

条目相关事件的事件参数。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [EntryEventArgs(ArchiveEntry entry)](#EntryEventArgs-com.aspose.zip.ArchiveEntry-) | 初始化 [EntryEventArgs](../../com.aspose.zip/entryeventargs) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getEntry()](#getEntry--) | 获取触发事件的存档条目。 |
### EntryEventArgs(ArchiveEntry entry) {#EntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public EntryEventArgs(ArchiveEntry entry)
```


初始化 [EntryEventArgs](../../com.aspose.zip/entryeventargs) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | 事件触发的归档条目。 |

### getEntry() {#getEntry--}
```
public final ArchiveEntry getEntry()
```


获取触发事件的存档条目。

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - the archive entry the event is raised for.
