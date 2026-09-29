---
title: "EntryEventArgsXar"
second_title: "Aspose.ZIP for Java API 参考"
description: "条目相关事件的事件参数。"
type: docs
weight: 64
url: /zh/java/com.aspose.zip/entryeventargsxar/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgsXar extends System.EventArgs
```

条目相关事件的事件参数。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [EntryEventArgsXar(XarEntry entry)](#EntryEventArgsXar-com.aspose.zip.XarEntry-) | 初始化 [EntryEventArgs](../../com.aspose.zip/entryeventargs) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getEntry()](#getEntry--) | 获取触发事件的存档条目。 |
### EntryEventArgsXar(XarEntry entry) {#EntryEventArgsXar-com.aspose.zip.XarEntry-}
```
public EntryEventArgsXar(XarEntry entry)
```


初始化 [EntryEventArgs](../../com.aspose.zip/entryeventargs) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | 触发事件的存档条目 |

### getEntry() {#getEntry--}
```
public final XarEntry getEntry()
```


获取触发事件的存档条目。

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - the archive entry the event is raised for
