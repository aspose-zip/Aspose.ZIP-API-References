---
title: "EventsBagXar"
second_title: "Aspose.ZIP for Java API 参考"
description: "用于保存时的事件容器。"
type: docs
weight: 67
url: /zh/java/com.aspose.zip/eventsbagxar/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagXar
```

用于在 [XarArchive](../../com.aspose.zip/xararchive) 保存时的事件容器。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [EventsBagXar()](#EventsBagXar--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | 获取在压缩归档条目之前触发的事件。 |
| [getEntryCompressed()](#getEntryCompressed--) | 获取在归档条目压缩完成后触发的事件。 |
| [setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--) | 设置在压缩归档条目之前触发的事件。 |
| [setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--) | 设置在归档条目压缩完成后触发的事件。 |
### EventsBagXar() {#EventsBagXar--}
```
public EventsBagXar()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsXar> getEntryAccessed()
```


获取在压缩归档条目之前触发的事件。

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgsXar> getEntryCompressed()
```


获取在归档条目压缩完成后触发的事件。

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--}
```
public void setEntryAccessed(Event<EntryEventArgsXar> value)
```


设置在压缩归档条目之前触发的事件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsXar&gt; | 在归档条目被压缩之前触发的事件。 |

### setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--}
```
public void setEntryCompressed(Event<CancelEntryEventArgsXar> value)
```


设置在归档条目压缩完成后触发的事件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgsXar&gt; | 在归档条目被压缩之后触发的事件 |

