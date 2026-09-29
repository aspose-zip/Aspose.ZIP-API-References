---
title: "EventsBagIso"
second_title: "Aspose.ZIP for Java API 参考"
description: "用于保存时的事件容器。"
type: docs
weight: 66
url: /zh/java/com.aspose.zip/eventsbagiso/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagIso
```

用于在 [IsoArchive](../../com.aspose.zip/isoarchive) 保存时的事件容器。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [EventsBagIso()](#EventsBagIso--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | 获取在压缩归档条目之前触发的事件。 |
| [getEntryCompressed()](#getEntryCompressed--) | 获取在归档条目压缩完成后触发的事件。 |
| [setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | 设置在压缩归档条目之前触发的事件。 |
| [setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | 设置在归档条目压缩完成后触发的事件。 |
### EventsBagIso() {#EventsBagIso--}
```
public EventsBagIso()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsIso> getEntryAccessed()
```


获取在压缩归档条目之前触发的事件。

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<EntryEventArgsIso> getEntryCompressed()
```


获取在归档条目压缩完成后触发的事件。

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryAccessed(Event<EntryEventArgsIso> value)
```


设置在压缩归档条目之前触发的事件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | 在归档条目被压缩之前触发的事件。 |

### setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryCompressed(Event<EntryEventArgsIso> value)
```


设置在归档条目压缩完成后触发的事件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | 在归档条目被压缩之后触发的事件 |

